# Comparing `tmp/openeo_processes_dask-2023.5.1.tar.gz` & `tmp/openeo_processes_dask-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openeo_processes_dask-2023.5.1.tar", max compression
+gzip compressed data, was "openeo_processes_dask-2023.7.0.tar", max compression
```

## Comparing `openeo_processes_dask-2023.5.1.tar` & `openeo_processes_dask-2023.7.0.tar`

### file list

```diff
@@ -1,204 +1,207 @@
--rw-r--r--   0        0        0    10765 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/LICENSE
--rw-r--r--   0        0        0     3067 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/README.md
--rw-r--r--   0        0        0       25 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/__init__.py
--rw-r--r--   0        0        0      781 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/__init__.py
--rw-r--r--   0        0        0    10187 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/arrays.py
--rw-r--r--   0        0        0     2997 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/comparison.py
--rw-r--r--   0        0        0     3944 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/core.py
--rw-r--r--   0        0        0      135 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/__init__.py
--rw-r--r--   0        0        0     3232 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/_filter.py
--rw-r--r--   0        0        0     2976 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/_xr_interop.py
--rw-r--r--   0        0        0     3820 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/aggregate.py
--rw-r--r--   0        0        0     2256 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/apply.py
--rw-r--r--   0        0        0     2617 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/experimental.py
--rw-r--r--   0        0        0     2179 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/general.py
--rw-r--r--   0        0        0    10376 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/merge.py
--rw-r--r--   0        0        0     1814 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/reduce.py
--rw-r--r--   0        0        0      443 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/utils.py
--rw-r--r--   0        0        0      221 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/data_model.py
--rw-r--r--   0        0        0      868 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/exceptions.py
--rw-r--r--   0        0        0       24 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/experimental/__init__.py
--rw-r--r--   0        0        0     2545 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/experimental/resample.py
--rw-r--r--   0        0        0     7821 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/math.py
--rw-r--r--   0        0        0       29 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/ml/__init__.py
--rw-r--r--   0        0        0     2846 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/ml/random_forest.py
--rw-r--r--   0        0        0      233 2023-05-19 11:47:02.047792 openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/utils.py
--rw-r--r--   0        0        0      892 2023-05-19 11:47:02.051792 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/__init__.py
--rw-r--r--   0        0        0       75 2023-05-19 11:47:02.779789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/.git
--rw-r--r--   0        0        0       27 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      445 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/issue-or-clarification-for-existing-process.md
--rw-r--r--   0        0        0      856 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-parameter.md
--rw-r--r--   0        0        0     1516 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-proposal.md
--rw-r--r--   0        0        0      167 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/other.md
--rw-r--r--   0        0        0     1953 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/.github/workflows/docs.yml
--rw-r--r--   0        0        0      329 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/.github/workflows/tests.yml
--rw-r--r--   0        0        0    19276 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/LICENSE
--rw-r--r--   0        0        0     4577 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/README.md
--rw-r--r--   0        0        0     2325 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/absolute.json
--rw-r--r--   0        0        0     2390 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/add.json
--rw-r--r--   0        0        0     1981 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/add_dimension.json
--rw-r--r--   0        0        0     6149 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/aggregate_spatial.json
--rw-r--r--   0        0        0    10450 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/aggregate_temporal.json
--rw-r--r--   0        0        0     7320 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/aggregate_temporal_period.json
--rw-r--r--   0        0        0     3799 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/all.json
--rw-r--r--   0        0        0     2371 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/and.json
--rw-r--r--   0        0        0     3768 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/any.json
--rw-r--r--   0        0        0     2737 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/apply.json
--rw-r--r--   0        0        0     6430 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/apply_dimension.json
--rw-r--r--   0        0        0     1145 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arccos.json
--rw-r--r--   0        0        0     1192 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arcosh.json
--rw-r--r--   0        0        0     1133 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arcsin.json
--rw-r--r--   0        0        0     1151 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arctan.json
--rw-r--r--   0        0        0     1720 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arctan2.json
--rw-r--r--   0        0        0     5380 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/ard_normalized_radar_backscatter.json
--rw-r--r--   0        0        0     6009 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/ard_surface_reflectance.json
--rw-r--r--   0        0        0     1591 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_concat.json
--rw-r--r--   0        0        0     4992 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_contains.json
--rw-r--r--   0        0        0     2619 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_create.json
--rw-r--r--   0        0        0     3377 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_element.json
--rw-r--r--   0        0        0     3594 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_filter.json
--rw-r--r--   0        0        0     5266 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_find.json
--rw-r--r--   0        0        0      831 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_labels.json
--rw-r--r--   0        0        0     5638 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_modify.json
--rw-r--r--   0        0        0     1182 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arsinh.json
--rw-r--r--   0        0        0     1197 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/artanh.json
--rw-r--r--   0        0        0     2895 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/atmospheric_correction.json
--rw-r--r--   0        0        0     6511 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/between.json
--rw-r--r--   0        0        0     1402 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/ceil.json
--rw-r--r--   0        0        0     2811 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/clip.json
--rw-r--r--   0        0        0      585 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/constant.json
--rw-r--r--   0        0        0     1038 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/cos.json
--rw-r--r--   0        0        0     1093 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/cosh.json
--rw-r--r--   0        0        0     5028 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/count.json
--rw-r--r--   0        0        0      685 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/create_raster_cube.json
--rw-r--r--   0        0        0     1220 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/dimension_labels.json
--rw-r--r--   0        0        0     2235 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/divide.json
--rw-r--r--   0        0        0     1672 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/drop_dimension.json
--rw-r--r--   0        0        0      713 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/e.json
--rw-r--r--   0        0        0     5450 2023-05-19 11:47:02.787789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/eq.json
--rw-r--r--   0        0        0     1652 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/examples/array_contains_nodata.json
--rw-r--r--   0        0        0     1810 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/examples/array_find_nodata.json
--rw-r--r--   0        0        0     1728 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/examples/rename-enumerated-labels.json
--rw-r--r--   0        0        0     1672 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/exp.json
--rw-r--r--   0        0        0     3089 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/extrema.json
--rw-r--r--   0        0        0     3536 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/filter_bands.json
--rw-r--r--   0        0        0     4600 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/filter_labels.json
--rw-r--r--   0        0        0     4069 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/filter_temporal.json
--rw-r--r--   0        0        0     2047 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/first.json
--rw-r--r--   0        0        0     3985 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/fit_regr_random_forest.json
--rw-r--r--   0        0        0     1574 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/floor.json
--rw-r--r--   0        0        0     2645 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/gt.json
--rw-r--r--   0        0        0     3797 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/gte.json
--rw-r--r--   0        0        0     2521 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/if.json
--rw-r--r--   0        0        0     1569 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/int.json
--rw-r--r--   0        0        0     1132 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/is_infinite.json
--rw-r--r--   0        0        0     1646 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/is_nan.json
--rw-r--r--   0        0        0     1398 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/is_nodata.json
--rw-r--r--   0        0        0     1760 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/is_valid.json
--rw-r--r--   0        0        0     2042 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/last.json
--rw-r--r--   0        0        0     5011 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/linear_scale_range.json
--rw-r--r--   0        0        0     2111 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/ln.json
--rw-r--r--   0        0        0    16038 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/load_collection.json
--rw-r--r--   0        0        0     1956 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/load_ml_model.json
--rw-r--r--   0        0        0     1477 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/load_vector_cube.json
--rw-r--r--   0        0        0     2322 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/log.json
--rw-r--r--   0        0        0     2634 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/lt.json
--rw-r--r--   0        0        0     3787 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/lte.json
--rw-r--r--   0        0        0     2476 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/max.json
--rw-r--r--   0        0        0     4412 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/mean.json
--rw-r--r--   0        0        0     4029 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/median.json
--rw-r--r--   0        0        0     6712 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/merge_cubes.json
--rw-r--r--   0        0        0    11001 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/meta/implementation.md
--rw-r--r--   0        0        0    19134 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/meta/subtype-schemas.json
--rw-r--r--   0        0        0     2408 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/min.json
--rw-r--r--   0        0        0     4358 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/anomaly.json
--rw-r--r--   0        0        0     4833 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_kernel.json
--rw-r--r--   0        0        0    11277 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_neighborhood.json
--rw-r--r--   0        0        0     4087 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/array_apply.json
--rw-r--r--   0        0        0     3970 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/climatological_normal.json
--rw-r--r--   0        0        0     5205 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_bbox.json
--rw-r--r--   0        0        0     2123 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_spatial.json
--rw-r--r--   0        0        0     2194 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/mask.json
--rw-r--r--   0        0        0     2948 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/mask_polygon.json
--rw-r--r--   0        0        0     1633 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_dimension.json
--rw-r--r--   0        0        0     4437 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_labels.json
--rw-r--r--   0        0        0     6869 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/resample_spatial.json
--rw-r--r--   0        0        0     3908 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/run_udf.json
--rw-r--r--   0        0        0     2605 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/text_begins.json
--rw-r--r--   0        0        0     2573 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/text_contains.json
--rw-r--r--   0        0        0     2579 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/text_ends.json
--rw-r--r--   0        0        0     2863 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/text_merge.json
--rw-r--r--   0        0        0      883 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/trim_cube.json
--rw-r--r--   0        0        0     2634 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/mod.json
--rw-r--r--   0        0        0     2564 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/multiply.json
--rw-r--r--   0        0        0      879 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/nan.json
--rw-r--r--   0        0        0     5428 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/ndvi.json
--rw-r--r--   0        0        0     6037 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/neq.json
--rw-r--r--   0        0        0     2566 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/normalized_difference.json
--rw-r--r--   0        0        0     1111 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/not.json
--rw-r--r--   0        0        0     2368 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/or.json
--rw-r--r--   0        0        0     5506 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/order.json
--rw-r--r--   0        0        0      686 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/pi.json
--rw-r--r--   0        0        0     2278 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/power.json
--rw-r--r--   0        0        0     1988 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/predict_random_forest.json
--rw-r--r--   0        0        0     3035 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/product.json
--rw-r--r--   0        0        0     5560 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/aggregate_spatial_window.json
--rw-r--r--   0        0        0     5380 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/ard_normalized_radar_backscatter.json
--rw-r--r--   0        0        0     6009 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/ard_surface_reflectance.json
--rw-r--r--   0        0        0     1702 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/array_append.json
--rw-r--r--   0        0        0     1601 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/array_create_labeled.json
--rw-r--r--   0        0        0     1454 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/array_find_label.json
--rw-r--r--   0        0        0     2405 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/array_interpolate_linear.json
--rw-r--r--   0        0        0     2895 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/atmospheric_correction.json
--rw-r--r--   0        0        0     2892 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/cloud_detection.json
--rw-r--r--   0        0        0     2814 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/cummax.json
--rw-r--r--   0        0        0     2815 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/cummin.json
--rw-r--r--   0        0        0     2888 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/cumproduct.json
--rw-r--r--   0        0        0     2777 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/cumsum.json
--rw-r--r--   0        0        0     5608 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/date_shift.json
--rw-r--r--   0        0        0     4600 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/filter_labels.json
--rw-r--r--   0        0        0     3769 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/fit_curve.json
--rw-r--r--   0        0        0     2214 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/inspect.json
--rw-r--r--   0        0        0     1132 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/is_infinite.json
--rw-r--r--   0        0        0    11705 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/load_result.json
--rw-r--r--   0        0        0     2292 2023-05-19 11:47:02.791789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/load_uploaded_files.json
--rw-r--r--   0        0        0     4138 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/predict_curve.json
--rw-r--r--   0        0        0     4000 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/resample_cube_temporal.json
--rw-r--r--   0        0        0     2624 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/run_udf_externally.json
--rw-r--r--   0        0        0     5986 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/sar_backscatter.json
--rw-r--r--   0        0        0     5910 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/quantiles.json
--rw-r--r--   0        0        0     2703 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/rearrange.json
--rw-r--r--   0        0        0     3483 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/reduce_dimension.json
--rw-r--r--   0        0        0     3402 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/reduce_spatial.json
--rw-r--r--   0        0        0     3425 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/resample_cube_spatial.json
--rw-r--r--   0        0        0     2759 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/round.json
--rw-r--r--   0        0        0     5986 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sar_backscatter.json
--rw-r--r--   0        0        0     1181 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/save_ml_model.json
--rw-r--r--   0        0        0     2928 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/save_result.json
--rw-r--r--   0        0        0     1094 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/save_vector_cube.json
--rw-r--r--   0        0        0     3086 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sd.json
--rw-r--r--   0        0        0     9529 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sen2like.json
--rw-r--r--   0        0        0     2503 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sgn.json
--rw-r--r--   0        0        0     1028 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sin.json
--rw-r--r--   0        0        0     1083 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sinh.json
--rw-r--r--   0        0        0     5177 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sort.json
--rw-r--r--   0        0        0     1891 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sqrt.json
--rw-r--r--   0        0        0     1975 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/subtract.json
--rw-r--r--   0        0        0     3008 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sum.json
--rw-r--r--   0        0        0     1114 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tan.json
--rw-r--r--   0        0        0     1191 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tanh.json
--rw-r--r--   0        0        0       50 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/.gitignore
--rw-r--r--   0        0        0      371 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/.words
--rw-r--r--   0        0        0     2075 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/README.md
--rw-r--r--   0        0        0     3396 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/docs.html
--rw-r--r--   0        0        0     1977 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/examples.test.js
--rw-r--r--   0        0        0     1013 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/package.json
--rw-r--r--   0        0        0     8960 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/processes.test.js
--rw-r--r--   0        0        0     1021 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/subtypes-file.test.js
--rw-r--r--   0        0        0     1929 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/subtypes-schemas.test.js
--rw-r--r--   0        0        0     4776 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/testHelpers.js
--rw-r--r--   0        0        0     4488 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/variance.json
--rw-r--r--   0        0        0     3119 2023-05-19 11:47:02.795789 openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/xor.json
--rw-r--r--   0        0        0     2009 2023-05-19 11:47:02.051792 openeo_processes_dask-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0     4863 1970-01-01 00:00:00.000000 openeo_processes_dask-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/LICENSE
+-rw-r--r--   0        0        0     3067 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/README.md
+-rw-r--r--   0        0        0       25 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/__init__.py
+-rw-r--r--   0        0        0      801 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/__init__.py
+-rw-r--r--   0        0        0    10187 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/arrays.py
+-rw-r--r--   0        0        0     2997 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/comparison.py
+-rw-r--r--   0        0        0     3980 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/core.py
+-rw-r--r--   0        0        0      155 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/__init__.py
+-rw-r--r--   0        0        0     6991 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/_filter.py
+-rw-r--r--   0        0        0     3900 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/_xr_interop.py
+-rw-r--r--   0        0        0     3820 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/aggregate.py
+-rw-r--r--   0        0        0     2417 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/apply.py
+-rw-r--r--   0        0        0     2617 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/experimental.py
+-rw-r--r--   0        0        0     2173 2023-07-13 07:15:27.418894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/general.py
+-rw-r--r--   0        0        0     5989 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/load.py
+-rw-r--r--   0        0        0    10376 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/merge.py
+-rw-r--r--   0        0        0     1814 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/reduce.py
+-rw-r--r--   0        0        0      443 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/utils.py
+-rw-r--r--   0        0        0      221 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/data_model.py
+-rw-r--r--   0        0        0      974 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/exceptions.py
+-rw-r--r--   0        0        0       24 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/experimental/__init__.py
+-rw-r--r--   0        0        0     2545 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/experimental/resample.py
+-rw-r--r--   0        0        0     2317 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/logic.py
+-rw-r--r--   0        0        0     7821 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/math.py
+-rw-r--r--   0        0        0       29 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/ml/__init__.py
+-rw-r--r--   0        0        0     2846 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/ml/random_forest.py
+-rw-r--r--   0        0        0      233 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/utils.py
+-rw-r--r--   0        0        0      892 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/__init__.py
+-rw-r--r--   0        0        0       75 2023-07-13 07:15:28.066896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/.git
+-rw-r--r--   0        0        0       27 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      445 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/issue-or-clarification-for-existing-process.md
+-rw-r--r--   0        0        0      856 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-parameter.md
+-rw-r--r--   0        0        0     1516 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-proposal.md
+-rw-r--r--   0        0        0      167 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/other.md
+-rw-r--r--   0        0        0     1953 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      329 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    19276 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/LICENSE
+-rw-r--r--   0        0        0     4577 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/README.md
+-rw-r--r--   0        0        0     2325 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/absolute.json
+-rw-r--r--   0        0        0     2390 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/add.json
+-rw-r--r--   0        0        0     1981 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/add_dimension.json
+-rw-r--r--   0        0        0     6149 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/aggregate_spatial.json
+-rw-r--r--   0        0        0    10450 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/aggregate_temporal.json
+-rw-r--r--   0        0        0     7320 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/aggregate_temporal_period.json
+-rw-r--r--   0        0        0     3799 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/all.json
+-rw-r--r--   0        0        0     2371 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/and.json
+-rw-r--r--   0        0        0     3768 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/any.json
+-rw-r--r--   0        0        0     2737 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/apply.json
+-rw-r--r--   0        0        0     6430 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/apply_dimension.json
+-rw-r--r--   0        0        0     1145 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arccos.json
+-rw-r--r--   0        0        0     1192 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arcosh.json
+-rw-r--r--   0        0        0     1133 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arcsin.json
+-rw-r--r--   0        0        0     1151 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arctan.json
+-rw-r--r--   0        0        0     1720 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arctan2.json
+-rw-r--r--   0        0        0     5380 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/ard_normalized_radar_backscatter.json
+-rw-r--r--   0        0        0     6009 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/ard_surface_reflectance.json
+-rw-r--r--   0        0        0     1591 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_concat.json
+-rw-r--r--   0        0        0     4992 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_contains.json
+-rw-r--r--   0        0        0     2619 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_create.json
+-rw-r--r--   0        0        0     3377 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_element.json
+-rw-r--r--   0        0        0     3594 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_filter.json
+-rw-r--r--   0        0        0     5266 2023-07-13 07:15:28.074896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_find.json
+-rw-r--r--   0        0        0      831 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_labels.json
+-rw-r--r--   0        0        0     5638 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_modify.json
+-rw-r--r--   0        0        0     1182 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arsinh.json
+-rw-r--r--   0        0        0     1197 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/artanh.json
+-rw-r--r--   0        0        0     2895 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/atmospheric_correction.json
+-rw-r--r--   0        0        0     6511 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/between.json
+-rw-r--r--   0        0        0     1402 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/ceil.json
+-rw-r--r--   0        0        0     2811 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/clip.json
+-rw-r--r--   0        0        0      585 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/constant.json
+-rw-r--r--   0        0        0     1038 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/cos.json
+-rw-r--r--   0        0        0     1093 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/cosh.json
+-rw-r--r--   0        0        0     5028 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/count.json
+-rw-r--r--   0        0        0      685 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/create_raster_cube.json
+-rw-r--r--   0        0        0     1220 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/dimension_labels.json
+-rw-r--r--   0        0        0     2235 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/divide.json
+-rw-r--r--   0        0        0     1672 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/drop_dimension.json
+-rw-r--r--   0        0        0      713 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/e.json
+-rw-r--r--   0        0        0     5450 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/eq.json
+-rw-r--r--   0        0        0     1652 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/examples/array_contains_nodata.json
+-rw-r--r--   0        0        0     1810 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/examples/array_find_nodata.json
+-rw-r--r--   0        0        0     1728 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/examples/rename-enumerated-labels.json
+-rw-r--r--   0        0        0     1672 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/exp.json
+-rw-r--r--   0        0        0     3089 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/extrema.json
+-rw-r--r--   0        0        0     3536 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/filter_bands.json
+-rw-r--r--   0        0        0     4600 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/filter_labels.json
+-rw-r--r--   0        0        0     4069 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/filter_temporal.json
+-rw-r--r--   0        0        0     2047 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/first.json
+-rw-r--r--   0        0        0     3985 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/fit_regr_random_forest.json
+-rw-r--r--   0        0        0     1574 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/floor.json
+-rw-r--r--   0        0        0     2645 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/gt.json
+-rw-r--r--   0        0        0     3797 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/gte.json
+-rw-r--r--   0        0        0     2521 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/if.json
+-rw-r--r--   0        0        0     1569 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/int.json
+-rw-r--r--   0        0        0     1132 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/is_infinite.json
+-rw-r--r--   0        0        0     1646 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/is_nan.json
+-rw-r--r--   0        0        0     1398 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/is_nodata.json
+-rw-r--r--   0        0        0     1760 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/is_valid.json
+-rw-r--r--   0        0        0     2042 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/last.json
+-rw-r--r--   0        0        0     5011 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/linear_scale_range.json
+-rw-r--r--   0        0        0     2111 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/ln.json
+-rw-r--r--   0        0        0    16038 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/load_collection.json
+-rw-r--r--   0        0        0     1956 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/load_ml_model.json
+-rw-r--r--   0        0        0    17030 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/load_stac.json
+-rw-r--r--   0        0        0     1477 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/load_vector_cube.json
+-rw-r--r--   0        0        0     2322 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/log.json
+-rw-r--r--   0        0        0     2634 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/lt.json
+-rw-r--r--   0        0        0     3787 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/lte.json
+-rw-r--r--   0        0        0     2476 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/max.json
+-rw-r--r--   0        0        0     4412 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/mean.json
+-rw-r--r--   0        0        0     4029 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/median.json
+-rw-r--r--   0        0        0     6712 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/merge_cubes.json
+-rw-r--r--   0        0        0    11001 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/meta/implementation.md
+-rw-r--r--   0        0        0    19134 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/meta/subtype-schemas.json
+-rw-r--r--   0        0        0     2408 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/min.json
+-rw-r--r--   0        0        0     4358 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/anomaly.json
+-rw-r--r--   0        0        0     4833 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_kernel.json
+-rw-r--r--   0        0        0    11277 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_neighborhood.json
+-rw-r--r--   0        0        0     4087 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/array_apply.json
+-rw-r--r--   0        0        0     3970 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/climatological_normal.json
+-rw-r--r--   0        0        0     5205 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_bbox.json
+-rw-r--r--   0        0        0     2123 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_spatial.json
+-rw-r--r--   0        0        0     2194 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/mask.json
+-rw-r--r--   0        0        0     2948 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/mask_polygon.json
+-rw-r--r--   0        0        0     1633 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_dimension.json
+-rw-r--r--   0        0        0     4437 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_labels.json
+-rw-r--r--   0        0        0     6869 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/resample_spatial.json
+-rw-r--r--   0        0        0     3908 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/run_udf.json
+-rw-r--r--   0        0        0     2605 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/text_begins.json
+-rw-r--r--   0        0        0     2573 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/text_contains.json
+-rw-r--r--   0        0        0     2579 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/text_ends.json
+-rw-r--r--   0        0        0     2863 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/text_merge.json
+-rw-r--r--   0        0        0      883 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/trim_cube.json
+-rw-r--r--   0        0        0     2634 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/mod.json
+-rw-r--r--   0        0        0     2564 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/multiply.json
+-rw-r--r--   0        0        0      879 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/nan.json
+-rw-r--r--   0        0        0     5428 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/ndvi.json
+-rw-r--r--   0        0        0     6037 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/neq.json
+-rw-r--r--   0        0        0     2566 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/normalized_difference.json
+-rw-r--r--   0        0        0     1111 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/not.json
+-rw-r--r--   0        0        0     2368 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/or.json
+-rw-r--r--   0        0        0     5506 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/order.json
+-rw-r--r--   0        0        0      686 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/pi.json
+-rw-r--r--   0        0        0     2278 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/power.json
+-rw-r--r--   0        0        0     1988 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/predict_random_forest.json
+-rw-r--r--   0        0        0     3035 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/product.json
+-rw-r--r--   0        0        0     5560 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/aggregate_spatial_window.json
+-rw-r--r--   0        0        0     5380 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/ard_normalized_radar_backscatter.json
+-rw-r--r--   0        0        0     6009 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/ard_surface_reflectance.json
+-rw-r--r--   0        0        0     1702 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/array_append.json
+-rw-r--r--   0        0        0     1601 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/array_create_labeled.json
+-rw-r--r--   0        0        0     1454 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/array_find_label.json
+-rw-r--r--   0        0        0     2405 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/array_interpolate_linear.json
+-rw-r--r--   0        0        0     2895 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/atmospheric_correction.json
+-rw-r--r--   0        0        0     2892 2023-07-13 07:15:28.078896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/cloud_detection.json
+-rw-r--r--   0        0        0     2814 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/cummax.json
+-rw-r--r--   0        0        0     2815 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/cummin.json
+-rw-r--r--   0        0        0     2888 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/cumproduct.json
+-rw-r--r--   0        0        0     2777 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/cumsum.json
+-rw-r--r--   0        0        0     5608 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/date_shift.json
+-rw-r--r--   0        0        0     4600 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/filter_labels.json
+-rw-r--r--   0        0        0     3769 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/fit_curve.json
+-rw-r--r--   0        0        0     2214 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/inspect.json
+-rw-r--r--   0        0        0     1132 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/is_infinite.json
+-rw-r--r--   0        0        0    11705 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/load_result.json
+-rw-r--r--   0        0        0     2292 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/load_uploaded_files.json
+-rw-r--r--   0        0        0     4138 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/predict_curve.json
+-rw-r--r--   0        0        0     4000 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/resample_cube_temporal.json
+-rw-r--r--   0        0        0     2624 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/run_udf_externally.json
+-rw-r--r--   0        0        0     5986 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/sar_backscatter.json
+-rw-r--r--   0        0        0     5910 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/quantiles.json
+-rw-r--r--   0        0        0     2703 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/rearrange.json
+-rw-r--r--   0        0        0     3483 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/reduce_dimension.json
+-rw-r--r--   0        0        0     3402 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/reduce_spatial.json
+-rw-r--r--   0        0        0     3425 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/resample_cube_spatial.json
+-rw-r--r--   0        0        0     2759 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/round.json
+-rw-r--r--   0        0        0     5986 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sar_backscatter.json
+-rw-r--r--   0        0        0     1181 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/save_ml_model.json
+-rw-r--r--   0        0        0     2928 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/save_result.json
+-rw-r--r--   0        0        0     1094 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/save_vector_cube.json
+-rw-r--r--   0        0        0     3086 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sd.json
+-rw-r--r--   0        0        0     9529 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sen2like.json
+-rw-r--r--   0        0        0     2503 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sgn.json
+-rw-r--r--   0        0        0     1028 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sin.json
+-rw-r--r--   0        0        0     1083 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sinh.json
+-rw-r--r--   0        0        0     5177 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sort.json
+-rw-r--r--   0        0        0     1891 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sqrt.json
+-rw-r--r--   0        0        0     1975 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/subtract.json
+-rw-r--r--   0        0        0     3008 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sum.json
+-rw-r--r--   0        0        0     1114 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tan.json
+-rw-r--r--   0        0        0     1191 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tanh.json
+-rw-r--r--   0        0        0       50 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/.gitignore
+-rw-r--r--   0        0        0      371 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/.words
+-rw-r--r--   0        0        0     2075 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/README.md
+-rw-r--r--   0        0        0     3396 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/docs.html
+-rw-r--r--   0        0        0     1977 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/examples.test.js
+-rw-r--r--   0        0        0     1013 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/package.json
+-rw-r--r--   0        0        0     8960 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/processes.test.js
+-rw-r--r--   0        0        0     1021 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/subtypes-file.test.js
+-rw-r--r--   0        0        0     1929 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/subtypes-schemas.test.js
+-rw-r--r--   0        0        0     4776 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/testHelpers.js
+-rw-r--r--   0        0        0     4488 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/variance.json
+-rw-r--r--   0        0        0     3119 2023-07-13 07:15:28.082896 openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/xor.json
+-rw-r--r--   0        0        0     2309 2023-07-13 07:15:27.422894 openeo_processes_dask-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4988 1970-01-01 00:00:00.000000 openeo_processes_dask-2023.7.0/PKG-INFO
```

### Comparing `openeo_processes_dask-2023.5.1/LICENSE` & `openeo_processes_dask-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/README.md` & `openeo_processes_dask-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/__init__.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 logger = logging.getLogger(__name__)
 
-
 from .arrays import *
 from .comparison import *
 from .cubes import *
+from .logic import *
 from .math import *
 
 try:
     from .ml import *
 except ImportError as e:
     logger.warning(
         "Did not load machine learning processes due to missing dependencies: Install them like this: `pip install openeo-processes-dask[implementations, ml]`"
```

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/arrays.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/arrays.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/comparison.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/comparison.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/core.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,18 +70,19 @@
 
         special_args = ["axis", "keepdims", "source_transposed_axis"]
         # Remove 'axis' and keepdims parameter if not expected in function signature.
         for arg in special_args:
             if arg not in inspect.signature(f).parameters:
                 resolved_kwargs.pop(arg, None)
 
-        pretty_args = {k: type(v) for k, v in resolved_kwargs.items()}
-        logger.warning(f"Running process {f.__name__}")
-        logger.warning(f"kwargs: {pretty_args}")
-        logger.warning("-" * 80)
+        pretty_args = {k: repr(v)[:80] for k, v in resolved_kwargs.items()}
+        logger.info(f"Running process {f.__name__}")
+        logger.debug(
+            f"Running process {f.__name__} with resolved parameters: {pretty_args}"
+        )
 
         return f(*resolved_args, **resolved_kwargs)
 
     return wrapper
 
 
 # This is not cool in most Python code, but I think it's fine here. It allows us to import and register new functions by just upgrading
```

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/_filter.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/aggregate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,90 +1,119 @@
-import logging
-from typing import Callable
+from typing import Callable, Optional, Union
 
-import numpy as np
-from openeo_pg_parser_networkx.pg_schema import TemporalInterval
+import rasterio
+from openeo_pg_parser_networkx.pg_schema import TemporalInterval, TemporalIntervals
 
-from openeo_processes_dask.process_implementations.data_model import RasterCube
+from openeo_processes_dask.process_implementations.data_model import (
+    RasterCube,
+    VectorCube,
+)
 from openeo_processes_dask.process_implementations.exceptions import (
-    BandFilterParameterMissing,
-    DimensionMissing,
     DimensionNotAvailable,
     TooManyDimensions,
 )
 
-logger = logging.getLogger(__name__)
-
-__all__ = ["filter_labels", "filter_temporal", "filter_bands"]
+__all__ = ["aggregate_temporal", "aggregate_temporal_period", "aggregate_spatial"]
 
 
-def filter_temporal(
-    data: RasterCube, extent: TemporalInterval, dimension: str = None
+def geometry_mask(geoms, geobox, all_touched=False, invert=False):
+    return rasterio.features.geometry_mask(
+        [geom.to_crs(geobox.crs) for geom in geoms],
+        out_shape=geobox.shape,
+        transform=geobox.affine,
+        all_touched=all_touched,
+        invert=invert,
+    )
+
+
+def aggregate_temporal(
+    data: RasterCube,
+    intervals: Union[TemporalIntervals, list[TemporalInterval], list[Optional[str]]],
+    reducer: Callable,
+    labels: Optional[list] = None,
+    dimension: Optional[str] = None,
+    context: Optional[dict] = None,
+    **kwargs,
 ) -> RasterCube:
     temporal_dims = data.openeo.temporal_dims
 
     if dimension is not None:
         if dimension not in data.dims:
             raise DimensionNotAvailable(
                 f"A dimension with the specified name: {dimension} does not exist."
             )
         applicable_temporal_dimension = dimension
-        if dimension not in temporal_dims:
-            logger.warning(
-                f"The selected dimension {dimension} exists but it is not labeled as a temporal dimension. Available temporal diemnsions are {temporal_dims}."
-            )
     else:
         if not temporal_dims:
             raise DimensionNotAvailable(
                 f"No temporal dimension detected on dataset. Available dimensions: {data.dims}"
             )
         if len(temporal_dims) > 1:
             raise TooManyDimensions(
                 f"The data cube contains multiple temporal dimensions: {temporal_dims}. The parameter `dimension` must be specified."
             )
-    applicable_temporal_dimension = temporal_dims[0]
+        applicable_temporal_dimension = temporal_dims[0]
 
-    start_time = extent[0]
-    if start_time is not None:
-        start_time = start_time.to_numpy()
-    end_time = extent[1]
-    if end_time is not None:
-        end_time = extent[1].to_numpy() - np.timedelta64(1, "ms")
-    # The second element is the end of the temporal interval.
-    # The specified instance in time is excluded from the interval.
-    # See https://processes.openeo.org/#filter_temporal
-
-    filtered = data.loc[{applicable_temporal_dimension: slice(start_time, end_time)}]
-
-    return filtered
-
-
-def filter_labels(data: RasterCube, condition: Callable, dimension: str) -> RasterCube:
-    if dimension not in data.dims:
-        raise DimensionNotAvailable(
-            f"Provided dimension ({dimension}) not found in data.dims: {data.dims}"
-        )
+    aggregated_data = data.groupby_bins(
+        group=applicable_temporal_dimension, labels=labels
+    )
 
-    labels = data[dimension].values
-    label_mask = condition(x=labels)
-    label = labels[label_mask]
-    data = data.sel(**{dimension: label})
-    return data
+    raise NotImplementedError("aggregate_temporal is currently not implemented")
 
 
-def filter_bands(data: RasterCube, bands: list[str] = None) -> RasterCube:
-    if bands is None:
-        raise BandFilterParameterMissing(
-            "The process `filter_bands` requires the parameters `bands` to be set."
-        )
+def aggregate_temporal_period(
+    data: RasterCube,
+    reducer: Callable,
+    period: str,
+    dimension: Optional[str] = None,
+) -> RasterCube:
+    temporal_dims = data.openeo.temporal_dims
 
-    if len(data.openeo.band_dims) < 1:
-        raise DimensionMissing("A band dimension is missing.")
-    band_dim = data.openeo.band_dims[0]
-
-    try:
-        data = data.sel(**{band_dim: bands})
-    except Exception as e:
-        raise Exception(
-            f"The provided bands: {bands} are not all available in the datacube. Please modify the bands parameter of filter_bands and choose among: {data[band_dim].values}."
+    if dimension is not None:
+        if dimension not in data.dims:
+            raise DimensionNotAvailable(
+                f"A dimension with the specified name: {dimension} does not exist."
+            )
+        applicable_temporal_dimension = dimension
+    else:
+        if not temporal_dims:
+            raise DimensionNotAvailable(
+                f"No temporal dimension detected on dataset. Available dimensions: {data.dims}"
+            )
+        if len(temporal_dims) > 1:
+            raise TooManyDimensions(
+                f"The data cube contains multiple temporal dimensions: {temporal_dims}. The parameter `dimension` must be specified."
+            )
+        applicable_temporal_dimension = temporal_dims[0]
+
+    periods_to_frequency = {
+        "hour": "H",
+        "day": "D",
+        "week": "W",
+        "month": "M",
+        "season": "QS-DEC",
+        "year": "AS",
+    }
+
+    if period in periods_to_frequency.keys():
+        frequency = periods_to_frequency[period]
+    else:
+        raise NotImplementedError(
+            f"The provided period '{period})' is not implemented yet. The available ones are {list(periods_to_frequency.keys())}."
         )
-    return data
+
+    resampled_data = data.resample({applicable_temporal_dimension: frequency})
+
+    positional_parameters = {"data": 0}
+    return resampled_data.reduce(
+        reducer, keep_attrs=True, positional_parameters=positional_parameters
+    )
+
+
+def aggregate_spatial(
+    data: RasterCube,
+    geometries: VectorCube,
+    reducer: Callable,
+    target_dimension: str = "result",
+    **kwargs,
+) -> VectorCube:
+    raise NotImplementedError
```

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/apply.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/apply.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         context = {}
 
     if dimension not in data.dims:
         raise DimensionNotAvailable(
             f"Provided dimension ({dimension}) not found in data.dims: {data.dims}"
         )
 
+    is_new_dim_added = target_dimension is not None
+
     if target_dimension is None:
         target_dimension = dimension
 
     positional_parameters = {"data": 0}
     named_parameters = {"context": context}
 
     # This transpose (and back later) is needed because apply_ufunc automatically moves
@@ -72,8 +74,11 @@
     reordered_result = result.transpose(*data.dims, ...).rename(
         {dimension: target_dimension}
     )
 
     if len(data[dimension]) == len(reordered_result[target_dimension]):
         reordered_result.rio.write_crs(data.rio.crs, inplace=True)
 
+    if is_new_dim_added:
+        reordered_result.openeo.add_dim_type(name=target_dimension, type="other")
+
     return reordered_result
```

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/experimental.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/experimental.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/general.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,9 +59,9 @@
     if name in data.dims:
         raise Exception(
             f"DimensionExists - A dimension with the specified name already exists. The existing dimensions are: {data.dims}"
         )
     data_e = data.assign_coords(**{name: label})
     data_e = data_e.expand_dims(name)
     # Register dimension in the openeo accessor
-    data_e.openeo.add_dim_to_guesses(name=name, type=type)
+    data_e.openeo.add_dim_type(name=name, type=type)
     return data_e
```

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/merge.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/merge.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/cubes/reduce.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/cubes/reduce.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/exceptions.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,7 +52,15 @@
 
 class DimensionMissing(OpenEOException):
     pass
 
 
 class BandFilterParameterMissing(OpenEOException):
     pass
+
+
+class NoDataAvailable(OpenEOException):
+    pass
+
+
+class TemporalExtentEmpty(OpenEOException):
+    pass
```

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/experimental/resample.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/experimental/resample.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/math.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/math.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/process_implementations/ml/random_forest.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/process_implementations/ml/random_forest.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/__init__.py` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-parameter.md` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-parameter.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-proposal.md` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-proposal.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/.github/workflows/docs.yml` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/CHANGELOG.md` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/LICENSE` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/LICENSE`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/README.md` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/README.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/absolute.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/absolute.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/add.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/add.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/add_dimension.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/add_dimension.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/aggregate_spatial.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/aggregate_spatial.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/aggregate_temporal.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/aggregate_temporal.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/aggregate_temporal_period.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/aggregate_temporal_period.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/all.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/all.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/and.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/and.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/any.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/any.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/apply.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/apply.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/apply_dimension.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/apply_dimension.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arccos.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arccos.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arcosh.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arcosh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arcsin.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arcsin.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arctan.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arctan.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arctan2.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arctan2.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/ard_normalized_radar_backscatter.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/ard_normalized_radar_backscatter.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/ard_surface_reflectance.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/ard_surface_reflectance.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_concat.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_concat.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_contains.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_contains.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_create.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_create.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_element.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_element.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_filter.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_filter.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_find.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_find.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_labels.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/array_modify.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/array_modify.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/arsinh.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/arsinh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/artanh.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/artanh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/atmospheric_correction.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/atmospheric_correction.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/between.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/between.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/ceil.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/ceil.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/clip.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/clip.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/constant.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/constant.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/cos.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/cos.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/cosh.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/cosh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/count.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/count.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/create_raster_cube.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/create_raster_cube.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/dimension_labels.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/dimension_labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/divide.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/divide.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/drop_dimension.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/drop_dimension.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/e.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/e.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/eq.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/eq.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/examples/array_contains_nodata.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/examples/array_contains_nodata.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/examples/array_find_nodata.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/examples/array_find_nodata.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/examples/rename-enumerated-labels.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/examples/rename-enumerated-labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/exp.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/exp.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/extrema.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/extrema.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/filter_bands.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/filter_bands.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/filter_labels.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/filter_labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/filter_temporal.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/filter_temporal.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/first.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/first.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/fit_regr_random_forest.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/fit_regr_random_forest.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/floor.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/floor.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/gt.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/gt.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/gte.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/gte.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/if.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/if.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/int.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/int.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/is_infinite.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/is_infinite.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/is_nan.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/is_nan.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/is_nodata.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/is_nodata.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/is_valid.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/is_valid.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/last.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/last.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/linear_scale_range.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/linear_scale_range.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/ln.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/ln.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/load_collection.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/load_collection.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/load_ml_model.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/load_ml_model.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/load_vector_cube.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/load_vector_cube.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/log.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/log.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/lt.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/lt.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/lte.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/lte.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/max.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/max.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/mean.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/mean.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/median.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/median.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/merge_cubes.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/merge_cubes.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/meta/implementation.md` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/meta/implementation.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/meta/subtype-schemas.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/meta/subtype-schemas.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/min.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/min.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/anomaly.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/anomaly.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_kernel.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_kernel.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_neighborhood.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_neighborhood.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/array_apply.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/array_apply.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/climatological_normal.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/climatological_normal.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_bbox.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_bbox.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_spatial.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_spatial.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/mask.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/mask.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/mask_polygon.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/mask_polygon.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_dimension.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_dimension.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_labels.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/resample_spatial.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/resample_spatial.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/run_udf.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/run_udf.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/text_begins.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/text_begins.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/text_contains.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/text_contains.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/text_ends.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/text_ends.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/text_merge.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/text_merge.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/missing-processes/trim_cube.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/missing-processes/trim_cube.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/mod.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/mod.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/multiply.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/multiply.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/nan.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/nan.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/ndvi.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/ndvi.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/neq.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/neq.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/normalized_difference.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/normalized_difference.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/not.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/not.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/or.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/or.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/order.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/order.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/pi.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/pi.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/power.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/power.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/predict_random_forest.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/predict_random_forest.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/product.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/product.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/aggregate_spatial_window.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/aggregate_spatial_window.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/ard_normalized_radar_backscatter.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/ard_normalized_radar_backscatter.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/ard_surface_reflectance.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/ard_surface_reflectance.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/array_append.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/array_append.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/array_create_labeled.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/array_create_labeled.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/array_find_label.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/array_find_label.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/array_interpolate_linear.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/array_interpolate_linear.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/atmospheric_correction.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/atmospheric_correction.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/cloud_detection.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/cloud_detection.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/cummax.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/cummax.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/cummin.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/cummin.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/cumproduct.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/cumproduct.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/cumsum.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/cumsum.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/date_shift.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/date_shift.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/filter_labels.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/filter_labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/fit_curve.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/fit_curve.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/inspect.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/inspect.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/is_infinite.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/is_infinite.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/load_result.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/load_result.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/load_uploaded_files.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/load_uploaded_files.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/predict_curve.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/predict_curve.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/resample_cube_temporal.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/resample_cube_temporal.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/run_udf_externally.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/run_udf_externally.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/proposals/sar_backscatter.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/proposals/sar_backscatter.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/quantiles.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/quantiles.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/rearrange.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/rearrange.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/reduce_dimension.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/reduce_dimension.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/reduce_spatial.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/reduce_spatial.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/resample_cube_spatial.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/resample_cube_spatial.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/round.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/round.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sar_backscatter.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sar_backscatter.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/save_ml_model.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/save_ml_model.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/save_result.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/save_result.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/save_vector_cube.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/save_vector_cube.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sd.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sd.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sen2like.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sen2like.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sgn.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sgn.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sin.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sin.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sinh.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sinh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sort.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sort.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sqrt.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sqrt.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/subtract.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/subtract.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/sum.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/sum.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tan.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tan.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tanh.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tanh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/README.md` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/README.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/docs.html` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/docs.html`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/examples.test.js` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/examples.test.js`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/package.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/package.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/processes.test.js` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/processes.test.js`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/subtypes-file.test.js` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/subtypes-file.test.js`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/subtypes-schemas.test.js` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/subtypes-schemas.test.js`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/tests/testHelpers.js` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/tests/testHelpers.js`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/variance.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/variance.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/openeo_processes_dask/specs/openeo-processes/xor.json` & `openeo_processes_dask-2023.7.0/openeo_processes_dask/specs/openeo-processes/xor.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2023.5.1/pyproject.toml` & `openeo_processes_dask-2023.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openeo-processes-dask"
-version = "2023.5.1"
+version = "2023.7.0"
 description = "Python implementations of many OpenEO processes, dask-friendly by default."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/Open-EO/openeo-processes-dask"
 classifiers = [
@@ -29,27 +29,31 @@
 rasterio = { version = "^1.3.4", optional = true }
 dask-geopandas = { version = ">=0.2.0,<1", optional = true }
 xgboost = { version = "^1.5.1", optional = true }
 rioxarray = { version = ">=0.12.0,<1", optional = true }
 odc-algo = { version = "==0.2.3", optional = true }
 openeo-pg-parser-networkx = { version = ">=2023.5.1", optional = true }
 odc-geo = { version = "^0.3.2", optional = true }
+stac_validator = { version = ">=3.3.1", optional = true }
+stackstac = { version = ">=0.4.3", optional = true }
+pystac_client = { version = ">=0.6.1", optional = true }
+planetary_computer = { version = ">=0.5.1", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 ipykernel = "^6.15.1"
 matplotlib = "^3.5.3"
 folium = ">=0.12.1,<1"
 mapclassify = "^2.4.3"
 bokeh = "<3"
 pre-commit = "^2.20.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.extras]
-implementations = ["geopandas", "xarray", "dask", "rasterio", "dask-geopandas", "rioxarray", "openeo-pg-parser-networkx", "odc-geo"]
+implementations = ["geopandas", "xarray", "dask", "rasterio", "dask-geopandas", "rioxarray", "openeo-pg-parser-networkx", "odc-geo", "stackstac", "planetary_computer", "pystac_client", "stac_validator"]
 experimental = ["odc-algo"]
 ml = ["xgboost"]
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
```

### Comparing `openeo_processes_dask-2023.5.1/PKG-INFO` & `openeo_processes_dask-2023.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openeo-processes-dask
-Version: 2023.5.1
+Version: 2023.7.0
 Summary: Python implementations of many OpenEO processes, dask-friendly by default.
 Home-page: https://github.com/Open-EO/openeo-processes-dask
 License: Apache 2.0
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
@@ -12,29 +12,30 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: experimental
 Provides-Extra: implementations
 Provides-Extra: ml
 Requires-Dist: dask-geopandas (>=0.2.0,<1) ; extra == "implementations"
 Requires-Dist: dask[array] (>=2022.11.1) ; extra == "implementations"
 Requires-Dist: geopandas (>=0.11.1,<1) ; extra == "implementations"
 Requires-Dist: odc-algo (==0.2.3) ; extra == "experimental"
 Requires-Dist: odc-geo (>=0.3.2,<0.4.0) ; extra == "implementations"
 Requires-Dist: openeo-pg-parser-networkx (>=2023.5.1) ; extra == "implementations"
+Requires-Dist: planetary_computer (>=0.5.1) ; extra == "implementations"
+Requires-Dist: pystac_client (>=0.6.1) ; extra == "implementations"
 Requires-Dist: rasterio (>=1.3.4,<2.0.0) ; extra == "implementations"
 Requires-Dist: rioxarray (>=0.12.0,<1) ; extra == "implementations"
+Requires-Dist: stac_validator (>=3.3.1) ; extra == "implementations"
+Requires-Dist: stackstac (>=0.4.3) ; extra == "implementations"
 Requires-Dist: xarray (>=2022.11.0) ; extra == "implementations"
 Requires-Dist: xgboost (>=1.5.1,<2.0.0) ; extra == "ml"
 Project-URL: Repository, https://github.com/Open-EO/openeo-processes-dask
 Description-Content-Type: text/markdown
 
 # OpenEO Processes Dask
```


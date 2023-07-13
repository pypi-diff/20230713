# Comparing `tmp/cqlpy-0.2.7.tar.gz` & `tmp/cqlpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqlpy-0.2.7.tar", max compression
+gzip compressed data, was "cqlpy-0.3.0.tar", max compression
```

## Comparing `cqlpy-0.2.7.tar` & `cqlpy-0.3.0.tar`

### file list

```diff
@@ -1,95 +1,94 @@
--rw-r--r--   0        0        0     1070 2023-07-11 12:26:06.242231 cqlpy-0.2.7/LICENSE
--rw-r--r--   0        0        0        8 2023-07-11 12:26:06.242231 cqlpy-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-07-11 12:26:06.242231 cqlpy-0.2.7/cqlpy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 12:26:06.242231 cqlpy-0.2.7/cqlpy/_internal/__init__.py
--rw-r--r--   0        0        0     5335 2023-07-11 12:26:06.242231 cqlpy-0.2.7/cqlpy/_internal/context/context.py
--rw-r--r--   0        0        0     2077 2023-07-11 12:26:06.242231 cqlpy-0.2.7/cqlpy/_internal/context/cql_valueset_provider.py
--rw-r--r--   0        0        0      829 2023-07-11 12:26:06.242231 cqlpy-0.2.7/cqlpy/_internal/context/fhir/fhir_cql_type.py
--rw-r--r--   0        0        0  1023948 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/context/fhir/r4/map.py
--rw-r--r--   0        0        0    18950 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/context/fhir/r4/model.py
--rw-r--r--   0        0        0      689 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/context/parameter_provider.py
--rw-r--r--   0        0        0     3013 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/context/resource_query.py
--rw-r--r--   0        0        0     2532 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/context/type_factory.py
--rw-r--r--   0        0        0      143 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/exceptions.py
--rw-r--r--   0        0        0      123 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/aggregate/count.py
--rw-r--r--   0        0        0      339 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/arithmetic/max_value.py
--rw-r--r--   0        0        0      320 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/arithmetic/min_value.py
--rw-r--r--   0        0        0      688 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/clinical/any_in_valueset.py
--rw-r--r--   0        0        0     1041 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/clinical/in_valueset.py
--rw-r--r--   0        0        0      120 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/equal.py
--rw-r--r--   0        0        0      511 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/equivalent.py
--rw-r--r--   0        0        0      735 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/greater.py
--rw-r--r--   0        0        0      763 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/greater_or_equal.py
--rw-r--r--   0        0        0      507 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/in_list.py
--rw-r--r--   0        0        0      726 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/less.py
--rw-r--r--   0        0        0      753 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/less_or_equal.py
--rw-r--r--   0        0        0      741 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/comparison/not_equal.py
--rw-r--r--   0        0        0      671 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/cql_in.py
--rw-r--r--   0        0        0     1326 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/add.py
--rw-r--r--   0        0        0      541 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/after.py
--rw-r--r--   0        0        0      558 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/before.py
--rw-r--r--   0        0        0      588 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/calculate_age_at.py
--rw-r--r--   0        0        0      170 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/date_time_precision.py
--rw-r--r--   0        0        0      898 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/difference_between.py
--rw-r--r--   0        0        0      890 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/duration_between.py
--rw-r--r--   0        0        0      378 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/same_or_before.py
--rw-r--r--   0        0        0     1342 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/date_time/subtract.py
--rw-r--r--   0        0        0     3800 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/collapse.py
--rw-r--r--   0        0        0      381 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/end.py
--rw-r--r--   0        0        0     1411 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/in_interval.py
--rw-r--r--   0        0        0     1546 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/included_in.py
--rw-r--r--   0        0        0      587 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/overlaps.py
--rw-r--r--   0        0        0      976 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/interval/start.py
--rw-r--r--   0        0        0      348 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/list/distinct.py
--rw-r--r--   0        0        0      230 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/list/exists.py
--rw-r--r--   0        0        0      324 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/list/first.py
--rw-r--r--   0        0        0      291 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/list/flatten.py
--rw-r--r--   0        0        0     2195 2023-07-11 12:26:06.246231 cqlpy-0.2.7/cqlpy/_internal/operators/list/intersect.py
--rw-r--r--   0        0        0      306 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/list/last.py
--rw-r--r--   0        0        0      404 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/list/singleton_from.py
--rw-r--r--   0        0        0      236 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/list/union.py
--rw-r--r--   0        0        0      409 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/nullological/coalesce.py
--rw-r--r--   0        0        0      212 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/nullological/is_false.py
--rw-r--r--   0        0        0      358 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/nullological/is_null.py
--rw-r--r--   0        0        0      193 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/nullological/is_true.py
--rw-r--r--   0        0        0      254 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/sort/sort_by_column.py
--rw-r--r--   0        0        0      134 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/sort/sort_by_direction.py
--rw-r--r--   0        0        0      173 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/sort/sort_by_expression.py
--rw-r--r--   0        0        0       51 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/sort/tuple_sort.py
--rw-r--r--   0        0        0      166 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/string/ends_with.py
--rw-r--r--   0        0        0      170 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/string/split.py
--rw-r--r--   0        0        0      149 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/to_list.py
--rw-r--r--   0        0        0      162 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/type/to_concept.py
--rw-r--r--   0        0        0      280 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/operators/type/to_datetime.py
--rw-r--r--   0        0        0      509 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/parameter.py
--rw-r--r--   0        0        0        0 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/providers/__init__.py
--rw-r--r--   0        0        0     4258 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/providers/local_valueset_provider.py
--rw-r--r--   0        0        0      216 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/providers/logger.py
--rw-r--r--   0        0        0     4946 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/providers/rosetta_valueset_provider.py
--rw-r--r--   0        0        0    10714 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/scripts/fhir_map_generator.py
--rw-r--r--   0        0        0        0 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/__init__.py
--rw-r--r--   0        0        0     2901 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/any.py
--rw-r--r--   0        0        0      988 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/boolean.py
--rw-r--r--   0        0        0     1700 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/code.py
--rw-r--r--   0        0        0      851 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/code_system.py
--rw-r--r--   0        0        0     2457 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/concept.py
--rw-r--r--   0        0        0     1001 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/date.py
--rw-r--r--   0        0        0     2986 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/datetime.py
--rw-r--r--   0        0        0     1128 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/decimal.py
--rw-r--r--   0        0        0      756 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/integer.py
--rw-r--r--   0        0        0     3674 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/interval.py
--rw-r--r--   0        0        0     1605 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/list.py
--rw-r--r--   0        0        0       81 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/long.py
--rw-r--r--   0        0        0      416 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/null.py
--rw-r--r--   0        0        0      887 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/quantity.py
--rw-r--r--   0        0        0     1053 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/string.py
--rw-r--r--   0        0        0     1997 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/valueset.py
--rw-r--r--   0        0        0      731 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/types/valueset_scope.py
--rw-r--r--   0        0        0      372 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/_internal/valueset_provider.py
--rw-r--r--   0        0        0      450 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/context.py
--rw-r--r--   0        0        0     4227 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/operators.py
--rw-r--r--   0        0        0      319 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/providers.py
--rw-r--r--   0        0        0        0 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/py.typed
--rw-r--r--   0        0        0     1088 2023-07-11 12:26:06.250231 cqlpy-0.2.7/cqlpy/types.py
--rw-r--r--   0        0        0      670 2023-07-11 12:26:30.598128 cqlpy-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 cqlpy-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-13 18:37:17.964717 cqlpy-0.3.0/LICENSE
+-rw-r--r--   0        0        0    16761 2023-07-13 18:37:17.964717 cqlpy-0.3.0/README.md
+-rw-r--r--   0        0        0      519 2023-07-13 18:37:17.964717 cqlpy-0.3.0/cqlpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:37:17.964717 cqlpy-0.3.0/cqlpy/_internal/__init__.py
+-rw-r--r--   0        0        0     5253 2023-07-13 18:37:17.964717 cqlpy-0.3.0/cqlpy/_internal/context/context.py
+-rw-r--r--   0        0        0     2272 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/context/cql_valueset_provider.py
+-rw-r--r--   0        0        0      829 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/context/fhir/fhir_cql_type.py
+-rw-r--r--   0        0        0  1023948 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/context/fhir/r4/map.py
+-rw-r--r--   0        0        0    19176 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/context/fhir/r4/model.py
+-rw-r--r--   0        0        0      689 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/context/parameter_provider.py
+-rw-r--r--   0        0        0     3013 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/context/resource_query.py
+-rw-r--r--   0        0        0     2561 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/context/type_factory.py
+-rw-r--r--   0        0        0      412 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/exceptions.py
+-rw-r--r--   0        0        0      266 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/logger.py
+-rw-r--r--   0        0        0      472 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/operators/aggregate/count.py
+-rw-r--r--   0        0        0      747 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/operators/arithmetic/max_value.py
+-rw-r--r--   0        0        0      717 2023-07-13 18:37:17.968716 cqlpy-0.3.0/cqlpy/_internal/operators/arithmetic/min_value.py
+-rw-r--r--   0        0        0     1457 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/clinical/any_in_valueset.py
+-rw-r--r--   0        0        0     1158 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/clinical/calculate_age_at.py
+-rw-r--r--   0        0        0     1635 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/clinical/in_valueset.py
+-rw-r--r--   0        0        0      692 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/comparison/equal.py
+-rw-r--r--   0        0        0     1261 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/comparison/equivalent.py
+-rw-r--r--   0        0        0     1297 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/comparison/greater.py
+-rw-r--r--   0        0        0     1387 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/comparison/greater_or_equal.py
+-rw-r--r--   0        0        0      947 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/comparison/in_list.py
+-rw-r--r--   0        0        0     1283 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/comparison/less.py
+-rw-r--r--   0        0        0     1386 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/comparison/less_or_equal.py
+-rw-r--r--   0        0        0     1352 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/comparison/not_equal.py
+-rw-r--r--   0        0        0     1890 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/cql_in.py
+-rw-r--r--   0        0        0     1716 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/date_time/add.py
+-rw-r--r--   0        0        0     1145 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/date_time/after.py
+-rw-r--r--   0        0        0     1180 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/date_time/before.py
+-rw-r--r--   0        0        0      170 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/date_time/date_time_precision.py
+-rw-r--r--   0        0        0     1540 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/date_time/difference_between.py
+-rw-r--r--   0        0        0     1645 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/date_time/duration_between.py
+-rw-r--r--   0        0        0     1163 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/date_time/same_or_before.py
+-rw-r--r--   0        0        0     1833 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/date_time/subtract.py
+-rw-r--r--   0        0        0     4428 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/interval/collapse.py
+-rw-r--r--   0        0        0      814 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/interval/end.py
+-rw-r--r--   0        0        0     2062 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/interval/in_interval.py
+-rw-r--r--   0        0        0     2510 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/interval/included_in.py
+-rw-r--r--   0        0        0     1175 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/interval/overlaps.py
+-rw-r--r--   0        0        0     1046 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/interval/start.py
+-rw-r--r--   0        0        0      759 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/list/distinct.py
+-rw-r--r--   0        0        0      727 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/list/exists.py
+-rw-r--r--   0        0        0      758 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/list/first.py
+-rw-r--r--   0        0        0      738 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/list/flatten.py
+-rw-r--r--   0        0        0     2551 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/list/intersect.py
+-rw-r--r--   0        0        0      686 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/list/last.py
+-rw-r--r--   0        0        0      732 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/list/singleton_from.py
+-rw-r--r--   0        0        0      681 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/list/union.py
+-rw-r--r--   0        0        0      845 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/nullological/coalesce.py
+-rw-r--r--   0        0        0      597 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/nullological/is_false.py
+-rw-r--r--   0        0        0      761 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/nullological/is_null.py
+-rw-r--r--   0        0        0      587 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/nullological/is_true.py
+-rw-r--r--   0        0        0      875 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/sort/sort_by_column.py
+-rw-r--r--   0        0        0      502 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/sort/sort_by_direction.py
+-rw-r--r--   0        0        0      730 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/sort/sort_by_expression.py
+-rw-r--r--   0        0        0      302 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/sort/tuple_sort.py
+-rw-r--r--   0        0        0      738 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/string/ends_with.py
+-rw-r--r--   0        0        0      694 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/string/split.py
+-rw-r--r--   0        0        0      562 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/to_list.py
+-rw-r--r--   0        0        0      485 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/type/to_concept.py
+-rw-r--r--   0        0        0      707 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/operators/type/to_datetime.py
+-rw-r--r--   0        0        0      509 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/parameter.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/providers/__init__.py
+-rw-r--r--   0        0        0     4586 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/providers/local_valueset_provider.py
+-rw-r--r--   0        0        0     5363 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/providers/rosetta_valueset_provider.py
+-rw-r--r--   0        0        0     1510 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/providers/valueset_provider.py
+-rw-r--r--   0        0        0    10714 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/scripts/fhir_map_generator.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/__init__.py
+-rw-r--r--   0        0        0     3482 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/any.py
+-rw-r--r--   0        0        0     1364 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/boolean.py
+-rw-r--r--   0        0        0     2081 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/code.py
+-rw-r--r--   0        0        0     1190 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/code_system.py
+-rw-r--r--   0        0        0     2573 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/concept.py
+-rw-r--r--   0        0        0     1310 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/date.py
+-rw-r--r--   0        0        0     3517 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/datetime.py
+-rw-r--r--   0        0        0     1373 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/decimal.py
+-rw-r--r--   0        0        0     1001 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/integer.py
+-rw-r--r--   0        0        0     4593 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/interval.py
+-rw-r--r--   0        0        0     1649 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/list.py
+-rw-r--r--   0        0        0      226 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/long.py
+-rw-r--r--   0        0        0      921 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/null.py
+-rw-r--r--   0        0        0     1246 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/quantity.py
+-rw-r--r--   0        0        0     1294 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/string.py
+-rw-r--r--   0        0        0     2678 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/valueset.py
+-rw-r--r--   0        0        0      731 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/_internal/types/valueset_scope.py
+-rw-r--r--   0        0        0      430 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/exceptions.py
+-rw-r--r--   0        0        0     4226 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/operators.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/py.typed
+-rw-r--r--   0        0        0     1088 2023-07-13 18:37:17.972716 cqlpy-0.3.0/cqlpy/types.py
+-rw-r--r--   0        0        0      671 2023-07-13 18:37:43.940838 cqlpy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    17307 1970-01-01 00:00:00.000000 cqlpy-0.3.0/PKG-INFO
```

### Comparing `cqlpy-0.2.7/LICENSE` & `cqlpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.7/cqlpy/_internal/context/context.py` & `cqlpy-0.3.0/cqlpy/_internal/context/context.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,73 +4,96 @@
 
 from cqlpy._internal.context.fhir.r4.model import FhirR4DataModel
 from cqlpy._internal.context.parameter_provider import ParameterProvider
 from cqlpy._internal.parameter import Parameter
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.valueset import Valueset
 from cqlpy._internal.types.valueset_scope import ValuesetScope
-from cqlpy._internal.valueset_provider import ValuesetProvider
+from cqlpy._internal.providers.valueset_provider import ValuesetProvider
+
+from cqlpy._internal.exceptions import CqlPyValueError
 
 
 class Context:
     """
     A context is a required parameter on every CQL expression that is converted to python as a function.
+
+    ## Usage
+
     The expected signature of every function that implements a CQL Expression is:
 
-        def EXPRESSION_NAME(context: Context):
+    ```python
+    def EXPRESSION_NAME(context: Context):
+    ```
 
     The Context provides access to the data model, parameter values, and value set codes as needed by the internal elements
     of a python function that implements a CQL expression. The Context provides access to these concepts via a retrieve operation
     that is implemented with syntax such as:
 
-        context["Encounter"]    # if a string is requested (assumed to be a FHIR resource type), context returns a
-                                # list of Resources from the model, in this case all Encounter resources.
-
-        context["Encounter", Valueset, "type"]
-                                # if a tuple is requested (assumed to be a FHIR resource type), context returns a
-                                # list of Resources from the model, in this case Encounter resources, filtered by
-                                # checking the specified property to see if it has a coded value in the specified value set.
-
-        context[Parameter]      # if a Parameter is requested, context returns the type specified by the Parameter
-                                # with value determined by the parameter_provider from external parameters or the default value.
-
-        context[Valueset]       # if a Valueset is requested, context returns a Valueset that includes with Codes property populated
-                                # from the valueset_provider.
+    ```python
+    context["Encounter"]    # if a string is requested (assumed to be a FHIR resource type), context returns a
+                            # list of Resources from the model, in this case all Encounter resources.
+
+    context["Encounter", Valueset, "type"]
+                            # if a tuple is requested (assumed to be a FHIR resource type), context returns a
+                            # list of Resources from the model, in this case Encounter resources, filtered by
+                            # checking the specified property to see if it has a coded value in the specified value set.
+
+    context[Parameter]      # if a Parameter is requested, context returns the type specified by the Parameter
+                            # with value determined by the parameter_provider from external parameters or the default value.
+
+    context[Valueset]       # if a Valueset is requested, context returns a Valueset that includes with Codes property populated
+                            # from the valueset_provider.
+    ```
 
     The Context iterates through the bundle (as a json object) to retrieve a list of Resources.
 
     Properties of Resources can be obtained using syntax such as:
 
-        Encounter["period"]     # The property of the resource is properly typed when requested (in this case, Interval)
-                                # by parsing the related bundle json element.
+    ```
+    Encounter["period"]     # The property of the resource is properly typed when requested (in this case, Interval)
+                            # by parsing the related bundle json element.
+    ```
 
     Context Resource retrieve operations and Resource property retrieve operations are cached so that iterating through the bundle
     and parsing json is only performed once (at time of the first request).
     """
 
     def __init__(
         self,
         valueset_provider: ValuesetProvider,
         bundle: Optional[Union[str, dict]] = None,
         bundle_file_name: Optional[str] = None,
         parameters: Optional[dict] = None,
     ):
+        """
+        Create a new Context.
+
+        ## Parameters
+
+        - `valueset_provider`: A `cqlpy.providers.ValuesetProvider` that is used to retrieve valuesets by id.
+            Available providers are in `cqlpy.providers`.
+        - `bundle`: A json object that represents a FHIR bundle.
+        - `bundle_file_name`: A file name that contains a FHIR bundle as JSON.
+        - `parameters`: Parameters used to control execution of the CQL.
+        """
+
         parsed_bundle = None
         if bundle_file_name:
             with open(bundle_file_name, encoding="utf-8") as f:
                 parsed_bundle = json.loads(f.read())
 
         if isinstance(bundle, str):
             parsed_bundle = json.loads(bundle)
 
         if isinstance(bundle, dict):
             parsed_bundle = bundle
 
         if parsed_bundle is None:
-            raise ValueError("bundle or bundle_file_name must be specified")
+            raise CqlPyValueError("bundle or bundle_file_name must be specified")
 
         self.parameter_provider = ParameterProvider(parameters)
         self.model = FhirR4DataModel(parsed_bundle, self.parameter_provider)
         self.cql_valueset_provider = CqlValuesetProvider(
             valueset_provider=valueset_provider
         )
 
@@ -96,18 +119,7 @@
             return self.cql_valueset_provider[requested_concept]
 
         if isinstance(requested_concept, Code):
             # In this case, there is nothing to lookup... the Code is fully populated.
             return requested_concept
 
         return self.model[requested_concept]
-
-    def set_context(self, context: str) -> None:
-        # At this time, only Patient context is supported and the context is stored without additional action.
-        # The current implementation can be extended to support additional contexts by using this stored context in
-        # retrieve operations (implemented in __getitem__) to filter the resources returned from the model.
-        self.context = context
-
-    def initialize(self, model, parameter_provider, cql_valueset_provider) -> None:
-        self.model = model
-        self.parameter_provider = parameter_provider
-        self.cql_valueset_provider = cql_valueset_provider
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/context/cql_valueset_provider.py` & `cqlpy-0.3.0/cqlpy/_internal/context/cql_valueset_provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from typing import Union
-from cqlpy._internal.exceptions import ValuesetProviderError
+
+from cqlpy._internal.exceptions import CqlPyValueError, ValuesetProviderError
+from cqlpy._internal.logger import get_logger
 from cqlpy._internal.types.valueset import Valueset
 from cqlpy._internal.types.valueset_scope import ValuesetScope
-from cqlpy._internal.valueset_provider import ValuesetProvider, ValuesetScopeProvider
+from cqlpy._internal.providers.valueset_provider import (
+    ValuesetProvider,
+    ValuesetScopeProvider,
+)
 
 _COMMON_URL_PREFIXES = [
     "http://cts.nlm.nih.gov/fhir/ValueSet/",
     "http://hl7.org/fhir/ValueSet/",
 ]
 
 
@@ -16,46 +21,47 @@
             return name[len(prefix) :]
     return name
 
 
 class CqlValuesetProvider:
     def __init__(self, valueset_provider: ValuesetProvider) -> None:
         self._valueset_provider = valueset_provider
+        self.__logger = get_logger().getChild(self.__class__.__name__)
 
     def __get_valueset(self, item: Valueset) -> Valueset:
         if item.id is None:
-            raise ValueError("value set id must be specified")
+            raise CqlPyValueError("value set id must be specified")
 
         name = _clean_name(item.id)
         result = self._valueset_provider.get_valueset(name=name, scope=None)
 
         if result:
             return Valueset.parse_fhir_json(result)
 
-        print(f"value set 'scopeless:{item.name}' not found")
+        self.__logger.warn(f"value set 'scopeless:{item.name}' not found")
 
         return item
 
     def __get_valueset_scope(self, item: ValuesetScope) -> list[Valueset]:
         if not isinstance(self._valueset_provider, ValuesetScopeProvider):
             raise ValuesetProviderError(
                 "The value set provider does not support scope-based value set retrieval"
             )
 
         if item.id is None:
-            raise ValueError("value set scope id must be specified")
+            raise CqlPyValueError("value set scope id must be specified")
 
         result = self._valueset_provider.get_valuesets_in_scope(scope=item.id)
 
         if result:
             return [
                 Valueset.parse_fhir_json(valueset["resource"]) for valueset in result
             ]
 
-        print(f"value set scope '{item.id}' not found")
+        self.__logger.error(f"value set scope '{item.id}' not found")
 
         return []
 
     def __getitem__(
         self, item: Union[Valueset, ValuesetScope]
     ) -> Union[Valueset, list[Valueset]]:
         if isinstance(item, ValuesetScope):
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/context/fhir/fhir_cql_type.py` & `cqlpy-0.3.0/cqlpy/_internal/context/fhir/fhir_cql_type.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.7/cqlpy/_internal/context/fhir/r4/map.py` & `cqlpy-0.3.0/cqlpy/_internal/context/fhir/r4/map.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.7/cqlpy/_internal/context/fhir/r4/model.py` & `cqlpy-0.3.0/cqlpy/_internal/context/fhir/r4/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from datetime import datetime
 import json
 from typing import Iterator, Optional, Protocol, Sequence, Union
 
 from cqlpy._internal.context.parameter_provider import ParameterProvider
 from cqlpy._internal.context.resource_query import ResourceQuery, ResourceQueryFilter
 from cqlpy._internal.context.type_factory import TypeFactory
+from cqlpy._internal.logger import get_logger
+from cqlpy._internal.exceptions import CqlPyValueError
 from cqlpy._internal.operators.comparison.in_list import in_list
 from cqlpy._internal.operators.list.exists import exists
 from cqlpy._internal.operators.list.intersect import intersect
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.parameter import Parameter
 from cqlpy._internal.types.any import CqlAny
 from cqlpy._internal.types.code import Code
@@ -40,15 +42,15 @@
         return json.dumps(self._fhir_json)
 
     def __handle_choice(
         self, property_name: str, fhir_cql_type: FhirChoice
     ) -> Optional[CqlAny]:
         value: Optional[CqlAny] = None
         if any(
-            choice.item_type == "DateTime"
+            choice.item_type.name == "DateTime"
             for choice in fhir_cql_type.choices
             if isinstance(choice, FhirInterval)
         ):
             if f"{property_name}DateTime" in self._fhir_json:
                 value = DateTime.parse_fhir_json(
                     self._fhir_json[f"{property_name}DateTime"]
                 )
@@ -58,15 +60,15 @@
             if f"{property_name}DateTime" in self._fhir_json:
                 value = DateTime.parse_fhir_json(
                     self._fhir_json[f"{property_name}DateTime"]
                 )
                 return value
 
         elif any(
-            choice.item_type == "Date"
+            choice.item_type.name == "Date"
             for choice in fhir_cql_type.choices
             if isinstance(choice, FhirInterval)
         ):
             if f"{property_name}Date" in self._fhir_json:
                 value = Date.parse_fhir_json(self._fhir_json[f"{property_name}Date"])
                 return Interval(value, True, value, True)
 
@@ -254,26 +256,27 @@
         codes: list[Code] = []
         for item in filter_:
             if isinstance(item, Valueset):
                 codes.extend(item.codes)
             elif isinstance(item, Code):
                 codes.append(item)
             else:
-                raise ValueError(f"Unsupported filter item type: {type(item)}")
+                raise CqlPyValueError(f"Unsupported filter item type: {type(item)}")
         return codes
 
     raise NotImplementedError
 
 
 class FhirR4DataModel:
     def __init__(self, bundle: dict, parameter_provider: ParameterProvider) -> None:
         self.__parameter_provider = parameter_provider
         self.resource_id_index = {}
         self.resource_type_index: dict[str, list[str]] = {}
         self.retrieve_cache: dict[ResourceQuery, list[Resource]] = {}
+        self.__logger = get_logger().getChild(self.__class__.__name__)
 
         if "entry" not in bundle:
             return
 
         for entry in bundle["entry"]:
             if not (
                 (resource_json := entry.get("resource"))
@@ -426,38 +429,38 @@
         ],
     ) -> Sequence[FhirBase]:
         duration_start_time = datetime.now()
 
         query = ResourceQuery.from_query(resource_query)
 
         if query in self.retrieve_cache:
-            print(
+            self.__logger.info(
                 f"retrieve from cache duration={(datetime.now() - duration_start_time).total_seconds()} resourceType={query.resource_type} filter={query.description}"
             )
             return self.retrieve_cache[query]
 
         resources = list(self.__retrieve_resources(query))
 
         if query.property_filter is None:
             return resources
 
         if self.__parameter_provider[Parameter("strict", "String")] == "True":
-            print(
+            self.__logger.info(
                 f"retrieve strict=True resources={len(resources)} duration={(datetime.now() - duration_start_time).total_seconds()} resourceType={query.resource_type} filter={query.description}"
             )
             self.retrieve_cache[query] = resources
 
             return resources
 
         resource_proxies = list(
             self.__build_resource_proxies(
                 resource_type=query.resource_type, resources=resources
             )
         )
-        print(
+        self.__logger.info(
             f"retrieve resources={len(resource_proxies)} duration={(datetime.now() - duration_start_time).total_seconds()} resourceType={query.resource_type} filter={query.description}"
         )
         self.retrieve_cache[query] = resource_proxies
 
         return resource_proxies
 
     def __generate_resource_proxy(
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/context/parameter_provider.py` & `cqlpy-0.3.0/cqlpy/_internal/context/parameter_provider.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.7/cqlpy/_internal/context/resource_query.py` & `cqlpy-0.3.0/cqlpy/_internal/context/resource_query.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.7/cqlpy/_internal/context/type_factory.py` & `cqlpy-0.3.0/cqlpy/_internal/context/type_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, Literal, Optional, Type, TypeVar, Union
+from typing import Optional, Type
+
+from cqlpy._internal.exceptions import CqlPyTypeError
 from cqlpy._internal.types.any import CqlAny
 from cqlpy._internal.types.boolean import Boolean
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.concept import Concept
 from cqlpy._internal.types.date import Date
 from cqlpy._internal.types.datetime import DateTime
 from cqlpy._internal.types.decimal import Decimal
@@ -52,15 +54,15 @@
 class TypeFactory:
     @staticmethod
     def get_type(type_name: str) -> tuple[Type[CqlAny], Optional[Type[CqlAny]]]:
         cql_name, subtype_name = _split_generic_name(type_name)
         cql_type, subtype = _map_cql_type(cql_name), _map_cql_type(subtype_name)
 
         if cql_type is None:
-            raise ValueError(f"Unknown CQL type: {type_name}")
+            raise CqlPyTypeError(f"Unknown CQL type: {type_name}")
 
         return cql_type, subtype
 
     @staticmethod
     def get_type_from_fhir_cql(
         fhir_cql_type: FhirCqlType,
     ) -> tuple[Type[CqlAny], Optional[Type[CqlAny]]]:
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/operators/comparison/greater.py` & `cqlpy-0.3.0/cqlpy/_internal/operators/comparison/greater.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,38 @@
-# 5.4 Greater https://cql.hl7.org/09-b-cqlreference.html#greater
-
-
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.types.quantity import Quantity
+from cqlpy._internal.types.boolean import Boolean
+
+
+def greater(left, right) -> Boolean:
+    """
+    Returns True if the left argument is greater than the right
+    argument, False otherwise. You may also use the `>` operator to
+    compare two values, though the result will be a Python type.
+
+    [Specification](http://cql.hl7.org/09-b-cqlreference.html#greater)
+
+    ## Parameters
+
+    - `left`: The left argument.
+    - `right`: The right argument.
+
+    ## Returns
+
+    True if the left argument is greater than the right argument, False
+    otherwise.
 
+    ## Usage
 
-def greater(left, right) -> bool:
+    ```python
+    greater(Integer(2), Integer(1))  # True
+    ```
+    """
     if is_null(left) or is_null(right):
-        return False
+        return Boolean(False)
     else:
         left_value = (
             left["value"]
             if left.__class__.__name__ == "Resource"
             else left.value
             if isinstance(left, Quantity)
             else left
@@ -19,8 +40,8 @@
         right_value = (
             right["value"]
             if right.__class__.__name__ == "Resource"
             else right.value
             if isinstance(right, Quantity)
             else right
         )
-        return left > right
+        return Boolean(left > right)
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/operators/comparison/less_or_equal.py` & `cqlpy-0.3.0/cqlpy/_internal/operators/comparison/less_or_equal.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,40 @@
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.types.quantity import Quantity
 
-# 5.7 Less or Equal https://cql.hl7.org/09-b-cqlreference.html#less-or-equal
+from cqlpy._internal.types.boolean import Boolean
 
 
-def less_or_equal(left, right) -> bool:
+def less_or_equal(left, right) -> Boolean:
+    """
+    Returns True if the left argument is less than or equal to the
+    right argument, False otherwise. You may also use the `<=` operator
+    to compare two values, though the result will be a Python type.
+
+    [Specification](http://cql.hl7.org/09-b-cqlreference.html#less-or-equal)
+
+    ## Parameters
+
+    - `left`: The left argument.
+    - `right`: The right argument.
+
+    ## Returns
+
+    True if the left argument is less than or equal to the right
+    argument, False otherwise.
+
+    ## Usage
+
+    ```python
+    less_or_equal(Integer(1), Integer(2))  # True
+    less_or_equal(Integer(1), Integer(1))  # True
+    ```
+    """
     if is_null(left) or is_null(right):
-        return False
+        return Boolean(False)
     else:
         left_value = (
             left["value"]
             if left.__class__.__name__ == "Resource"
             else left.value
             if isinstance(left, Quantity)
             else left
@@ -18,8 +42,8 @@
         right_value = (
             right["value"]
             if right.__class__.__name__ == "Resource"
             else right.value
             if isinstance(right, Quantity)
             else right
         )
-        return left <= right
+        return Boolean(left <= right)
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/operators/date_time/add.py` & `cqlpy-0.3.0/cqlpy/_internal/operators/date_time/subtract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,48 @@
-# 8.1 Add https://cql.hl7.org/09-b-cqlreference.html#add-1
+# 8.15 Substract https://cql.hl7.org/09-b-cqlreference.html#subtract-1
 
+from datetime import timedelta
 from dateutil.relativedelta import relativedelta
 
-from datetime import timedelta
 from cqlpy._internal.operators.date_time.date_time_precision import DateTimePrecision
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.types.datetime import DateTime
 from cqlpy._internal.types.null import Null, Some
 from cqlpy._internal.types.quantity import Quantity
 
 
-def add(left: DateTime, right: Quantity) -> Some[DateTime]:
+def subtract(left: DateTime, right: Quantity) -> Some[DateTime]:
+    """
+    Subtracts the given quantity from the given `DateTime`. Implements CQL's `subtract`.
+
+    [Specification](https://cql.hl7.org/09-b-cqlreference.html#subtract-1)
+
+    ## Parameters
+
+    - `left`: The `DateTime` to subtract from.
+    - `right`: The `Quantity` to subtract.
+
+    ## Returns
+
+    A new `DateTime` with the given quantity subtracted from it.
+
+    ## Usage
+
+    ```python
+    subtract(DateTime(2012, 1, 1), Quantity(1, "years"))  # DateTime(2011, 1, 1)
+    ```
+    """
     if is_null(left) or is_null(right):
         return Null()
     assert right.value is not None
 
     if (right.unit == "days") or (right.unit == DateTimePrecision.Day):
-        return DateTime().parse_datetime(left.value + timedelta(days=right.value))
+        return DateTime().parse_datetime(left.value - timedelta(days=right.value))
     if (right.unit == "weeks") or (right.unit == DateTimePrecision.Week):
-        return DateTime().parse_datetime(left.value + timedelta(days=7 * right.value))
+        return DateTime().parse_datetime(left.value - timedelta(days=7 * right.value))
     if (right.unit == "months") or (right.unit == DateTimePrecision.Month):
         months = int(right.value)
-        return DateTime().parse_datetime(left.value + relativedelta(months=months))
+        return DateTime().parse_datetime(left.value - relativedelta(months=months))
     if (right.unit == "years") or (right.unit == DateTimePrecision.Year):
         years = int(right.value)
-        return DateTime().parse_datetime(left.value + relativedelta(years=years))
-
+        return DateTime().parse_datetime(left.value - relativedelta(years=years))
     return Null()
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/operators/date_time/duration_between.py` & `cqlpy-0.3.0/cqlpy/_internal/operators/date_time/difference_between.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,49 @@
+from dateutil.relativedelta import relativedelta
+
 from cqlpy._internal.operators.date_time.date_time_precision import DateTimePrecision
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.types.datetime import DateTime
+from cqlpy._internal.types.integer import Integer
 from cqlpy._internal.types.null import Null, Some
 
-from dateutil.relativedelta import relativedelta
 
+def difference_between(
+    low: DateTime,
+    high: DateTime,
+    precision: DateTimePrecision,
+) -> Some[Integer]:
+    """
+    Returns the number of boundaries crossed for the specified precision between the two `DateTime`s.
+    Implements CQL's `difference between`.
+
+    If either argument is `Null`, the result is `Null`.
+
+    [Specification](https://cql.hl7.org/09-b-cqlreference.html#difference)
 
-# 8.8 Duration Between https://cql.hl7.org/09-b-cqlreference.html#duration
+    ## Parameters
 
+    - `low`: The first `DateTime`.
+    - `high`: The second `DateTime`.
 
-def duration_between(
-    low: DateTime, high: DateTime, precision: DateTimePrecision
-) -> Some[int]:
+    ## Returns
+
+    The number of boundaries crossed between the two `DateTime`s.
+
+    ## Usage
+
+    ```python
+    difference_between(DateTime(2012, 1, 1), DateTime(2013, 1, 1), DateTimePrecision.Year)  # Integer(1)
+    ```
+    """
     if is_null(low) or is_null(high):
         return Null()
-    elif precision == DateTimePrecision.Day:
-        return (high.value - low.value).days
-    elif precision == DateTimePrecision.Month:
-        (high.value.year - low.value.year) * 12 + high.value.month - low.value.month
-    elif precision == DateTimePrecision.Year:
-        return relativedelta(high.value, low.value).years
+    if precision == DateTimePrecision.Day:
+        return Integer((high.value - low.value).days)
+    if precision == DateTimePrecision.Month:
+        return Integer(
+            (high.value.year - low.value.year) * 12 + high.value.month - low.value.month
+        )
+    if precision == DateTimePrecision.Year:
+        return Integer(relativedelta(high.value, low.value).years)
+
     return Null()
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/operators/date_time/subtract.py` & `cqlpy-0.3.0/cqlpy/_internal/operators/date_time/add.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,47 @@
-# 8.15 Substract https://cql.hl7.org/09-b-cqlreference.html#subtract-1
-
-from datetime import timedelta
 from dateutil.relativedelta import relativedelta
 
+from datetime import timedelta
 from cqlpy._internal.operators.date_time.date_time_precision import DateTimePrecision
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.types.datetime import DateTime
 from cqlpy._internal.types.null import Null, Some
 from cqlpy._internal.types.quantity import Quantity
 
 
-def subtract(left: DateTime, right: Quantity) -> Some[DateTime]:
+def add(left: DateTime, right: Quantity) -> Some[DateTime]:
+    """
+    Adds the given quantity to the given `DateTime`. Implements CQL's `add`.
+
+    [Specification](https://cql.hl7.org/09-b-cqlreference.html#add-1)
+
+    ## Parameters
+
+    - `left`: The `DateTime` to add to.
+    - `right`: The `Quantity` to add.
+
+    ## Returns
+
+    A new `DateTime` with the given quantity added to it.
+
+    ## Usage
+
+    ```python
+    add(DateTime(2012, 1, 1), Quantity(1, "years"))  # DateTime(2013, 1, 1)
+    ```
+    """
     if is_null(left) or is_null(right):
         return Null()
     assert right.value is not None
 
     if (right.unit == "days") or (right.unit == DateTimePrecision.Day):
-        return DateTime().parse_datetime(left.value - timedelta(days=right.value))
+        return DateTime().parse_datetime(left.value + timedelta(days=right.value))
     if (right.unit == "weeks") or (right.unit == DateTimePrecision.Week):
-        return DateTime().parse_datetime(left.value - timedelta(days=7 * right.value))
+        return DateTime().parse_datetime(left.value + timedelta(days=7 * right.value))
     if (right.unit == "months") or (right.unit == DateTimePrecision.Month):
         months = int(right.value)
-        return DateTime().parse_datetime(left.value - relativedelta(months=months))
+        return DateTime().parse_datetime(left.value + relativedelta(months=months))
     if (right.unit == "years") or (right.unit == DateTimePrecision.Year):
         years = int(right.value)
-        return DateTime().parse_datetime(left.value - relativedelta(years=years))
+        return DateTime().parse_datetime(left.value + relativedelta(years=years))
+
     return Null()
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/operators/interval/collapse.py` & `cqlpy-0.3.0/cqlpy/_internal/operators/interval/collapse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Optional
+from cqlpy._internal.exceptions import CqlPyTypeError, CqlPyValueError
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.types.date import Date
 from cqlpy._internal.types.datetime import DateTime
 from cqlpy._internal.types.decimal import Decimal
 from cqlpy._internal.types.integer import Integer
 from cqlpy._internal.types.list import List
 from cqlpy._internal.types.interval import Interval, IntervalBoundType
@@ -11,15 +12,15 @@
 
 def _get_sortable_interval_value(
     interval: Interval[IntervalBoundType],
 ) -> tuple[IntervalBoundType, int, IntervalBoundType, int]:
     low = interval.low if interval.low is not None else None
     high = interval.high if interval.high is not None else None
     if low is None or high is None:
-        raise ValueError("Cannot sort interval with null bounds")
+        raise CqlPyValueError("Cannot sort interval with null bounds")
     return (
         low,
         0 if interval.low_closed else 1,
         high,
         0 if interval.high_closed else 1,
     )
 
@@ -37,14 +38,37 @@
         return not (some_first_closed or some_next_closed)
     return first < next_
 
 
 def collapse(
     argument: Some[List[Some[Interval[IntervalBoundType]]]],
 ) -> Some[List[Interval[IntervalBoundType]]]:
+    """
+    Collapses a list of intervals into a list of intervals with no overlaps.
+    Implements CQL's `collapse`.
+
+    If the argument is `Null`, the result is `Null`.
+
+    [Specification](https://cql.hl7.org/09-b-cqlreference.html#collapse)
+
+    ## Parameters
+
+    - `argument`: The list of intervals to collapse.
+
+    ## Returns
+
+    A new list of intervals with no overlaps.
+
+    ## Usage
+
+    ```python
+    collapse(List([Interval(1, 2), Interval(2, 3)]))  # List([Interval(1, 3)])
+    ```
+    """
+
     if is_null(argument):
         return Null()
     assert isinstance(argument, List)
     if len(argument) == 0:
         return List([])
     if len(argument) == 1 and is_null(argument[0]):
         return List([])
@@ -67,15 +91,15 @@
             continue
         if (
             interval.low is None
             or last_interval.high is None
             or interval.high is None
             or last_interval.low is None
         ):
-            raise ValueError("Cannot collapse interval with null bounds")
+            raise CqlPyValueError("Cannot collapse interval with null bounds")
 
         if _space_between_points(
             first=last_interval.high,
             first_closed=last_interval.high_closed,
             next_=interval.low,
             next_closed=interval.low_closed,
         ):
@@ -89,17 +113,19 @@
             high = last_interval.high
             high_closed = last_interval.high_closed
         else:
             high = interval.high
             high_closed = interval.high_closed
 
         if not isinstance(high, (DateTime, Date, Integer, Decimal)):
-            raise TypeError(f"Expected an interval type, got {type(high)}")
+            raise CqlPyTypeError(f"Expected an interval type, got {type(high)}")
         if not isinstance(last_interval.low, (DateTime, Date, Integer, Decimal)):
-            raise TypeError(f"Expected an interval type, got {type(last_interval.low)}")
+            raise CqlPyTypeError(
+                f"Expected an interval type, got {type(last_interval.low)}"
+            )
         collapsed_list[-1] = Interval(
             last_interval.low,
             last_interval.low_closed if last_interval.low_closed is not None else True,
             high,
             high_closed if high_closed is not None else True,
         )
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/operators/interval/included_in.py` & `cqlpy-0.3.0/cqlpy/_internal/operators/interval/included_in.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,81 @@
 # 9.13 Included In https://cql.hl7.org/09-b-cqlreference.html#included-in
 
 from typing import Union
+from cqlpy._internal.exceptions import CqlPyTypeError
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.types.date import Date
 from cqlpy._internal.types.datetime import DateTime
 from cqlpy._internal.types.decimal import Decimal
 from cqlpy._internal.types.integer import Integer
 
 from cqlpy._internal.types.interval import Interval
 from cqlpy._internal.types.null import Null
 
+from cqlpy._internal.types.boolean import Boolean
+
 
 _IncludedInType = Union[Interval, Date, DateTime, Integer, Decimal, None, Null]
 
 
-def included_in(left: _IncludedInType, right: Interval) -> bool:
+def included_in(left: _IncludedInType, right: Interval) -> Boolean:
+    """
+    Returns `True` if the left argument is part of the right `Interval`, `False` otherwise. If either argument is `Null`, the result is `False`.
+
+    [Specification](https://cql.hl7.org/09-b-cqlreference.html#included-in)
+
+    ## Parameters
+
+    - `left`: The point or interval to check for inclusion.
+    - `right`: The interval to check for inclusion in.
+
+    ## Returns
+
+    `True` if the left argument is part of the right `Interval`, `False` otherwise.
+
+    ## Usage
+
+    ```python
+    included_in(1, Interval(0, 2))  # True
+    included_in(Interval(1, 2), Interval(0, 2))  # True
+    ```
+    """
     if is_null(left) or is_null(right):
-        return False
+        return Boolean(False)
 
     if isinstance(left, Interval):
         if (
             len(
                 {
                     left.low.__class__,
                     left.high.__class__,
                     right.low.__class__,
                     right.high.__class__,
                 }
             )
             > 1
         ):
-            raise TypeError("Cannot compare intervals of different types")
-        return included_in(left.low, right) and included_in(left.high, right)
+            raise CqlPyTypeError("Cannot compare intervals of different types")
+
+        left_in = included_in(left.low, right)
+        right_in = included_in(left.high, right)
+        if is_null(left_in) or is_null(right_in):
+            return Boolean(False)
+        return Boolean(left_in.value and right_in.value)
 
     if (
         isinstance(left, DateTime)
         and isinstance(right, Interval)
         and isinstance(right.low, DateTime)
         and isinstance(right.high, DateTime)
     ):
-        return (
-            (left > right.low)
-            and (left < right.high)
-            or (left == right.low and right.low_closed)
-            or (left == right.high and right.high_closed)
-        ) or False
+        return Boolean(
+            (
+                (left > right.low)
+                and (left < right.high)
+                or (left == right.low and right.low_closed)
+                or (left == right.high and right.high_closed)
+            )
+            or False
+        )
 
-    return False
+    return Boolean(False)
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/operators/interval/start.py` & `cqlpy-0.3.0/cqlpy/_internal/operators/interval/start.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,19 +9,32 @@
 from cqlpy._internal.types.decimal import Decimal
 from cqlpy._internal.types.integer import Integer
 from cqlpy._internal.types.interval import Interval
 from cqlpy._internal.types.null import Null, Some
 
 
 def start(argument: Interval[DateTime]) -> Some[DateTime]:
+    """
+    Returns the start of the given `Interval`.
+
+    If the argument is `Null`, the result is `Null`.
+
+    [Specification](https://cql.hl7.org/09-b-cqlreference.html#start)
+
+    ## Parameters
+
+    - `argument`: The `Interval` to get the start of.
+
+    ## Returns
+
+    The start of the given `Interval`.
+
+    ## Usage
+
+    ```python
+    start(Interval(1, 2))  # 1
+    ```
+    """
     if not is_null(argument):
         return argument.low or Null()
     else:
         return Null()
-
-
-# def overlaps(self, cql_interval) -> bool:
-#     return self.low.included_in(cql_interval) or self.high.included_in(cql_interval) or cql_interval.low.included_in(self)
-
-# def intersect(self, cql_interval): # -> CqlList:
-#     # this is just a placeholder to test syntax; implementation required
-#     return self
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/operators/list/intersect.py` & `cqlpy-0.3.0/cqlpy/_internal/operators/list/intersect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-# 10.4 Intersect https://cql.hl7.org/09-b-cqlreference.html#intersect-1
-
-
 from typing import TypeVar, Union
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.operators.interval.overlaps import overlaps
-from cqlpy._internal.types.any import CqlAny
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.date import Date
 from cqlpy._internal.types.datetime import DateTime
 from cqlpy._internal.types.decimal import Decimal
 from cqlpy._internal.types.integer import Integer
 from cqlpy._internal.types.interval import Interval
 from cqlpy._internal.types.null import Null
@@ -18,40 +14,65 @@
 )
 
 
 def intersect(
     left: Union[list[_IntersectType], Interval[_IntersectType]],
     right: Union[list[_IntersectType], Interval[_IntersectType]],
 ) -> Union[list, Interval, Null]:
-    if (not is_null(left)) and (not is_null(right)):
-        if isinstance(left, Interval) and isinstance(right, Interval):
-            if not (
-                isinstance(left.low, DateTime)
-                and isinstance(right.low, DateTime)
-                and isinstance(left.high, DateTime)
-                and isinstance(right.high, DateTime)
-            ):
-                return Null()
-            if overlaps(left, right):
-                return Interval(
-                    DateTime.parse_datetime(max(left.low.value, right.low.value)),
-                    False,
-                    DateTime.parse_datetime(min(left.high.value, right.high.value)),
-                    False,
-                )
-            return Null()
+    """
+    Returns the set intersection of the given lists or intervals. Items in the
+    arguments must be comparable and `DateTime`, `Date`, `Integer`, or `Decimal`.
+
+    If either argument is `Null`, the result is `Null`.
+
+    [Specification](https://cql.hl7.org/09-b-cqlreference.html#intersect-1)
+
+    ## Parameters
 
-        elif isinstance(left, list) and isinstance(right, list):
-            return_list = []
-            for left_item in left:
-                for right_item in right:
-                    if isinstance(left_item, Code) and isinstance(right_item, Code):
-                        if left_item.code == right_item.code:
-                            return_list.append(left_item)
-
-                    else:
-                        if left_item == right_item:
-                            return_list.append(left_item)
+    - `left`: The first list or interval.
+    - `right`: The second list or interval.
+
+    ## Returns
+
+    The common items of the given lists or intervals.
+
+    ## Usage
+
+    ```python
+    intersect([1, 2, 3], [2, 3, 4])  # [2, 3]
+    ```
+    """
+    if (is_null(left)) or (is_null(right)):
+        return Null()
+
+    if isinstance(left, Interval) and isinstance(right, Interval):
+        if not (
+            isinstance(left.low, DateTime)
+            and isinstance(right.low, DateTime)
+            and isinstance(left.high, DateTime)
+            and isinstance(right.high, DateTime)
+        ):
+            return Null()
+        if overlaps(left, right):
+            return Interval(
+                DateTime.parse_datetime(max(left.low.value, right.low.value)),
+                False,
+                DateTime.parse_datetime(min(left.high.value, right.high.value)),
+                False,
+            )
+        return Null()
+
+    if isinstance(left, list) and isinstance(right, list):
+        return_list = []
+        for left_item in left:
+            for right_item in right:
+                if isinstance(left_item, Code) and isinstance(right_item, Code):
+                    if left_item.code == right_item.code:
+                        return_list.append(left_item)
+
+                else:
+                    if left_item == right_item:
+                        return_list.append(left_item)
 
-            return return_list
+        return return_list
 
     return Null()
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/providers/local_valueset_provider.py` & `cqlpy-0.3.0/cqlpy/_internal/providers/local_valueset_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 import json
 import re
-from logging import getLogger
 from os import PathLike
 from pathlib import Path
 from typing import Optional
 
-from traitlets import Any
+from typing import Any
 
-from cqlpy._internal.valueset_provider import ValuesetProvider
+from cqlpy._internal.providers.valueset_provider import ValuesetProvider
+from cqlpy._internal.logger import get_logger
 
-_DEFAULT_FILE_PATTERN = r".*?\.json|.*?\.ndjson"
-
-
-class _ValuesetReadError(Exception):
-    ...
+from cqlpy._internal.exceptions import (
+    CqlPyKeyError,
+    ValuesetInterpretationError,
+    ValuesetReadError,
+)
 
-
-class _ValuesetInterpretationError(_ValuesetReadError):
-    ...
+_DEFAULT_FILE_PATTERN = r".*?\.json|.*?\.ndjson"
 
 
 class LocalValuesetProvider(ValuesetProvider):
     """
     A value set provider that loads value sets from a local directory or file.
 
     JSON and NDJSON files are supported.
-
-    :param directory_or_file: The directory or file to load value sets from. If a
-        directory is provided, all files in the directory will be loaded. If a file is
-        provided, only that file will be loaded.
-    :param pattern: A regular expression pattern to match files in the directory. Only
-        files that match the pattern will be loaded. Defaults to .json and .ndjson
-        files.
     """
 
     def __init__(
         self, directory_or_file: PathLike, pattern: Optional[str] = None
     ) -> None:
+        """
+        Creates a new local value set provider.
+
+        ## Parameters
+
+        - `directory_or_file`: The directory or file to load value sets from. If a
+            directory is provided, all files in the directory will be loaded. If a file is
+            provided, only that file will be loaded.
+        - `pattern`: A regular expression pattern to match files in the directory. Only
+            files that match the pattern will be loaded. Defaults to .json and .ndjson
+            files.
+        """
         self.__directory = Path(directory_or_file)
         self.__pattern = pattern
         self.__valuesets: Optional[dict[str, dict[str, Any]]] = None
-        self.__logger = getLogger()
+        self.__logger = get_logger().getChild(self.__class__.__name__)
 
     def __interpret_valueset(self, definition: str) -> list[tuple[str, dict[str, Any]]]:
         valuesets: list[tuple[str, dict[str, Any]]] = []
         try:
             valueset = json.loads(definition)
             valuesets.append((valueset["id"], valueset))
             return valuesets
@@ -53,31 +56,31 @@
                 try:
                     valueset = json.loads(line)
                     valuesets.append((valueset["id"], valueset))
                 except Exception as error:
                     self.__logger.warning(
                         f"Failed to interpret value set definition: {error}"
                     )
-                    raise _ValuesetInterpretationError(
+                    raise ValuesetInterpretationError(
                         "Failed to interpret value set definition"
                     ) from error
             return valuesets
         except Exception as error:
             self.__logger.warning(f"Failed to interpret value set definition: {error}")
-            raise _ValuesetInterpretationError(
+            raise ValuesetInterpretationError(
                 "Failed to interpret value set definition"
             ) from error
 
     def __read_valueset(self, path: Path) -> list[tuple[str, dict[str, Any]]]:
         try:
             with open(path, "r") as handle:
                 return self.__interpret_valueset(handle.read())
         except Exception as error:
             self.__logger.warning(f"Failed to read file {path}: {error}")
-            raise _ValuesetReadError(f"Failed to read file {path}") from error
+            raise ValuesetReadError(f"Failed to read file {path}") from error
 
     def __read_valuesets(self) -> dict[str, dict[str, Any]]:
         valuesets: dict[str, dict[str, Any]] = {}
         if self.__directory.is_file():
             self.__logger.debug(f"Reading value set from {self.__directory.name}")
             valueset_pairs = self.__read_valueset(self.__directory)
             for valueset_id, valueset_description in valueset_pairs:
@@ -94,17 +97,24 @@
             valueset_pairs = self.__read_valueset(file)
             for valueset_id, valueset_description in valueset_pairs:
                 valuesets[valueset_id] = valueset_description
         return valuesets
 
     @property
     def valuesets(self) -> dict[str, dict[str, Any]]:
+        """
+        All currently-loaded value sets.
+
+        ## Returns
+
+        A dictionary of value set IDs to value set definitions.
+        """
         if self.__valuesets is None:
             self.__valuesets = self.__read_valuesets()
         return self.__valuesets
 
     def get_valueset(self, name: str, scope: Optional[str]) -> dict[str, Any]:
         try:
             valueset = self.valuesets[name]
-        except _ValuesetReadError as error:
-            raise KeyError(f"Value set {name} not found") from error
+        except ValuesetReadError as error:
+            raise CqlPyKeyError(f"Value set {name} not found") from error
         return valueset
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/providers/rosetta_valueset_provider.py` & `cqlpy-0.3.0/cqlpy/_internal/providers/rosetta_valueset_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,52 @@
 from datetime import datetime
 import urllib
 import requests
 
 from typing import Optional, Any
 
-from cqlpy._internal.types.valueset import Valueset
+from cqlpy._internal.logger import get_logger
+
+from cqlpy._internal.exceptions import CqlPyValueError
 
 
 FHIR_VERSION = "R4"
 ROSETTA_BASE_URL = (
     f"https://api.rosetta.careevolution.com/terminology/v1/fhir/{FHIR_VERSION}"
 )
 ROSETTA_PAGE_SIZE = 250
 
 
 class RosettaValuesetProvider:
-    def __init__(self, logger: Any, api_key: str):
-        self._logger = logger
+    """
+    A valueset provider that uses the [Rosetta terminology service](https://rosetta.careevolution.com).
+    """
+
+    def __init__(self, api_key: str):
+        """
+        Creates a new instance of the RosettaValuesetProvider class.
+
+        ## Parameters
+
+        - `api_key`: The API key to use when making requests to the Rosetta terminology service.
+        """
         self._api_key = api_key
+        self._logger = get_logger().getChild(self.__class__.__name__)
 
     def _get_valueset_url(
         self,
         name: Optional[str] = None,
         scope: Optional[str] = None,
         page_number: int = 0,
     ) -> str:
         extension = ""
         name_param = ""
 
         if scope is None and name is None:
-            raise ValueError("Either scope or name must be provided")
+            raise CqlPyValueError("Either scope or name must be provided")
 
         if scope:
             extension = f"&extension.scope={scope}"
         if name:
             valueset_id = urllib.parse.quote_plus(name)
             name_param = f"name={valueset_id}"
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/scripts/fhir_map_generator.py` & `cqlpy-0.3.0/cqlpy/_internal/scripts/fhir_map_generator.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/any.py` & `cqlpy-0.3.0/cqlpy/_internal/types/any.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 _FhirJsonType = TypeVar("_FhirJsonType", bound=object)
 _CqlAnyType = TypeVar("_CqlAnyType")
 
 
 class CqlAny(Generic[_FhirJsonType, _CqlAnyType], metaclass=ABCMeta):
     """
-    All Cql types inherit from the CqlAny base class.
+    All CQL types inherit from the CqlAny base class. This class cannot be instantiated.
+
+    [Specification](http://cql.hl7.org/N1/09-b-cqlreference.html#any)
     """
 
     def __hash__(self) -> int:
         return hash(self.value)
 
     def __str__(self) -> str:
         return str(self.value)
@@ -58,38 +60,68 @@
 
         return False
 
     @property
     @abstractmethod
     def value(self) -> _CqlAnyType:
         """
-        A representation of the Cql type as a python type that is useful for comparison operations.
+        A representation of the CQL type as a python type that is useful for comparison operations.
         """
         pass
 
     @classmethod
     @abstractmethod
     def parse_fhir_json(
         self,
         fhir_json: _FhirJsonType,
         subtype: Optional[Type["CqlAny"]] = None,
     ) -> "CqlAny":
         """
-        This method will instatiate the instance with the appropriate state based on snippet of FHIR represented as an object.
-        The object should be in the format that would appear in FHIR json.
-        This method returns a reference to the instance to support one line syntax such as: return my_cql_string.parse_fhir_json("foo")
+        Instatiates the instance with the appropriate state based on snippet of FHIR.
+
+        ## Parameters
+
+        - `fhir_json`: A snippet of FHIR. The type of this parameter is determined by the type of the CqlAny instance, but is usually a `dict`.
+        - `subtype`: The `CqlAny` child type for generic types. If this is not provided, the type will be inferred from the snippet.
+
+        ## Usage
+
+        ```python
+        String.parse_fhir_json("foo")
+        Code.parse_fhir_json({"code": "foo", "system": "bar"})
+        List.parse_fhir_json(["1", "2", "3"], subtype=String)
+        ```
+
+        ## Returns
+
+        A new instance of the `CqlAny` type.
         """
         pass
 
     @classmethod
     @abstractmethod
     def parse_cql(
         self,
         cql: str,
         subtype: Optional[Type["CqlAny"]] = None,
     ) -> "CqlAny":
         """
-        This method will instatiate the instance with the appropriate state based on snippet of CQL represented as a string.
-        This method returns a reference to the instance to support one line syntax such as: return my_cql_string.parse_cql("foo")
-        This method will generally be called from the constructor so that the type can be instantiated in one line: return CqlString("foo")
+        Instatiates the instance with the appropriate state based on snippet of CQL represented as a string.
+
+        ## Parameters
+
+        - `cql`: The snippet of CQL to parse.
+        - `subtype`: The `CqlAny` child type for generic types. If this is not provided, the type will be inferred from the snippet.
+
+        ## Usage
+
+        ```python
+        String.parse_cql("foo")
+        Integer.parse_cql("1")
+        List.parse_cql("{1, 2, 3}", subtype=Integer)
+        ```
+
+        ## Returns
+
+        A new instance of the `CqlAny` type.
         """
         pass
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/boolean.py` & `cqlpy-0.3.0/cqlpy/_internal/types/boolean.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,31 @@
-from typing import Optional, Type
+from typing import Optional, Type, Union
 from cqlpy._internal.exceptions import CqlParseError
 from cqlpy._internal.types.any import CqlAny
 
 
 class Boolean(CqlAny[str, bool], int):
-    def __init__(self, value: bool):
-        self.__value = value
+    """
+    Represents the CQL Boolean type.
+
+    [Specification](http://cql.hl7.org/N1/09-b-cqlreference.html#boolean-1)
+    """
+
+    def __init__(self, value: Union[bool, "Boolean"]):
+        """
+        Creates a new Boolean.
+
+        ## Parameters
+
+        - `value`: The value of the Boolean.
+        """
+        if isinstance(value, Boolean):
+            self.__value = value.value
+        else:
+            self.__value = value
 
     @property
     def value(self) -> bool:
         return self.__value
 
     def __int__(self) -> int:
         return int(self.value)
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/code.py` & `cqlpy-0.3.0/cqlpy/_internal/types/code_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,48 @@
-from typing import Optional, Any, Union, Type
+from typing import Optional, Type
 
 from cqlpy._internal.types.any import CqlAny
-from cqlpy._internal.types.code_system import CodeSystem
 
 
-class Code(
-    CqlAny[
-        dict[str, Any],
-        tuple[Union[str, CodeSystem, None], Optional[str], Optional[str]],
-    ]
-):
+class CodeSystem(CqlAny[object, tuple[Optional[str], Optional[str]]]):
+    """
+    A pointer to an externally-defined code system.
+
+    [Specification](http://cql.hl7.org/N1/09-b-cqlreference.html#codesystem)
+    """
+
     def __init__(
         self,
-        system: Union[str, CodeSystem, None] = None,
-        code: Optional[str] = None,
-        display: Optional[str] = None,
+        id: Optional[str] = None,
         version: Optional[str] = None,
     ):
-        self.code = code
-        self.display = display
-        self.system = system
+        """
+        Creates a new CodeSystem.
+
+        ## Parameters
+
+        - `id`: The globally-unique id of the CodeSystem.
+        - `version`: The version of the CodeSystem.
+        """
+        self.id = id
         self.version = version
 
     def __str__(self) -> str:
-        return (
-            "code:"
-            + str(self.code)
-            + ", display:"
-            + str(self.display)
-            + ", system:"
-            + str(self.system)
-        )
+        return "id:" + str(self.id) + ", version:" + str(self.version)
 
     @property
-    def value(
-        self,
-    ) -> tuple[Union[str, CodeSystem, None], Optional[str], Optional[str]]:
-        return self.system, self.code, self.version
+    def value(self) -> tuple[Optional[str], Optional[str]]:
+        return self.id, self.version
 
     @classmethod
-    def parse_cql(cls, cql: str, subtype: Optional[Type[CqlAny]] = None) -> "Code":
+    def parse_cql(
+        cls, cql: str, subtype: Optional[Type[CqlAny]] = None
+    ) -> "CodeSystem":
         return cls()
 
     @classmethod
     def parse_fhir_json(
         cls,
-        fhir_json: dict[str, Any],
+        fhir_json: object,
         subtype: Optional[Type["CqlAny"]] = None,
-    ) -> "Code":
-        code = fhir_json["code"] if "code" in fhir_json else ""
-        display = fhir_json["display"] if "display" in fhir_json else ""
-        system = fhir_json["system"] if "system" in fhir_json else ""
-        version = fhir_json["version"] if "version" in fhir_json else ""
-
-        return cls(
-            system=system,
-            code=code,
-            display=display,
-            version=version,
-        )
+    ) -> "CodeSystem":
+        return cls()
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/concept.py` & `cqlpy-0.3.0/cqlpy/_internal/types/concept.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,48 +5,63 @@
 
 
 class Concept(CqlAny[dict[str, list[dict[str, str]]], list[Code]]):
     """
     Concept represents a FHIR codeable concept as a list of Code
     The FHIR codeable concept will be represented in json following the pattern of the following example:
 
+    ```python
     {
         'coding': [
-                    {
-                        'system': 'http://anthem.com/codes/Facets/DiagnosisCode',
-                        'code': '78099',
-                        'display': 'Other general symptoms',
-                        'userSelected': True
-                    },
-                    {
-                        'system': 'http://fhir.carevolution.com/codes/z-ICD9-DONOTUSE/DiagnosisCode',
-                        'version': 'LEGACY',
-                        'code': '78099',
-                        'display': 'Other general symptoms',
-                        'userSelected': False
-                    },
-                    {
-                        'system': 'http://hl7.org/fhir/sid/icd-9-cm',
-                        'code': '780.99',
-                        'display':
-                        'Other general symptoms',
-                        'userSelected': False
-                    },
-                    {
-                        'system': 'http://fhir.carevolution.com/codes/ICD9/DiagnosisCode',
-                        'code': '78099',
-                        'display': 'Other general symptoms',
-                        'userSelected': False
-                    }
-                ]
+            {
+                'system': 'http://anthem.com/codes/Facets/DiagnosisCode',
+                'code': '78099',
+                'display': 'Other general symptoms',
+                'userSelected': True
+            },
+            {
+                'system': 'http://fhir.carevolution.com/codes/z-ICD9-DONOTUSE/DiagnosisCode',
+                'version': 'LEGACY',
+                'code': '78099',
+                'display': 'Other general symptoms',
+                'userSelected': False
+            },
+            {
+                'system': 'http://hl7.org/fhir/sid/icd-9-cm',
+                'code': '780.99',
+                'display':
+                'Other general symptoms',
+                'userSelected': False
+            },
+            {
+                'system': 'http://fhir.carevolution.com/codes/ICD9/DiagnosisCode',
+                'code': '78099',
+                'display': 'Other general symptoms',
+                'userSelected': False
+            }
+        ]
     }
+    ```
+
+    [Specification](http://cql.hl7.org/09-b-cqlreference.html#concept-1)
     """
 
-    def __init__(self, codes: list = []):
-        self.codes = codes
+    def __init__(self, codes: Optional[list[Code]] = None):
+        """
+        Creates a new Concept.
+
+        ## Parameters
+
+        - `codes`: The `Code` list which comprises the `Concept`.
+        """
+        if codes is None:
+            self.codes = []
+        else:
+            self.codes = codes
+
         self.display = ""
 
     def __str__(self) -> str:
         return "display= , codes = " + str([str(code) for code in self.codes])
 
     @property
     def value(self) -> list[Code]:
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/datetime.py` & `cqlpy-0.3.0/cqlpy/_internal/types/datetime.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,43 @@
 from datetime import datetime
 from typing import Optional, Type
 
 from cqlpy._internal.types.any import CqlAny
 
 
 class DateTime(CqlAny[object, datetime]):
+    """
+    Represents a CQL datetime.
+
+    [Specification](http://cql.hl7.org/09-b-cqlreference.html#datetime)
+    """
+
     def __init__(
         self,
         year: Optional[int] = None,
         month: Optional[int] = None,
         day: Optional[int] = None,
         hour: Optional[int] = None,
         minute: Optional[int] = None,
         second: Optional[int] = None,
         millisecond: Optional[int] = None,
     ):
+        """
+        Creates a new DateTime.
+
+        ## Parameters
+
+        - `year`: The year of the DateTime.
+        - `month`: The month of the DateTime.
+        - `day`: The day of the DateTime.
+        - `hour`: The hour of the DateTime.
+        - `minute`: The minute of the DateTime.
+        - `second`: The second of the DateTime.
+        - `millisecond`: The millisecond of the DateTime.
+        """
         self.year = year
         self.month = month
         self.day = day
         self.hour = hour
         self.minute = minute
         self.second = second
         self.millisecond = millisecond
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/decimal.py` & `cqlpy-0.3.0/cqlpy/_internal/types/decimal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 from cqlpy._internal.types.any import CqlAny
 from typing import Union, Optional, Type
 
 
 class Decimal(CqlAny[Union[str, float, int], float], float):
+    """
+    Represents a CQL decimal.
+
+    [Specification](http://cql.hl7.org/09-b-cqlreference.html#decimal-1)
+    """
+
     def __init__(self, value: Union[str, float, int]):
+        """
+        Creates a new Decimal.
+
+        ## Parameters
+
+        - `value`: The value of the Decimal.
+        """
         self.__value = float(value)
 
     def __repr__(self) -> str:
         return f"Decimal({self.value})"
 
     def __new__(cls, value: Union[str, float, int]):
         return float.__new__(cls, value)
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/integer.py` & `cqlpy-0.3.0/cqlpy/_internal/types/integer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 from typing import Union, Optional, Type
 
 from cqlpy._internal.types.any import CqlAny
 
 
 class Integer(CqlAny[Union[str, int], int], int):
+    """
+    Represents a CQL integer.
+
+    [Specification](http://cql.hl7.org/09-b-cqlreference.html#integer-1)
+    """
+
     def __init__(self, value: Union[str, int]):
+        """
+        Creates a new Integer.
+
+        ## Parameters
+
+        - `value`: The value of the Integer.
+        """
         self.__value = int(value)
 
     @property
     def value(self) -> int:
         return self.__value
 
     def __int__(self) -> int:
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/interval.py` & `cqlpy-0.3.0/cqlpy/_internal/types/interval.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from cqlpy._internal.types.any import CqlAny
 from cqlpy._internal.types.date import Date
 from cqlpy._internal.types.datetime import DateTime
 from cqlpy._internal.types.decimal import Decimal
 from cqlpy._internal.types.integer import Integer
 
+from cqlpy._internal.exceptions import CqlPyValueError
+
 
 IntervalBoundType = TypeVar(
     "IntervalBoundType", bound=Union[DateTime, Date, Integer, Decimal]
 )
 
 
 def _infer_generic_value(value: str) -> Union[DateTime, Date, Integer, Decimal]:
@@ -29,36 +31,57 @@
         pass
 
     try:
         return Decimal(value)
     except ValueError:
         pass
 
-    raise ValueError(f"Could not infer type for {value}")
+    raise CqlPyValueError(f"Could not infer type for {value}")
 
 
 class Interval(
     Generic[IntervalBoundType],
     CqlAny[
         dict[str, Any],
         tuple[
             Optional[IntervalBoundType],
             Optional[bool],
             Optional[IntervalBoundType],
             Optional[bool],
         ],
     ],
 ):
+    """
+    Specifies a range of values. The bounds of the interval may be open or closed.
+    The bounds of the interval must be the same type and may be one of `DateTime`, `Date`, `Integer`, or `Decimal`.
+    """
+
     def __init__(
         self,
         low: Optional[IntervalBoundType] = None,
         low_closed: Optional[bool] = None,
         high: Optional[IntervalBoundType] = None,
         high_closed: Optional[bool] = None,
     ):
+        """
+        Creates a new `Interval` with the specified bounds.
+
+        ## Parameters
+
+        - `low`: The lower bound of the interval.
+        - `low_closed`: Whether the lower bound is closed.
+        - `high`: The upper bound of the interval.
+        - `high_closed`: Whether the upper bound is closed.
+
+        ## Usage
+
+        ```python
+        Interval(1, True, 10, False)
+        ```
+        """
         self.low = low
         self.low_closed = low_closed
         self.high = high
         self.high_closed = high_closed
 
     def __str__(self) -> str:
         return (
@@ -97,17 +120,17 @@
             low = _infer_generic_value(low_value)
             high = _infer_generic_value(high_value)
 
         low_closed = cql[:1] == "["
         high_closed = cql[-1] == "]"
 
         return cls(
-            low=low,
+            low=low,  # type: ignore  # Inferred generics have unclear usage.
             low_closed=low_closed,
-            high=high,
+            high=high,  # type: ignore  # Inferred generics have unclear usage.
             high_closed=high_closed,
         )
 
     @classmethod
     def parse_fhir_json(
         cls,
         fhir_json: dict[str, Any],
@@ -128,12 +151,12 @@
         else:
             high = low
 
         low_closed = True
         high_closed = True
 
         return cls(
-            low=low,
+            low=low,  # type: ignore  # Inferred generics have unclear usage.
             low_closed=low_closed,
-            high=high,
+            high=high,  # type: ignore  # Inferred generics have unclear usage.
             high_closed=high_closed,
         )
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/list.py` & `cqlpy-0.3.0/cqlpy/_internal/types/list.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,16 +39,18 @@
         return self.__value
 
     @classmethod
     def parse_fhir_json(
         cls,
         fhir_json: list[Any],
         subtype: Optional[Type[CqlAny]] = None,
-    ) -> "List":
+    ) -> "List[_ListItemType]":
         type_ = subtype or String
         return cls([type_.parse_fhir_json(item) for item in fhir_json])
 
     @classmethod
-    def parse_cql(cls, cql: str, subtype: Optional[Type[CqlAny]] = None) -> "List":
+    def parse_cql(
+        cls, cql: str, subtype: Optional[Type[CqlAny]] = None
+    ) -> "List[_ListItemType]":
         type_ = subtype or String
         stripped_cql = cql.strip("{}")
         return cls([type_.parse_cql(item.strip()) for item in stripped_cql.split(",")])
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/quantity.py` & `cqlpy-0.3.0/cqlpy/_internal/types/quantity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 from typing import Optional, Type
 from cqlpy._internal.types.any import CqlAny
 
 
 class Quantity(CqlAny[object, Optional[float]]):
+    """
+    Represents a CQL quantity, which is a numeric value with a unit of measure.
+
+    [Specification](http://cql.hl7.org/09-b-cqlreference.html#quantity)
+    """
+
     def __init__(self, value: Optional[float] = None, unit: Optional[str] = None):
+        """
+        Creates a new Quantity.
+
+        ## Parameters
+
+        - `value`: The numeric count of the Quantity.
+        - `unit`: The unit of measure of the Quantity.
+        """
         self._value = value
         self._unit = unit
 
     def __str__(self) -> str:
         if self._value is None:
             return self._unit or ""
         return str(self._value) + " " + (self._unit or "")
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/string.py` & `cqlpy-0.3.0/cqlpy/_internal/types/string.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 from typing import Optional, Type
 from cqlpy._internal.types.any import CqlAny
 
 
 class String(CqlAny[str, str], str):
+    """
+    Represents a CQL string.
+
+    [Specification](http://cql.hl7.org/09-b-cqlreference.html#string-1)
+    """
+
     def __init__(self, value: str):
+        """
+        Creates a new String.
+
+        ## Parameters
+
+        - `value`: The value of the String.
+        """
         self.__value = value
 
     def __hash__(self) -> int:
         return hash(self.value)
 
     def __new__(cls, value: str):
         return str.__new__(cls, value)
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/valueset.py` & `cqlpy-0.3.0/cqlpy/_internal/types/code.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,77 @@
-from typing import Any, Optional, Type
+from typing import Optional, Any, Union, Type
+
 from cqlpy._internal.types.any import CqlAny
-from cqlpy._internal.types.code import Code
+from cqlpy._internal.types.code_system import CodeSystem
+
+
+class Code(
+    CqlAny[
+        dict[str, Any],
+        tuple[Union[str, CodeSystem, None], Optional[str], Optional[str]],
+    ]
+):
+    """
+    Represents CQL terminology codes.
 
+    [Specification](http://cql.hl7.org/N1/09-b-cqlreference.html#code-1)
+    """
 
-class Valueset(CqlAny[dict[str, Any], list[Code]]):
     def __init__(
         self,
-        valueset_id: Optional[str] = None,
-        name: Optional[str] = None,
+        system: Union[str, CodeSystem, None] = None,
+        code: Optional[str] = None,
+        display: Optional[str] = None,
         version: Optional[str] = None,
-        use_context: Optional[str] = None,
-        codes: Optional[list[Code]] = None,
     ):
-        self.id = valueset_id
-        self.name = name
+        """
+        Creates a new Code.
+
+        ## Parameters
+
+        - `system`: The system of the Code.
+        - `code`: The code of the Code.
+        - `display`: The display of the Code.
+        - `version`: The version of the Code.
+        """
+        self.code = code
+        self.display = display
+        self.system = system
         self.version = version
-        self.use_context = use_context
-        self.codes: list[Code] = codes or []
 
     def __str__(self) -> str:
         return (
-            "id:"
-            + (self.id or "")
-            + ", version:"
-            + (self.version or "")
-            + ", codes:"
-            + str([str(code) for code in self.codes])
+            "code:"
+            + str(self.code)
+            + ", display:"
+            + str(self.display)
+            + ", system:"
+            + str(self.system)
         )
 
     @property
-    def value(self) -> list[Code]:
-        return self.codes
+    def value(
+        self,
+    ) -> tuple[Union[str, CodeSystem, None], Optional[str], Optional[str]]:
+        return self.system, self.code, self.version
 
     @classmethod
-    def parse_cql(cls, cql: str, subtype: Optional[Type[CqlAny]] = None) -> "Valueset":
-        valueset_id = ""
-        version = ""
-        name = ""
-
-        return cls(
-            valueset_id=valueset_id,
-            name=name,
-            version=version,
-        )
+    def parse_cql(cls, cql: str, subtype: Optional[Type[CqlAny]] = None) -> "Code":
+        return cls()
 
     @classmethod
     def parse_fhir_json(
         cls,
         fhir_json: dict[str, Any],
         subtype: Optional[Type["CqlAny"]] = None,
-    ) -> "Valueset":
-        version: str = fhir_json["version"]
-        name: str = fhir_json["name"]
-        includes: list[dict[str, Any]] = fhir_json["compose"]["include"]
-
-        codes = [
-            Code(
-                system=include.get("system", ""),
-                code=concept["code"],
-                display=concept.get("display", ""),
-                version=include.get("version", ""),
-            )
-            for include in includes
-            for concept in include["concept"]
-        ]
+    ) -> "Code":
+        code = fhir_json["code"] if "code" in fhir_json else ""
+        display = fhir_json["display"] if "display" in fhir_json else ""
+        system = fhir_json["system"] if "system" in fhir_json else ""
+        version = fhir_json["version"] if "version" in fhir_json else ""
 
         return cls(
-            valueset_id="",
-            name=name,
+            system=system,
+            code=code,
+            display=display,
             version=version,
-            codes=codes,
         )
```

### Comparing `cqlpy-0.2.7/cqlpy/_internal/types/valueset_scope.py` & `cqlpy-0.3.0/cqlpy/_internal/types/valueset_scope.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.7/cqlpy/operators.py` & `cqlpy-0.3.0/cqlpy/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cqlpy._internal.operators.comparison.less import less
 from cqlpy._internal.operators.comparison.less_or_equal import less_or_equal
 from cqlpy._internal.operators.comparison.not_equal import not_equal
 from cqlpy._internal.operators.cql_in import cql_in
 from cqlpy._internal.operators.date_time.add import add
 from cqlpy._internal.operators.date_time.after import after
 from cqlpy._internal.operators.date_time.before import before
-from cqlpy._internal.operators.date_time.calculate_age_at import calculate_age_at
+from cqlpy._internal.operators.clinical.calculate_age_at import calculate_age_at
 from cqlpy._internal.operators.date_time.date_time_precision import DateTimePrecision
 from cqlpy._internal.operators.date_time.difference_between import difference_between
 from cqlpy._internal.operators.date_time.duration_between import duration_between
 from cqlpy._internal.operators.date_time.same_or_before import same_or_before
 from cqlpy._internal.operators.date_time.subtract import subtract
 from cqlpy._internal.operators.interval.collapse import collapse
 from cqlpy._internal.operators.interval.end import end
```

### Comparing `cqlpy-0.2.7/cqlpy/types.py` & `cqlpy-0.3.0/cqlpy/types.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.7/pyproject.toml` & `cqlpy-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "John Wyderko <john@careevolution.com>",
   "Jeremy Fortune <jeremy@careevolution.com>",
 ]
 description = "Tooling to execute CQL-like Python against FHIR resources."
 license = "MIT"
 name = "cqlpy"
 readme = "README.md"
-version = "0.2.7"
+version = "0.3.0"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "^23.3.0"}
@@ -19,10 +19,11 @@
 notebook = "^6.5.3"
 types-python-dateutil = "^2.8.19.11"
 types-requests = "^2.30.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 
+
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.4.0"]
```


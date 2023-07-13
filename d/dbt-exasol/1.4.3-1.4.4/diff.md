# Comparing `tmp/dbt_exasol-1.4.3.tar.gz` & `tmp/dbt_exasol-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_exasol-1.4.3.tar", max compression
+gzip compressed data, was "dbt_exasol-1.4.4.tar", max compression
```

## Comparing `dbt_exasol-1.4.3.tar` & `dbt_exasol-1.4.4.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rwxr-xr-x   0        0        0    35148 2021-12-30 07:56:19.472113 dbt_exasol-1.4.3/LICENSE
--rw-r--r--   0        0        0     2504 2023-06-12 16:14:26.080747 dbt_exasol-1.4.3/README.md
--rw-r--r--   0        0        0       65 2023-05-30 21:28:56.423110 dbt_exasol-1.4.3/dbt/__init__.py
--rw-r--r--   0        0        0       65 2023-05-30 21:28:56.427667 dbt_exasol-1.4.3/dbt/adapters/__init__.py
--rw-r--r--   0        0        0      508 2023-05-30 21:33:28.065894 dbt_exasol-1.4.3/dbt/adapters/exasol/__init__.py
--rw-r--r--   0        0        0       19 2023-06-13 06:57:57.600762 dbt_exasol-1.4.3/dbt/adapters/exasol/__version__.py
--rw-r--r--   0        0        0     3675 2023-06-12 16:35:19.474496 dbt_exasol-1.4.3/dbt/adapters/exasol/column.py
--rw-r--r--   0        0        0    10688 2023-06-12 16:35:19.475379 dbt_exasol-1.4.3/dbt/adapters/exasol/connections.py
--rw-r--r--   0        0        0     2806 2023-06-12 16:35:19.476101 dbt_exasol-1.4.3/dbt/adapters/exasol/impl.py
--rw-r--r--   0        0        0     1959 2023-06-12 16:35:19.476752 dbt_exasol-1.4.3/dbt/adapters/exasol/relation.py
--rw-r--r--   0        0        0       65 2023-05-30 21:28:56.417362 dbt_exasol-1.4.3/dbt/include/__init__.py
--rw-r--r--   0        0        0       52 2023-05-30 21:28:56.419671 dbt_exasol-1.4.3/dbt/include/exasol/__init__.py
--rwxr-xr-x   0        0        0      236 2021-12-30 07:56:19.481658 dbt_exasol-1.4.3/dbt/include/exasol/__pycache__/__init__.cpython-37.pyc
--rwxr-xr-x   0        0        0       74 2021-12-30 07:56:19.482361 dbt_exasol-1.4.3/dbt/include/exasol/dbt_project.yml
--rw-r--r--   0        0        0     6240 2023-06-12 16:35:19.477331 dbt_exasol-1.4.3/dbt/include/exasol/macros/adapters.sql
--rw-r--r--   0        0        0      673 2023-05-30 21:30:19.492885 dbt_exasol-1.4.3/dbt/include/exasol/macros/apply_grants.sql
--rwxr-xr-x   0        0        0     1458 2023-05-30 21:30:19.489001 dbt_exasol-1.4.3/dbt/include/exasol/macros/catalog.sql
--rw-r--r--   0        0        0     4239 2023-05-30 21:30:19.462558 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/incremental.sql
--rw-r--r--   0        0        0      259 2023-05-30 21:30:19.453074 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/incremental_strategies.sql
--rw-r--r--   0        0        0     1025 2023-06-12 16:35:19.477809 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/merge.sql
--rwxr-xr-x   0        0        0      470 2023-05-30 21:30:19.450464 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/seed.sql
--rw-r--r--   0        0        0     8044 2023-05-30 21:30:19.464735 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/snapshot.sql
--rw-r--r--   0        0        0      748 2023-05-30 21:30:19.455665 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/snapshot_merge.sql
--rw-r--r--   0        0        0     3258 2023-05-30 21:30:19.457925 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/strategies.sql
--rw-r--r--   0        0        0     3524 2023-05-30 21:30:19.460381 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/table.sql
--rw-r--r--   0        0        0      178 2023-05-30 21:30:19.480626 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/any_value.sql
--rw-r--r--   0        0        0       85 2023-05-30 21:30:19.482423 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/bool_or.sql
--rw-r--r--   0        0        0      469 2023-05-30 21:30:19.466872 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/dateadd.sql
--rw-r--r--   0        0        0      441 2023-05-30 21:30:19.474475 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/datediff.sql
--rw-r--r--   0        0        0      130 2023-05-30 21:30:19.478733 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/hash.sql
--rw-r--r--   0        0        0      381 2023-05-30 21:30:19.484622 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/last_day.sql
--rw-r--r--   0        0        0      415 2023-05-30 21:30:19.471787 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/listagg.sql
--rw-r--r--   0        0        0      775 2023-05-30 21:30:19.476801 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/safe_cast.sql
--rw-r--r--   0        0        0      165 2023-05-30 21:30:19.486659 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/split_part.sql
--rw-r--r--   0        0        0      519 2023-06-12 16:35:19.478151 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/timestamps.sql
--rw-r--r--   0        0        0      374 2023-05-31 15:48:24.596080 dbt_exasol-1.4.3/dbt/include/exasol/profile_template.yml
--rw-r--r--   0        0        0      906 2023-06-13 06:57:43.652646 dbt_exasol-1.4.3/pyproject.toml
--rw-r--r--   0        0        0      606 2023-05-30 21:28:56.447674 dbt_exasol-1.4.3/tests/conftest.py
--rw-r--r--   0        0        0     7729 2023-05-30 21:28:56.484385 dbt_exasol-1.4.3/tests/functional/adapter/expected_catalog.py
--rw-r--r--   0        0        0     1438 2023-05-30 21:28:56.450549 dbt_exasol-1.4.3/tests/functional/adapter/files.py
--rw-r--r--   0        0        0      521 2023-05-30 21:28:56.489680 dbt_exasol-1.4.3/tests/functional/adapter/fixtures.py
--rw-r--r--   0        0        0      676 2023-06-12 16:35:19.481459 dbt_exasol-1.4.3/tests/functional/adapter/query_comment_tests/test_query_comment.py
--rw-r--r--   0        0        0      190 2023-06-12 16:35:19.481812 dbt_exasol-1.4.3/tests/functional/adapter/relations/test_changing_relation_type.py
--rw-r--r--   0        0        0     2708 2023-05-30 21:28:56.452648 dbt_exasol-1.4.3/tests/functional/adapter/test_basic.py
--rw-r--r--   0        0        0     1255 2023-05-30 21:28:56.455200 dbt_exasol-1.4.3/tests/functional/adapter/test_concurrency.py
--rw-r--r--   0        0        0    12762 2023-05-30 21:28:56.486846 dbt_exasol-1.4.3/tests/functional/adapter/test_docs_generate.py
--rw-r--r--   0        0        0      457 2023-06-12 13:34:48.744670 dbt_exasol-1.4.3/tests/functional/adapter/test_ephemeral.py
--rw-r--r--   0        0        0     2068 2023-05-30 21:28:56.476133 dbt_exasol-1.4.3/tests/functional/adapter/test_failing_test.py
--rw-r--r--   0        0        0     1350 2023-06-12 16:35:19.482380 dbt_exasol-1.4.3/tests/functional/adapter/utils/data_types/test_data_types.py
--rw-r--r--   0        0        0      591 2023-05-30 21:28:56.463459 dbt_exasol-1.4.3/tests/functional/adapter/utils/data_types/test_type_bigint.py
--rw-r--r--   0        0        0     1167 2023-06-12 16:35:19.482708 dbt_exasol-1.4.3/tests/functional/adapter/utils/test_timestamps.py
--rw-r--r--   0        0        0    12212 2023-06-12 16:35:19.483126 dbt_exasol-1.4.3/tests/functional/adapter/utils/test_utils.py
--rw-r--r--   0        0        0    14496 2023-05-30 21:28:56.468780 dbt_exasol-1.4.3/tests/functional/adapter/utils/utils_fixtures.py
--rw-r--r--   0        0        0      924 2023-06-12 16:35:19.483568 dbt_exasol-1.4.3/tests/functional/test_grants.py
--rw-r--r--   0        0        0     8096 2023-05-30 21:28:56.496086 dbt_exasol-1.4.3/tests/functional/test_incremental.py
--rw-r--r--   0        0        0     1465 2023-05-30 21:28:56.492771 dbt_exasol-1.4.3/tests/functional/test_issues.py
--rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 dbt_exasol-1.4.3/PKG-INFO
+-rwxr-xr-x   0        0        0    35148 2021-12-30 07:56:19.472113 dbt_exasol-1.4.4/LICENSE
+-rw-r--r--   0        0        0     2504 2023-06-12 16:14:26.080747 dbt_exasol-1.4.4/README.md
+-rw-r--r--   0        0        0       65 2023-05-30 21:28:56.423110 dbt_exasol-1.4.4/dbt/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-30 21:28:56.427667 dbt_exasol-1.4.4/dbt/adapters/__init__.py
+-rw-r--r--   0        0        0      508 2023-05-30 21:33:28.065894 dbt_exasol-1.4.4/dbt/adapters/exasol/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-13 13:43:37.649099 dbt_exasol-1.4.4/dbt/adapters/exasol/__version__.py
+-rw-r--r--   0        0        0     3675 2023-07-13 13:43:37.649751 dbt_exasol-1.4.4/dbt/adapters/exasol/column.py
+-rw-r--r--   0        0        0    10688 2023-07-13 13:43:37.650303 dbt_exasol-1.4.4/dbt/adapters/exasol/connections.py
+-rw-r--r--   0        0        0     2806 2023-07-13 13:43:37.650795 dbt_exasol-1.4.4/dbt/adapters/exasol/impl.py
+-rw-r--r--   0        0        0     1959 2023-07-13 13:43:37.651214 dbt_exasol-1.4.4/dbt/adapters/exasol/relation.py
+-rw-r--r--   0        0        0       65 2023-05-30 21:28:56.417362 dbt_exasol-1.4.4/dbt/include/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-30 21:28:56.419671 dbt_exasol-1.4.4/dbt/include/exasol/__init__.py
+-rwxr-xr-x   0        0        0      236 2021-12-30 07:56:19.481658 dbt_exasol-1.4.4/dbt/include/exasol/__pycache__/__init__.cpython-37.pyc
+-rwxr-xr-x   0        0        0       74 2021-12-30 07:56:19.482361 dbt_exasol-1.4.4/dbt/include/exasol/dbt_project.yml
+-rw-r--r--   0        0        0     6582 2023-07-13 13:43:37.651628 dbt_exasol-1.4.4/dbt/include/exasol/macros/adapters.sql
+-rw-r--r--   0        0        0      673 2023-05-30 21:30:19.492885 dbt_exasol-1.4.4/dbt/include/exasol/macros/apply_grants.sql
+-rwxr-xr-x   0        0        0     1458 2023-05-30 21:30:19.489001 dbt_exasol-1.4.4/dbt/include/exasol/macros/catalog.sql
+-rw-r--r--   0        0        0     4239 2023-05-30 21:30:19.462558 dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/incremental.sql
+-rw-r--r--   0        0        0      259 2023-05-30 21:30:19.453074 dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0        0        0     1025 2023-07-13 13:43:37.652069 dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/merge.sql
+-rwxr-xr-x   0        0        0      470 2023-05-30 21:30:19.450464 dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/seed.sql
+-rw-r--r--   0        0        0     8044 2023-05-30 21:30:19.464735 dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/snapshot.sql
+-rw-r--r--   0        0        0      748 2023-05-30 21:30:19.455665 dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0        0        0     3258 2023-05-30 21:30:19.457925 dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/strategies.sql
+-rw-r--r--   0        0        0     3524 2023-05-30 21:30:19.460381 dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/table.sql
+-rw-r--r--   0        0        0      178 2023-05-30 21:30:19.480626 dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/any_value.sql
+-rw-r--r--   0        0        0       85 2023-05-30 21:30:19.482423 dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/bool_or.sql
+-rw-r--r--   0        0        0      469 2023-05-30 21:30:19.466872 dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0      441 2023-05-30 21:30:19.474475 dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      130 2023-05-30 21:30:19.478733 dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/hash.sql
+-rw-r--r--   0        0        0      381 2023-05-30 21:30:19.484622 dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      415 2023-05-30 21:30:19.471787 dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      775 2023-05-30 21:30:19.476801 dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/safe_cast.sql
+-rw-r--r--   0        0        0      165 2023-05-30 21:30:19.486659 dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/split_part.sql
+-rw-r--r--   0        0        0      519 2023-07-13 13:43:37.652501 dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/timestamps.sql
+-rw-r--r--   0        0        0      374 2023-05-31 15:48:24.596080 dbt_exasol-1.4.4/dbt/include/exasol/profile_template.yml
+-rw-r--r--   0        0        0      906 2023-07-13 13:43:37.655671 dbt_exasol-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0      606 2023-05-30 21:28:56.447674 dbt_exasol-1.4.4/tests/conftest.py
+-rw-r--r--   0        0        0     7729 2023-05-30 21:28:56.484385 dbt_exasol-1.4.4/tests/functional/adapter/expected_catalog.py
+-rw-r--r--   0        0        0     1438 2023-05-30 21:28:56.450549 dbt_exasol-1.4.4/tests/functional/adapter/files.py
+-rw-r--r--   0        0        0      521 2023-05-30 21:28:56.489680 dbt_exasol-1.4.4/tests/functional/adapter/fixtures.py
+-rw-r--r--   0        0        0      676 2023-07-13 13:43:37.656112 dbt_exasol-1.4.4/tests/functional/adapter/query_comment_tests/test_query_comment.py
+-rw-r--r--   0        0        0      190 2023-07-13 13:43:37.656509 dbt_exasol-1.4.4/tests/functional/adapter/relations/test_changing_relation_type.py
+-rw-r--r--   0        0        0     2708 2023-05-30 21:28:56.452648 dbt_exasol-1.4.4/tests/functional/adapter/test_basic.py
+-rw-r--r--   0        0        0     1255 2023-05-30 21:28:56.455200 dbt_exasol-1.4.4/tests/functional/adapter/test_concurrency.py
+-rw-r--r--   0        0        0    12762 2023-05-30 21:28:56.486846 dbt_exasol-1.4.4/tests/functional/adapter/test_docs_generate.py
+-rw-r--r--   0        0        0      457 2023-06-12 13:34:48.744670 dbt_exasol-1.4.4/tests/functional/adapter/test_ephemeral.py
+-rw-r--r--   0        0        0     2068 2023-05-30 21:28:56.476133 dbt_exasol-1.4.4/tests/functional/adapter/test_failing_test.py
+-rw-r--r--   0        0        0     1350 2023-07-13 13:43:37.657380 dbt_exasol-1.4.4/tests/functional/adapter/utils/data_types/test_data_types.py
+-rw-r--r--   0        0        0      591 2023-05-30 21:28:56.463459 dbt_exasol-1.4.4/tests/functional/adapter/utils/data_types/test_type_bigint.py
+-rw-r--r--   0        0        0     1167 2023-07-13 13:43:37.657778 dbt_exasol-1.4.4/tests/functional/adapter/utils/test_timestamps.py
+-rw-r--r--   0        0        0    12212 2023-07-13 13:43:37.658191 dbt_exasol-1.4.4/tests/functional/adapter/utils/test_utils.py
+-rw-r--r--   0        0        0    14496 2023-05-30 21:28:56.468780 dbt_exasol-1.4.4/tests/functional/adapter/utils/utils_fixtures.py
+-rw-r--r--   0        0        0      924 2023-07-13 13:43:37.658516 dbt_exasol-1.4.4/tests/functional/test_grants.py
+-rw-r--r--   0        0        0     8096 2023-05-30 21:28:56.496086 dbt_exasol-1.4.4/tests/functional/test_incremental.py
+-rw-r--r--   0        0        0     1465 2023-05-30 21:28:56.492771 dbt_exasol-1.4.4/tests/functional/test_issues.py
+-rw-r--r--   0        0        0      831 2023-07-13 13:37:57.952202 dbt_exasol-1.4.4/tests/functional/test_view_comment.py
+-rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 dbt_exasol-1.4.4/PKG-INFO
```

### Comparing `dbt_exasol-1.4.3/LICENSE` & `dbt_exasol-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/README.md` & `dbt_exasol-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/adapters/exasol/column.py` & `dbt_exasol-1.4.4/dbt/adapters/exasol/column.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/adapters/exasol/connections.py` & `dbt_exasol-1.4.4/dbt/adapters/exasol/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/adapters/exasol/impl.py` & `dbt_exasol-1.4.4/dbt/adapters/exasol/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/adapters/exasol/relation.py` & `dbt_exasol-1.4.4/dbt/adapters/exasol/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/include/exasol/macros/adapters.sql` & `dbt_exasol-1.4.4/dbt/include/exasol/macros/adapters.sql`

 * *Files 5% similar despite different names*

```diff
@@ -118,16 +118,19 @@
         limit 0
     {% endcall %}
 
     {{ return(load_result('get_columns_in_query').table.columns | map(attribute='name') | list) }}
 {% endmacro %}
 
 {% macro exasol__alter_relation_comment(relation, relation_comment) -%}
-  {%- set comment = relation_comment | replace("'", '"') %}
-  COMMENT ON {{ relation.type }} {{ relation }} IS '{{ comment }}';
+  {# Comments on views are not supported outside DDL, see https://docs.exasol.com/db/latest/sql/comment.htm#UsageNotes #}
+  {%- if not relation.is_view %}
+    {%- set comment = relation_comment | replace("'", '"') %}
+    COMMENT ON {{ relation.type }} {{ relation }} IS '{{ comment }}';
+  {%- endif %}
 {% endmacro %}
 
 {% macro get_column_comment_sql(column_name, column_dict, apply_comment=false) -%}
   {% if (column_name|upper in column_dict) -%}
     {% set matched_column = column_name|upper -%}
   {% elif (column_name|lower in column_dict) -%}
     {% set matched_column = column_name|lower -%}
@@ -141,20 +144,23 @@
   {% else -%}
     {% set comment = "" -%}
   {% endif -%}
   {{ adapter.quote(column_name) }} {{ "COMMENT" if apply_comment }} IS '{{ comment }}'
 {%- endmacro %}
 
 {% macro exasol__alter_column_comment(relation, column_dict) -%}
+  {# Comments on views are not supported outside DDL, see https://docs.exasol.com/db/latest/sql/comment.htm#UsageNotes #}
+  {%- if not relation.is_view %}
     {% set query_columns = get_columns_in_query(sql) %} 
     COMMENT ON {{ relation.type }} {{ relation }} (
     {% for column_name in query_columns %}
-        {{ get_column_comment_sql(column_name, column_dict) }} {{- ',' if not loop.last }}
+      {{ get_column_comment_sql(column_name, column_dict) }} {{- ',' if not loop.last }}
     {% endfor %}
     );
+  {%- endif %}
 {% endmacro %}
 
 {% macro persist_view_column_docs(relation, sql) %}
 {%- if config.persist_column_docs() %}
 (
   {% set query_columns = get_columns_in_query(sql) %}
   {%- for column_name in query_columns %}
```

### Comparing `dbt_exasol-1.4.3/dbt/include/exasol/macros/apply_grants.sql` & `dbt_exasol-1.4.4/dbt/include/exasol/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/include/exasol/macros/catalog.sql` & `dbt_exasol-1.4.4/dbt/include/exasol/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/incremental.sql` & `dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/merge.sql` & `dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/snapshot.sql` & `dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/snapshot_merge.sql` & `dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/strategies.sql` & `dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/table.sql` & `dbt_exasol-1.4.4/dbt/include/exasol/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/safe_cast.sql` & `dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/safe_cast.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/timestamps.sql` & `dbt_exasol-1.4.4/dbt/include/exasol/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/pyproject.toml` & `dbt_exasol-1.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-exasol"
-version = "1.4.3"
+version = "1.4.4"
 description = "Adapter to dbt-core for warehouse Exasol"
 authors = ["Torsten Glunde <torsten.glunde@alligator-company.com>", "Ilija Kutle <ilija.kutle@alligator-company.com>"]
 homepage = "https://alligatorcompany.gitlab.io/dbt-exasol"
 repository = "https://github.com/tglunde/dbt-exasol"
 packages = [
   { include = "dbt" },
   { include = "dbt/**/*.py" },
```

### Comparing `dbt_exasol-1.4.3/tests/conftest.py` & `dbt_exasol-1.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/expected_catalog.py` & `dbt_exasol-1.4.4/tests/functional/adapter/expected_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/files.py` & `dbt_exasol-1.4.4/tests/functional/adapter/files.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/fixtures.py` & `dbt_exasol-1.4.4/tests/functional/adapter/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/query_comment_tests/test_query_comment.py` & `dbt_exasol-1.4.4/tests/functional/adapter/query_comment_tests/test_query_comment.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/test_basic.py` & `dbt_exasol-1.4.4/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/test_concurrency.py` & `dbt_exasol-1.4.4/tests/functional/adapter/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/test_docs_generate.py` & `dbt_exasol-1.4.4/tests/functional/adapter/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/test_failing_test.py` & `dbt_exasol-1.4.4/tests/functional/adapter/test_failing_test.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/utils/data_types/test_data_types.py` & `dbt_exasol-1.4.4/tests/functional/adapter/utils/data_types/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/utils/data_types/test_type_bigint.py` & `dbt_exasol-1.4.4/tests/functional/adapter/utils/data_types/test_type_bigint.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/utils/test_timestamps.py` & `dbt_exasol-1.4.4/tests/functional/adapter/utils/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/utils/test_utils.py` & `dbt_exasol-1.4.4/tests/functional/adapter/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/adapter/utils/utils_fixtures.py` & `dbt_exasol-1.4.4/tests/functional/adapter/utils/utils_fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/test_grants.py` & `dbt_exasol-1.4.4/tests/functional/test_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/test_incremental.py` & `dbt_exasol-1.4.4/tests/functional/test_incremental.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/tests/functional/test_issues.py` & `dbt_exasol-1.4.4/tests/functional/test_issues.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.3/PKG-INFO` & `dbt_exasol-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-exasol
-Version: 1.4.3
+Version: 1.4.4
 Summary: Adapter to dbt-core for warehouse Exasol
 Home-page: https://alligatorcompany.gitlab.io/dbt-exasol
 License: GPL3
 Author: Torsten Glunde
 Author-email: torsten.glunde@alligator-company.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
```


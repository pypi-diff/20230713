# Comparing `tmp/dbt-materialize-1.4.1.tar.gz` & `tmp/dbt-materialize-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-materialize-1.4.1.tar", last modified: Fri Apr 28 18:04:05 2023, max compression
+gzip compressed data, was "dbt-materialize-1.5.0.tar", last modified: Thu Jul 13 19:12:06 2023, max compression
```

## Comparing `dbt-materialize-1.4.1.tar` & `dbt-materialize-1.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     5950 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize  (1001)     5592 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/README.md
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.033542 dbt-materialize-1.4.1/dbt/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.033542 dbt-materialize-1.4.1/dbt/adapters/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.033542 dbt-materialize-1.4.1/dbt/adapters/materialize/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1159 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)      801 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/materialize/__version__.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)     3431 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/materialize/connections.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)     4104 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/materialize/impl.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1688 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/adapters/materialize/relation.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.033542 dbt-materialize-1.4.1/dbt/include/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.033542 dbt-materialize-1.4.1/dbt/include/materialize/
--rw-r--r--   0 materialize  (2000) materialize  (1001)      782 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize  (1001)      808 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/dbt_project.yml
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/dbt/include/materialize/macros/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     3862 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/adapters.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1848 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/catalog.sql
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1909 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/incremental.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1920 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/materialized_view.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     3023 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/seed.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1784 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/sink.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1828 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/source.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1933 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/table.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1960 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/test.sql
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1883 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/view.sql
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/dbt/include/materialize/macros/utils/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1016 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/dbt/include/materialize/macros/utils/listagg.sql
-drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/dbt_materialize.egg-info/
--rw-r--r--   0 materialize  (2000) materialize  (1001)     5950 2023-04-28 18:04:04.000000 dbt-materialize-1.4.1/dbt_materialize.egg-info/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1155 2023-04-28 18:04:04.000000 dbt-materialize-1.4.1/dbt_materialize.egg-info/SOURCES.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)        1 2023-04-28 18:04:04.000000 dbt-materialize-1.4.1/dbt_materialize.egg-info/dependency_links.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)       52 2023-04-28 18:04:04.000000 dbt-materialize-1.4.1/dbt_materialize.egg-info/requires.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)        4 2023-04-28 18:04:04.000000 dbt-materialize-1.4.1/dbt_materialize.egg-info/top_level.txt
--rw-r--r--   0 materialize  (2000) materialize  (1001)       38 2023-04-28 18:04:05.043542 dbt-materialize-1.4.1/setup.cfg
--rw-r--r--   0 materialize  (2000) materialize  (1001)     1768 2023-04-28 18:03:33.000000 dbt-materialize-1.4.1/setup.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     5950 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     5592 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/README.md
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/adapters/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/adapters/materialize/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1159 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      801 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/materialize/__version__.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     3431 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/materialize/connections.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     4802 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/materialize/impl.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1688 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/adapters/materialize/relation.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/include/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      729 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/include/materialize/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      782 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize  (1001)      808 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/dbt_project.yml
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/include/materialize/macros/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     4808 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/adapters.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     2222 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/catalog.sql
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1909 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/incremental.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1920 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/materialized_view.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     3023 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/seed.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1784 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/sink.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1828 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/source.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1933 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/table.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1960 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/test.sql
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1883 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/view.sql
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt/include/materialize/macros/utils/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1016 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/dbt/include/materialize/macros/utils/listagg.sql
+drwxr-xr-x   0 materialize  (2000) materialize  (1001)        0 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/dbt_materialize.egg-info/
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     5950 2023-07-13 19:12:06.000000 dbt-materialize-1.5.0/dbt_materialize.egg-info/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1155 2023-07-13 19:12:06.000000 dbt-materialize-1.5.0/dbt_materialize.egg-info/SOURCES.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)        1 2023-07-13 19:12:06.000000 dbt-materialize-1.5.0/dbt_materialize.egg-info/dependency_links.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)       52 2023-07-13 19:12:06.000000 dbt-materialize-1.5.0/dbt_materialize.egg-info/requires.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)        4 2023-07-13 19:12:06.000000 dbt-materialize-1.5.0/dbt_materialize.egg-info/top_level.txt
+-rw-r--r--   0 materialize  (2000) materialize  (1001)       38 2023-07-13 19:12:06.656389 dbt-materialize-1.5.0/setup.cfg
+-rw-r--r--   0 materialize  (2000) materialize  (1001)     1768 2023-07-13 19:11:38.000000 dbt-materialize-1.5.0/setup.py
```

### Comparing `dbt-materialize-1.4.1/PKG-INFO` & `dbt-materialize-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.4.1
+Version: 1.5.0
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `dbt-materialize-1.4.1/README.md` & `dbt-materialize-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/__init__.py` & `dbt-materialize-1.5.0/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/adapters/__init__.py` & `dbt-materialize-1.5.0/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/adapters/materialize/__init__.py` & `dbt-materialize-1.5.0/dbt/adapters/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/adapters/materialize/__version__.py` & `dbt-materialize-1.5.0/dbt/adapters/materialize/__version__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # If you bump this version, bump it in setup.py too.
-version = "1.4.1"
+version = "1.5.0"
```

### Comparing `dbt-materialize-1.4.1/dbt/adapters/materialize/connections.py` & `dbt-materialize-1.5.0/dbt/adapters/materialize/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/adapters/materialize/relation.py` & `dbt-materialize-1.5.0/dbt/adapters/materialize/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/__init__.py` & `dbt-materialize-1.5.0/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/__init__.py` & `dbt-materialize-1.5.0/dbt/include/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/dbt_project.yml` & `dbt-materialize-1.5.0/dbt/include/materialize/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/macros/adapters.sql` & `dbt-materialize-1.5.0/dbt/include/materialize/macros/adapters.sql`

 * *Files 17% similar despite different names*

```diff
@@ -16,32 +16,44 @@
 
 -- Most of these macros are direct copies of their PostgreSQL counterparts.
 -- See: https://github.com/dbt-labs/dbt-core/blob/13b18654f/plugins/postgres/dbt/include/postgres/macros/adapters.sql
 
 {% macro materialize__create_view_as(relation, sql) -%}
 
   create view {{ relation }}
+    {% set contract_config = config.get('contract') %}
+    {% if contract_config.enforced %}
+      {{exceptions.warn("Model contracts cannot be enforced in this version of the adapter (see dbt-core #7213)")}}
+    {%- endif %}
   as (
     {{ sql }}
   );
 {%- endmacro %}
 
 {% macro materialize__create_materialized_view_as(relation, sql) -%}
   {%- set cluster = config.get('cluster', target.cluster) -%}
 
   create materialized view {{ relation }}
+    {% set contract_config = config.get('contract') %}
+    {% if contract_config.enforced %}
+      {{exceptions.warn("Model contracts cannot be enforced in this version of the adapter (see dbt-core #7213)")}}
+    {%- endif %}
   {% if cluster %}
     in cluster {{ cluster }}
   {% endif %}
   as (
     {{ sql }}
   );
 {%- endmacro %}
 
 {% macro materialize__create_arbitrary_object(sql) -%}
+    {% set contract_config = config.get('contract') %}
+    {% if contract_config.enforced %}
+      {{exceptions.warn("Model contracts cannot be enforced in this version of the adapter (see dbt-core #7213)")}}
+    {%- endif %}
     {{ sql }}
 {%- endmacro %}
 
 {% macro materialize__rename_relation(from_relation, to_relation) -%}
   {% set target_name = adapter.quote_as_configured(to_relation.identifier, 'identifier') %}
   {% call statement('rename_relation') -%}
     {% if relation.type == 'view' %}
@@ -92,15 +104,21 @@
 -- In the dbt-adapter we extend the Relation class to include sinks and indexes
 {% macro materialize__list_relations_without_caching(schema_relation) %}
   {% call statement('list_relations_without_caching', fetch_result=True) -%}
     select
         d.name as database,
         s.name as schema,
         o.name,
-        case when o.type = 'materialized-view' then 'materializedview' else o.type end as type
+        case when o.type = 'materialized-view' then 'materializedview'
+             else o.type
+        end as type
     from mz_objects o
+    left join mz_sources so on o.id = so.id
     join mz_schemas s on o.schema_id = s.id and s.name = '{{ schema_relation.schema }}'
     join mz_databases d on s.database_id = d.id and d.name = '{{ schema_relation.database }}'
-    where type in ('table', 'source', 'view', 'materialized-view', 'index', 'sink')
+    where o.type in ('table', 'source', 'view', 'materialized-view', 'index', 'sink')
+      --Exclude subsources and progress subsources, which aren't relevant in this
+      --context and can bork the adapter (see #20483)
+      and coalesce(so.type, '') not in ('subsource', 'progress')
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
```

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/macros/catalog.sql` & `dbt-materialize-1.5.0/dbt/include/materialize/macros/catalog.sql`

 * *Files 21% similar despite different names*

```diff
@@ -20,22 +20,29 @@
   {{ adapter.verify_database(database) }}
 
   {%- call statement('catalog', fetch_result=True) -%}
         select
             d.name as table_database,
             s.name as table_schema,
             o.name as table_name,
-            case when o.type = 'materialized-view' then 'materializedview' else o.type end as table_type,
+            case when o.type = 'materialized-view' then 'materializedview'
+                 --This macro is used for the dbt documentation. We use
+                 --the source type in mz_sources here instead of that
+                 --in mz_objects to correctly report subsources.
+                 when o.type = 'source' then so.type
+                 else o.type end as table_type,
             '' as table_comment,
             c.name as column_name,
             c.position as column_index,
             c.type as column_type,
             '' as column_comment,
-            '' as table_owner
+            r.name as table_owner
         from mz_objects o
+        left join mz_sources so on o.id = so.id
+        join mz_roles r on o.owner_id = r.id
         join mz_schemas s on o.schema_id = s.id
         join mz_databases d on s.database_id = d.id and d.name = '{{ database }}'
         join mz_columns c on c.id = o.id
         where s.name in (
             {%- for schema in schemas -%}
                 '{{ schema }}' {%- if not loop.last %}, {% endif -%}
             {%- endfor -%}
```

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/incremental.sql` & `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/materialized_view.sql` & `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/seed.sql` & `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/sink.sql` & `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/sink.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/source.sql` & `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/source.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/table.sql` & `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/test.sql` & `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/macros/materializations/view.sql` & `dbt-materialize-1.5.0/dbt/include/materialize/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt/include/materialize/macros/utils/listagg.sql` & `dbt-materialize-1.5.0/dbt/include/materialize/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/dbt_materialize.egg-info/PKG-INFO` & `dbt-materialize-1.5.0/dbt_materialize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.4.1
+Version: 1.5.0
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `dbt-materialize-1.4.1/dbt_materialize.egg-info/SOURCES.txt` & `dbt-materialize-1.5.0/dbt_materialize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.4.1/setup.py` & `dbt-materialize-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 from setuptools import find_packages
 
 setup(
     name="dbt-materialize",
     # This adapter's minor version should match the required dbt-postgres version,
     # but patch versions may differ.
     # If you bump this version, bump it in __version__.py too.
-    version="1.4.1",
+    version="1.5.0",
     description="The Materialize adapter plugin for dbt.",
     long_description=(Path(__file__).parent / "README.md").open().read(),
     long_description_content_type="text/markdown",
     author="Materialize, Inc.",
     author_email="support@materialize.com",
     url="https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize",
     packages=find_packages(),
     package_data={
         "dbt": [
             "include/materialize/dbt_project.yml",
             "include/materialize/macros/*.sql",
             "include/materialize/macros/**/*.sql",
         ]
     },
-    install_requires=["dbt-postgres~=1.4.0"],
+    install_requires=["dbt-postgres~=1.5.0"],
     extras_require={
-        "dev": ["dbt-tests-adapter~=1.4.0"],
+        "dev": ["dbt-tests-adapter~=1.5.0"],
     },
 )
```


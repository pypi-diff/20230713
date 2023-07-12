# Comparing `tmp/dbt_semantic_interfaces-0.1.0.dev9.tar.gz` & `tmp/dbt_semantic_interfaces-0.1.0rc1.tar.gz`

## Comparing `dbt_semantic_interfaces-0.1.0.dev9.tar` & `dbt_semantic_interfaces-0.1.0rc1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/.tool-versions
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/CHANGELOG.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/__init__.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/base.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/metadata.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/metric.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/project_configuration.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_manifest.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_model.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_version.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/__init__.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/dimension.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/entity.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/filters/__init__.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/generate_json_schema_file.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/__init__.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/dimension.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/entity.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/metadata.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/metric.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/project_configuration.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/protocol_hint.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/semantic_manifest.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/semantic_model.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/semantic_version.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/time_spine_configuration.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/agg_time_dimension.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/rule_set.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/entity_type.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/metric_type.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0    28360 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    15056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/pyvenv.cfg
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/Activate.ps1
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/activate
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/activate.csh
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/activate.fish
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/hatch
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/hatchling
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/httpx
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/keyring
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/markdown-it
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/pip
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/pip3
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/pip3.9
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/pygmentize
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/python3.9 -> python
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/userpath
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/virtualenv
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/README.md
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/pyproject.toml
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev9/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/.tool-versions
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/call_parameter_sets.py
+-rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/__init__.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/base.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/metadata.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/metric.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/project_configuration.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_manifest.py
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_model.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_version.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/__init__.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/dimension.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/entity.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/filters/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/generate_json_schema_file.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/where_filter_parser.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/project_configuration.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/protocol_hint.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/semantic_version.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/time_spine_configuration.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/rule_set.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0    28374 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
+-rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    15056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/pyvenv.cfg
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/Activate.ps1
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate.csh
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate.fish
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/hatch
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/hatchling
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/httpx
+-rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/keyring
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/markdown-it
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/pip
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/pip3
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/pip3.9
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/pygmentize
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/python3.9 -> python
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/userpath
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/virtualenv
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/README.md
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/Makefile` & `dbt_semantic_interfaces-0.1.0rc1/Makefile`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/base.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/base.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/metric.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/project_configuration.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/project_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_model.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     SemanticModel,
     SemanticModelDefaults,
 )
 from dbt_semantic_interfaces.references import (
     LinkableElementReference,
     MeasureReference,
     SemanticModelReference,
+    TimeDimensionReference,
 )
 
 
 class NodeRelation(HashableBaseModel):
     """Path object to where the data should be."""
 
     alias: str
@@ -163,7 +164,20 @@
 
     def get_entity(self, entity_reference: LinkableElementReference) -> PydanticEntity:  # noqa: D
         for entity in self.entities:
             if entity.reference == entity_reference:
                 return entity
 
         raise ValueError(f"No entity with name ({entity_reference}) in semantic_model with name ({self.name})")
+
+    def checked_agg_time_dimension_for_measure(self, measure_reference: MeasureReference):  # noqa: D
+        measure = self.get_measure(measure_reference=measure_reference)
+        if self.defaults is not None:
+            default_agg_time_dimesion = self.defaults.agg_time_dimension
+
+        agg_time_dimension_name = measure.agg_time_dimension or default_agg_time_dimesion
+        assert agg_time_dimension_name is not None, (
+            f"Aggregation time dimension for measure {measure.name} is not set! This should either be set directly on "
+            f"the measure specification in the model, or else defaulted to the primary time dimension in the data "
+            f"source containing the measure."
+        )
+        return TimeDimensionReference(element_name=agg_time_dimension_name)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/semantic_version.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,19 @@
 from typing_extensions import override
 
 from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     PydanticCustomInputParser,
     PydanticParseableValueType,
 )
-from dbt_semantic_interfaces.protocols.semantic_version import SemanticVersion
 
 
 class PydanticSemanticVersion(PydanticCustomInputParser, HashableBaseModel):
     """Pydantic implementation of SemanticVersion."""
 
-    @override
-    def _implements_protocol(self) -> SemanticVersion:
-        return self
-
     major_version: str
     minor_version: str
     patch_version: Optional[str]
 
     @classmethod
     @override
     def _from_yaml_value(cls, input: PydanticParseableValueType) -> PydanticSemanticVersion:
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/dimension.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/entity.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/elements/measure.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/measure.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, Optional
 
 from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
 )
 from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
-from dbt_semantic_interfaces.references import MeasureReference, TimeDimensionReference
+from dbt_semantic_interfaces.references import MeasureReference
 from dbt_semantic_interfaces.type_enums import AggregationType
 
 
 class PydanticNonAdditiveDimensionParameters(HashableBaseModel):
     """Describes the params for specifying non-additive dimensions in a measure.
 
     NOTE: Currently, only TimeDimensions are supported for this filter
@@ -42,18 +42,9 @@
     expr: Optional[str] = None
     agg_params: Optional[PydanticMeasureAggregationParameters]
     metadata: Optional[PydanticMetadata]
     non_additive_dimension: Optional[PydanticNonAdditiveDimensionParameters] = None
     agg_time_dimension: Optional[str] = None
 
     @property
-    def checked_agg_time_dimension(self) -> TimeDimensionReference:  # noqa: D
-        assert self.agg_time_dimension, (
-            f"Aggregation time dimension for measure {self.name} is not set! This should either be set directly on "
-            f"the measure specification in the model, or else defaulted to the primary time dimension in the data "
-            f"source containing the measure."
-        )
-        return TimeDimensionReference(element_name=self.agg_time_dimension)
-
-    @property
     def reference(self) -> MeasureReference:  # noqa: D
         return MeasureReference(element_name=self.name)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/call_parameter_sets.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/generate_json_schema_file.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/generate_json_schema_file.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/objects.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/__init__.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/dimension.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/entity.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/measure.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/measure.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import Optional, Protocol, Sequence
 
-from dbt_semantic_interfaces.references import MeasureReference, TimeDimensionReference
+from dbt_semantic_interfaces.references import MeasureReference
 from dbt_semantic_interfaces.type_enums import AggregationType
 
 
 class NonAdditiveDimensionParameters(Protocol):
     """Describes the params for specifying non-additive dimensions in a measure."""
 
     @property
@@ -85,16 +85,10 @@
     @property
     @abstractmethod
     def agg_time_dimension(self) -> Optional[str]:  # noqa: D
         pass
 
     @property
     @abstractmethod
-    def checked_agg_time_dimension(self) -> TimeDimensionReference:
-        """Returns the aggregation time dimension, throwing an exception if it's not set."""
-        ...
-
-    @property
-    @abstractmethod
     def reference(self) -> MeasureReference:
         """Returns a reference to this measure."""
         ...
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/metadata.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/metric.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/project_configuration.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/project_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/protocol_hint.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/protocol_hint.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/semantic_model.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/semantic_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dbt_semantic_interfaces.protocols.entity import Entity
 from dbt_semantic_interfaces.protocols.measure import Measure
 from dbt_semantic_interfaces.protocols.metadata import Metadata
 from dbt_semantic_interfaces.references import (
     LinkableElementReference,
     MeasureReference,
     SemanticModelReference,
+    TimeDimensionReference,
 )
 
 
 class NodeRelation(Protocol):
     """Path object to where the data should be."""
 
     @property
@@ -142,9 +143,17 @@
         ...
 
     @property
     @abstractmethod
     def metadata(self) -> Optional[Metadata]:  # noqa: D
         pass
 
+    @abstractmethod
+    def checked_agg_time_dimension_for_measure(self, measure_reference: MeasureReference) -> TimeDimensionReference:
+        """Returns the `TimeDimensionReference` what a measure should use for it's `agg_time_dimension`.
+
+        Should raise an exception if a TimeDimensionReference cannot be built
+        """
+        ...
+
 
 SemanticModelT = TypeVar("SemanticModelT", bound=SemanticModel)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/protocols/time_spine_configuration.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/time_spine_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/add_input_metric_measures.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/add_input_metric_measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-import logging
-
 from typing_extensions import override
 
+from dbt_semantic_interfaces.errors import ModelTransformError
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
 from dbt_semantic_interfaces.protocols import ProtocolHint
 from dbt_semantic_interfaces.transformations.transform_rule import (
     SemanticManifestTransformRule,
 )
+from dbt_semantic_interfaces.type_enums import AggregationType
 
-logger = logging.getLogger(__name__)
+ONE = "1"
 
 
-class SetMeasureAggregationTimeDimensionRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
-    """Sets the aggregation time dimension for measures to the one specified as default."""
+class ConvertCountToSumRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
+    """Converts any COUNT measures to SUM equivalent."""
 
     @override
     def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
         return self
 
     @staticmethod
     def transform_model(semantic_manifest: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
         for semantic_model in semantic_manifest.semantic_models:
-            if semantic_model.defaults is None:
-                continue
-
-            if semantic_model.defaults.agg_time_dimension is None:
-                continue
-
             for measure in semantic_model.measures:
-                if not measure.agg_time_dimension:
-                    measure.agg_time_dimension = semantic_model.defaults.agg_time_dimension
-
+                if measure.agg == AggregationType.COUNT:
+                    if measure.expr is None:
+                        raise ModelTransformError(
+                            f"Measure '{measure.name}' uses a COUNT aggregation, which requires an expr to be "
+                            f"provided. Provide 'expr: 1' if a count of all rows is desired."
+                        )
+                    if measure.expr != ONE:
+                        # Just leave it as SUM(1) if we want to count all
+                        measure.expr = f"CASE WHEN {measure.expr} IS NOT NULL THEN 1 ELSE 0 END"
+                    measure.agg = AggregationType.SUM
         return semantic_manifest
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/names.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,50 @@
+import logging
+
 from typing_extensions import override
 
-from dbt_semantic_interfaces.errors import ModelTransformError
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
+from dbt_semantic_interfaces.implementations.semantic_model import PydanticSemanticModel
 from dbt_semantic_interfaces.protocols import ProtocolHint
 from dbt_semantic_interfaces.transformations.transform_rule import (
     SemanticManifestTransformRule,
 )
-from dbt_semantic_interfaces.type_enums import AggregationType
 
-ONE = "1"
+logger = logging.getLogger(__name__)
 
 
-class ConvertCountToSumRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
-    """Converts any COUNT measures to SUM equivalent."""
+class LowerCaseNamesRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
+    """Lowercases the names of both top level objects and semantic model elements in a model."""
 
     @override
     def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
         return self
 
     @staticmethod
     def transform_model(semantic_manifest: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
+        LowerCaseNamesRule._lowercase_top_level_objects(semantic_manifest)
         for semantic_model in semantic_manifest.semantic_models:
-            for measure in semantic_model.measures:
-                if measure.agg == AggregationType.COUNT:
-                    if measure.expr is None:
-                        raise ModelTransformError(
-                            f"Measure '{measure.name}' uses a COUNT aggregation, which requires an expr to be "
-                            f"provided. Provide 'expr: 1' if a count of all rows is desired."
-                        )
-                    if measure.expr != ONE:
-                        # Just leave it as SUM(1) if we want to count all
-                        measure.expr = f"CASE WHEN {measure.expr} IS NOT NULL THEN 1 ELSE 0 END"
-                    measure.agg = AggregationType.SUM
+            LowerCaseNamesRule._lowercase_semantic_model_elements(semantic_model)
+
         return semantic_manifest
+
+    @staticmethod
+    def _lowercase_semantic_model_elements(semantic_model: PydanticSemanticModel) -> None:
+        """Lowercases the names of semantic model elements."""
+        if semantic_model.measures:
+            for measure in semantic_model.measures:
+                measure.name = measure.name.lower()
+        if semantic_model.entities:
+            for entity in semantic_model.entities:
+                entity.name = entity.name.lower()
+        if semantic_model.dimensions:
+            for dimension in semantic_model.dimensions:
+                dimension.name = dimension.name.lower()
+
+    @staticmethod
+    def _lowercase_top_level_objects(model: PydanticSemanticManifest) -> None:
+        """Lowercases the names of model objects."""
+        if model.semantic_models:
+            for semantic_model in model.semantic_models:
+                semantic_model.name = semantic_model.name.lower()
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/pydantic_rule_set.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/pydantic_rule_set.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
 from dbt_semantic_interfaces.protocols import ProtocolHint
 from dbt_semantic_interfaces.transformations.add_input_metric_measures import (
     AddInputMetricMeasuresRule,
 )
-from dbt_semantic_interfaces.transformations.agg_time_dimension import (
-    SetMeasureAggregationTimeDimensionRule,
-)
 from dbt_semantic_interfaces.transformations.boolean_measure import (
     BooleanMeasureAggregationRule,
 )
 from dbt_semantic_interfaces.transformations.convert_count import ConvertCountToSumRule
 from dbt_semantic_interfaces.transformations.convert_median import (
     ConvertMedianToPercentileRule,
 )
@@ -39,18 +36,15 @@
 
     @override
     def _implements_protocol(self) -> SemanticManifestTransformRuleSet[PydanticSemanticManifest]:  # noqa: D
         return self
 
     @property
     def primary_rules(self) -> Sequence[SemanticManifestTransformRule[PydanticSemanticManifest]]:  # noqa:
-        return (
-            LowerCaseNamesRule(),
-            SetMeasureAggregationTimeDimensionRule(),
-        )
+        return (LowerCaseNamesRule(),)
 
     @property
     def secondary_rules(self) -> Sequence[SemanticManifestTransformRule[PydanticSemanticManifest]]:  # noqa: D
         return (
             CreateProxyMeasureRule(),
             BooleanMeasureAggregationRule(),
             ConvertCountToSumRule(),
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/rule_set.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/transformations/transform_rule.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/transform_rule.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/type_enums/time_granularity.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/time_granularity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             measure_context = SemanticModelElementContext(
                 file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
                 semantic_model_element=SemanticModelElementReference(
                     semantic_model_name=semantic_model.name, element_name=measure.name
                 ),
                 element_type=SemanticModelElementType.MEASURE,
             )
-            agg_time_dimension_reference = measure.checked_agg_time_dimension
+            agg_time_dimension_reference = semantic_model.checked_agg_time_dimension_for_measure(measure.reference)
             if not SemanticModelValidationHelpers.time_dimension_in_model(
                 time_dimension_name=agg_time_dimension_reference.element_name, semantic_model=semantic_model
             ):
                 issues.append(
                     ValidationError(
                         context=measure_context,
                         message=f"In semantic model '{semantic_model.name}', measure '{measure.name}' has the "
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/element_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/entities.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/measures.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,20 +228,17 @@
     def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
         for semantic_model in semantic_manifest.semantic_models or []:
             for measure in semantic_model.measures:
                 non_additive_dimension = measure.non_additive_dimension
                 if non_additive_dimension is None:
                     continue
+                agg_time_dimension_reference = semantic_model.checked_agg_time_dimension_for_measure(measure.reference)
                 agg_time_dimension = next(
-                    (
-                        dim
-                        for dim in semantic_model.dimensions
-                        if measure.checked_agg_time_dimension.element_name == dim.name
-                    ),
+                    (dim for dim in semantic_model.dimensions if agg_time_dimension_reference.element_name == dim.name),
                     None,
                 )
                 if agg_time_dimension is None:
                     # Sanity check, should never hit this
                     issues.append(
                         ValidationError(
                             context=SemanticModelElementContext(
@@ -249,15 +246,15 @@
                                 semantic_model_element=SemanticModelElementReference(
                                     semantic_model_name=semantic_model.name, element_name=measure.name
                                 ),
                                 element_type=SemanticModelElementType.MEASURE,
                             ),
                             message=(
                                 f"Measure '{measure.name}' has a agg_time_dimension of "
-                                f"{measure.checked_agg_time_dimension.element_name} "
+                                f"{agg_time_dimension_reference.element_name} "
                                 f"that is not defined as a dimension in semantic model '{semantic_model.name}'."
                             ),
                         )
                     )
                     continue
 
                 # Validates that the non_additive_dimension exists as a time dimension in the semantic model
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/metrics.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/semantic_manifest_validator.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/semantic_manifest_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     CumulativeMetricRule,
     DerivedMetricRule,
 )
 from dbt_semantic_interfaces.validations.non_empty import NonEmptyRule
 from dbt_semantic_interfaces.validations.reserved_keywords import ReservedKeywordsRule
 from dbt_semantic_interfaces.validations.semantic_models import (
     SemanticModelDefaultsRule,
-    SemanticModelTimeDimensionWarningsRule,
     SemanticModelValidityWindowRule,
 )
 from dbt_semantic_interfaces.validations.unique_valid_name import UniqueAndValidNameRule
 from dbt_semantic_interfaces.validations.validator_helpers import (
     SemanticManifestValidationException,
     SemanticManifestValidationResults,
     SemanticManifestValidationRule,
@@ -58,15 +57,14 @@
     """A Validator that acts on SemanticManifest."""
 
     DEFAULT_RULES: Sequence[SemanticManifestValidationRule[SemanticManifestT]] = (
         PercentileAggregationRule[SemanticManifestT](),
         DerivedMetricRule[SemanticManifestT](),
         CountAggregationExprRule[SemanticManifestT](),
         SemanticModelMeasuresUniqueRule[SemanticManifestT](),
-        SemanticModelTimeDimensionWarningsRule[SemanticManifestT](),
         SemanticModelValidityWindowRule[SemanticManifestT](),
         DimensionConsistencyRule[SemanticManifestT](),
         ElementConsistencyRule[SemanticManifestT](),
         NaturalEntityConfigurationRule[SemanticManifestT](),
         OnePrimaryEntityPerSemanticModelRule[SemanticManifestT](),
         MeasureConstraintAliasesRule[SemanticManifestT](),
         MetricMeasuresRule[SemanticManifestT](),
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,51 +13,14 @@
     ValidationIssue,
     validate_safely,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class SemanticModelTimeDimensionWarningsRule(
-    SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]
-):
-    """Checks time dimensions in semantic models."""
-
-    @staticmethod
-    @validate_safely(whats_being_done="running model validation ensuring time dimensions are defined properly")
-    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
-        issues: List[ValidationIssue] = []
-
-        for semantic_model in semantic_manifest.semantic_models:
-            issues.extend(
-                SemanticModelTimeDimensionWarningsRule._validate_semantic_model(semantic_model=semantic_model)
-            )
-        return issues
-
-    @staticmethod
-    @validate_safely(whats_being_done="checking validity of the semantic model's time dimensions")
-    def _validate_semantic_model(semantic_model: SemanticModel) -> List[ValidationIssue]:
-        issues: List[ValidationIssue] = []
-
-        for measure in semantic_model.measures:
-            if measure.agg_time_dimension is None:
-                issues.append(
-                    ValidationError(
-                        context=SemanticModelContext(
-                            file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
-                            semantic_model=SemanticModelReference(semantic_model_name=semantic_model.name),
-                        ),
-                        message=f"Aggregation time dimension not specified for measure named '{measure.name}' in the "
-                        f"semantic model named '{semantic_model.name}'. Please add one",
-                    )
-                )
-
-        return issues
-
-
 class SemanticModelValidityWindowRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks validity windows in semantic models to ensure they comply with runtime requirements."""
 
     @staticmethod
     @validate_safely(whats_being_done="checking correctness of the time dimension validity parameters in the model")
     def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:
         """Checks the validity param definitions in every semantic model in the model."""
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/Activate.ps1` & `dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/activate` & `dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/activate.csh` & `dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/venv-3.9.16/bin/activate.fish` & `dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/.gitignore` & `dbt_semantic_interfaces-0.1.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/LICENSE` & `dbt_semantic_interfaces-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/README.md` & `dbt_semantic_interfaces-0.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/pyproject.toml` & `dbt_semantic_interfaces-0.1.0rc1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.1.0.dev9"
+version = "0.1.0rc1"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
@@ -16,23 +16,23 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "pydantic~=1.10.8",
-  "jsonschema==3.2.0",
+  "pydantic~=1.10",
+  "jsonschema~=3.0",
   "PyYAML~=6.0",
-  "more-itertools==8.10.0",
-  "Jinja2==3.1.2",
-  "click>=7.1.2",
-  "python-dateutil==2.8.2",
-  "importlib_metadata==6.6.0",
-  "typing-extensions~=4.6.1",
+  "more-itertools~=8.0",
+  "Jinja2~=3.0",
+  "click>=7.0,<9.0",
+  "python-dateutil~=2.0",
+  "importlib_metadata~=6.0",
+  "typing-extensions~=4.0",
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.sdist]
@@ -49,27 +49,27 @@
 
 [tool.hatch.envs.dev-env.scripts]
 all = ["pre-commit run --all-files"]
 
 [tool.hatch.envs.dev-env]
 description = "Env for running development commands like pytest / pre-commit"
 dependencies = [
-  "pytest~=7.3.0",
-  "pytest-xdist~=3.2.1",
-  "httpx~=0.24.0",
-  "pre-commit~=3.2.2",
-  "isort~=5.12.0",
-  "black~=23.3.0",
-  "ruff~=0.0.260",
-  "mypy~=1.3.0",
-  "pytest~=7.3.0",
-  "types-Jinja2~=2.11.9",
+  "pytest~=7.3",
+  "pytest-xdist~=3.2",
+  "httpx~=0.24",
+  "pre-commit~=3.2",
+  "isort~=5.12",
+  "black~=23.3",
+  "ruff==0.0.260",
+  "mypy~=1.3",
+  "pytest~=7.3",
+  "types-Jinja2~=2.11",
   "types-jsonschema~=4.17",
-  "types-python-dateutil~=2.8.19",
-  "types-PyYAML~=6.0.12",
+  "types-python-dateutil~=2.8",
+  "types-PyYAML~=6.0",
 ]
 
 [tool.ruff]
 line-length = 120
 select = [
   "E", # Pycodestyle
   "F", # Pyflakes
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev9/PKG-INFO` & `dbt_semantic_interfaces-0.1.0rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: dbt-semantic-interfaces
-Version: 0.1.0.dev9
+Version: 0.1.0rc1
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: click>=7.1.2
-Requires-Dist: importlib-metadata==6.6.0
-Requires-Dist: jinja2==3.1.2
-Requires-Dist: jsonschema==3.2.0
-Requires-Dist: more-itertools==8.10.0
-Requires-Dist: pydantic~=1.10.8
-Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: click<9.0,>=7.0
+Requires-Dist: importlib-metadata~=6.0
+Requires-Dist: jinja2~=3.0
+Requires-Dist: jsonschema~=3.0
+Requires-Dist: more-itertools~=8.0
+Requires-Dist: pydantic~=1.10
+Requires-Dist: python-dateutil~=2.0
 Requires-Dist: pyyaml~=6.0
-Requires-Dist: typing-extensions~=4.6.1
+Requires-Dist: typing-extensions~=4.0
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a target="_blank" href="https://twitter.com/dbt_labs">
     <img src="https://img.shields.io/twitter/follow/dbt_labs?labelColor=image.png&color=163B36&logo=twitter&style=flat">
   </a>
     <a target="_blank" href="https://www.getdbt.com/community/">
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev9
-Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
-Author-email: dbt Labs
+Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0rc1 Summary:
+The shared semantic layer definitions that dbt-core and MetricFlow use Author-
+email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Requires-Python: >=3.8 Requires-
-Dist: click>=7.1.2 Requires-Dist: importlib-metadata==6.6.0 Requires-Dist:
-jinja2==3.1.2 Requires-Dist: jsonschema==3.2.0 Requires-Dist: more-
-itertools==8.10.0 Requires-Dist: pydantic~=1.10.8 Requires-Dist: python-
-dateutil==2.8.2 Requires-Dist: pyyaml~=6.0 Requires-Dist: typing-
-extensions~=4.6.1 Description-Content-Type: text/markdown
+Dist: click<9.0,>=7.0 Requires-Dist: importlib-metadata~=6.0 Requires-Dist:
+jinja2~=3.0 Requires-Dist: jsonschema~=3.0 Requires-Dist: more-itertools~=8.0
+Requires-Dist: pydantic~=1.10 Requires-Dist: python-dateutil~=2.0 Requires-
+Dist: pyyaml~=6.0 Requires-Dist: typing-extensions~=4.0 Description-Content-
+Type: text/markdown
                     [https://img.shields.io/twitter/follow/
  dbt_labs?labelColor=image.png&color=163B36&logo=twitter&style=flat] [https://
     img.shields.io/badge/Slack-join-163B36] [https://img.shields.io/badge/
                         code%20style-black-000000.svg]
 # dbt-semantic-interfaces This repo contains the shared semantic classes,
 default validation, and tests designed to be used by both the dbt-core and
 MetricFlow projects. By centralizing these shared resources, we aim to maintain
```


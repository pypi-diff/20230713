# Comparing `tmp/taxpasta-0.4.0.tar.gz` & `tmp/taxpasta-0.4.1.tar.gz`

## Comparing `taxpasta-0.4.0.tar` & `taxpasta-0.4.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/__init__.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/py.typed
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/__init__.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/consensus_application.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/sample_merging_application.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/error/__init__.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/error/standardisation_error.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/error/taxpasta_error.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/_types.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/profile_reader.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/profile_standardisation_service.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/standard_profile_writer.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/table_reader.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/tidy_observation_table_writer.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/wide_observation_table_writer.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/__init__.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/model/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/model/sample.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/model/standard_profile.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/model/tidy_observation_table.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/model/wide_observation_table.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/service/__init__.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/service/consensus_builder.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/service/sample_merging_service.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/service/taxonomy_service.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/__init__.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/__init__.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/_dependency_check_mixin.py
--rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/application_service_registry.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/sample_etl_application.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/sample_sheet.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_file_format.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/supported_profiler.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader_file_format.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_file_format.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_file_format.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/__init__.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/bracken_profile.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/bracken_profile_reader.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/bracken_profile_standardisation_service.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/__init__.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_reader.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_standardisation_service.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/__init__.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/diamond_profile.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_reader.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_standardisation_service.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/__init__.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/ganon_profile.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/ganon_profile_reader.py
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/ganon_profile_standardisation_service.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/__init__.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_reader.py
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_standardisation_service.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/__init__.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_reader.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_standardisation_service.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/__init__.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_reader.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_standardisation_service.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_reader.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_standardisation_service.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/__init__.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_reader.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_standardisation_service.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/__init__.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile_reader.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile_standardisation_service.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/arrow_standard_profile_writer.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/csv_standard_profile_writer.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/ods_standard_profile_writer.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/parquet_standard_profile_writer.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/tsv_standard_profile_writer.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/xlsx_standard_profile_writer.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/__init__.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/arrow_table_reader.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/csv_table_reader.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/ods_table_reader.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/parquet_table_reader.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/tsv_table_reader.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/xlsx_table_reader.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/__init__.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/arrow_table_writer.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/csv_table_writer.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/ods_table_writer.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/parquet_table_writer.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/tsv_table_writer.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/xlsx_table_writer.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/__init__.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/arrow_wide_observation_table_writer.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/biom_wide_observation_table_writer.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/csv_wide_observation_table_writer.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/ods_wide_observation_table_writer.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/parquet_wide_observation_table_writer.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/tsv_wide_observation_table_writer.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/xlsx_wide_observation_table_writer.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/cli/__init__.py
--rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/cli/merge.py
--rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/cli/standardise.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/cli/taxpasta.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/domain/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/domain/service/__init__.py
--rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/domain/service/taxopy_taxonomy_service.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/helpers/__init__.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/helpers/base_data_frame_model.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/helpers/decorators.py
--rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 taxpasta-0.4.0/.gitignore
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 taxpasta-0.4.0/LICENSE
--rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 taxpasta-0.4.0/README.md
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 taxpasta-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 taxpasta-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/__init__.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/py.typed
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/__init__.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/consensus_application.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/sample_merging_application.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/error/__init__.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/error/standardisation_error.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/error/taxpasta_error.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/service/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/service/_types.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/service/profile_reader.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/service/profile_standardisation_service.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/service/standard_profile_writer.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/service/table_reader.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/service/tidy_observation_table_writer.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/application/service/wide_observation_table_writer.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/domain/__init__.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/domain/model/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/domain/model/sample.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/domain/model/standard_profile.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/domain/model/tidy_observation_table.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/domain/model/wide_observation_table.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/domain/service/__init__.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/domain/service/consensus_builder.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/domain/service/sample_merging_service.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/domain/service/taxonomy_service.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/__init__.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/__init__.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/_dependency_check_mixin.py
+-rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/application_service_registry.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/sample_etl_application.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/sample_sheet.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_file_format.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/supported_profiler.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader_file_format.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_file_format.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_file_format.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/bracken/__init__.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/bracken/bracken_profile.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/bracken/bracken_profile_reader.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/bracken/bracken_profile_standardisation_service.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/centrifuge/__init__.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_reader.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_standardisation_service.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/diamond/__init__.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/diamond/diamond_profile.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/diamond/diamond_profile_reader.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/diamond/diamond_profile_standardisation_service.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/ganon/__init__.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/ganon/ganon_profile.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/ganon/ganon_profile_reader.py
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/ganon/ganon_profile_standardisation_service.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/kaiju/__init__.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/kaiju/kaiju_profile.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_reader.py
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_standardisation_service.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/kraken2/__init__.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/kraken2/kraken2_profile.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_reader.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_standardisation_service.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/krakenuniq/__init__.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_reader.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_standardisation_service.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/megan6/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/megan6/megan6_profile.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/megan6/megan6_profile_reader.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/megan6/megan6_profile_standardisation_service.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/metaphlan/__init__.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_reader.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_standardisation_service.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/motus/__init__.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/motus/motus_profile.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/motus/motus_profile_reader.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/motus/motus_profile_standardisation_service.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/arrow_standard_profile_writer.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/csv_standard_profile_writer.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/ods_standard_profile_writer.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/parquet_standard_profile_writer.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/tsv_standard_profile_writer.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/xlsx_standard_profile_writer.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/__init__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/arrow_table_reader.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/csv_table_reader.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/ods_table_reader.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/parquet_table_reader.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/tsv_table_reader.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/xlsx_table_reader.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/__init__.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/arrow_table_writer.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/csv_table_writer.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/ods_table_writer.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/parquet_table_writer.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/tsv_table_writer.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/xlsx_table_writer.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/__init__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/arrow_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/biom_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/csv_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/ods_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/parquet_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/tsv_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/xlsx_wide_observation_table_writer.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/cli/__init__.py
+-rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/cli/merge.py
+-rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/cli/standardise.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/cli/taxpasta.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/domain/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/domain/service/__init__.py
+-rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/domain/service/taxopy_taxonomy_service.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/helpers/__init__.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/helpers/base_data_frame_model.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 taxpasta-0.4.1/src/taxpasta/infrastructure/helpers/decorators.py
+-rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 taxpasta-0.4.1/.gitignore
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 taxpasta-0.4.1/LICENSE
+-rw-r--r--   0        0        0    24004 2020-02-02 00:00:00.000000 taxpasta-0.4.1/README.md
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 taxpasta-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 taxpasta-0.4.1/PKG-INFO
```

### Comparing `taxpasta-0.4.0/src/taxpasta/__init__.py` & `taxpasta-0.4.1/src/taxpasta/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/__main__.py` & `taxpasta-0.4.1/src/taxpasta/__main__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/__init__.py` & `taxpasta-0.4.1/src/taxpasta/application/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/consensus_application.py` & `taxpasta-0.4.1/src/taxpasta/application/consensus_application.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/sample_merging_application.py` & `taxpasta-0.4.1/src/taxpasta/application/sample_merging_application.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/error/__init__.py` & `taxpasta-0.4.1/src/taxpasta/application/error/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/error/standardisation_error.py` & `taxpasta-0.4.1/src/taxpasta/application/error/standardisation_error.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/error/taxpasta_error.py` & `taxpasta-0.4.1/src/taxpasta/application/error/taxpasta_error.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/service/__init__.py` & `taxpasta-0.4.1/src/taxpasta/application/service/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/service/_types.py` & `taxpasta-0.4.1/src/taxpasta/application/service/_types.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/service/profile_reader.py` & `taxpasta-0.4.1/src/taxpasta/application/service/profile_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/service/profile_standardisation_service.py` & `taxpasta-0.4.1/src/taxpasta/application/service/profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/service/standard_profile_writer.py` & `taxpasta-0.4.1/src/taxpasta/application/service/standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/service/table_reader.py` & `taxpasta-0.4.1/src/taxpasta/application/service/table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/service/tidy_observation_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/application/service/tidy_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/application/service/wide_observation_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/application/service/wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/domain/__init__.py` & `taxpasta-0.4.1/src/taxpasta/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/domain/model/__init__.py` & `taxpasta-0.4.1/src/taxpasta/domain/model/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/domain/model/sample.py` & `taxpasta-0.4.1/src/taxpasta/domain/model/sample.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/domain/model/standard_profile.py` & `taxpasta-0.4.1/src/taxpasta/domain/model/standard_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/domain/model/tidy_observation_table.py` & `taxpasta-0.4.1/src/taxpasta/domain/model/tidy_observation_table.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/domain/model/wide_observation_table.py` & `taxpasta-0.4.1/src/taxpasta/domain/model/wide_observation_table.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/domain/service/__init__.py` & `taxpasta-0.4.1/src/taxpasta/domain/service/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/domain/service/consensus_builder.py` & `taxpasta-0.4.1/src/taxpasta/domain/service/consensus_builder.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/domain/service/sample_merging_service.py` & `taxpasta-0.4.1/src/taxpasta/domain/service/sample_merging_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/domain/service/taxonomy_service.py` & `taxpasta-0.4.1/src/taxpasta/domain/service/taxonomy_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/_dependency_check_mixin.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/_dependency_check_mixin.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/application_service_registry.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/application_service_registry.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/sample_etl_application.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/sample_etl_application.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/sample_sheet.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_file_format.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_file_format.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/supported_profiler.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/supported_profiler.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader_file_format.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader_file_format.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_file_format.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_file_format.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_file_format.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_file_format.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/bracken/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/bracken_profile.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/bracken/bracken_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/bracken_profile_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/bracken/bracken_profile_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/bracken_profile_standardisation_service.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/bracken/bracken_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/centrifuge/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_standardisation_service.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/diamond/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/diamond_profile.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/diamond/diamond_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/diamond/diamond_profile_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_standardisation_service.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/diamond/diamond_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/ganon/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/ganon_profile.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/ganon/ganon_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/ganon_profile_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/ganon/ganon_profile_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/ganon_profile_standardisation_service.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/ganon/ganon_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/kaiju/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/kaiju/kaiju_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_standardisation_service.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/kraken2/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/kraken2/kraken2_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_standardisation_service.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/krakenuniq/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,11 +48,15 @@
         result = pd.read_table(
             filepath_or_buffer=profile,
             sep="\t",
             skiprows=2,
             header=0,
             index_col=False,
             skipinitialspace=True,
-            dtype={"%": float},
+            dtype={
+                KrakenUniqProfile.percent: float,
+                KrakenUniqProfile.duplicates: float,
+                KrakenUniqProfile.coverage: float,
+            },
         )
         cls._check_num_columns(result, KrakenUniqProfile)
         return result
```

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_standardisation_service.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/megan6/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/megan6/megan6_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/megan6/megan6_profile_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_standardisation_service.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/megan6/megan6_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/metaphlan/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_standardisation_service.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/motus/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/motus/motus_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/motus/motus_profile_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile_standardisation_service.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/motus/motus_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/arrow_standard_profile_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/arrow_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/csv_standard_profile_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/csv_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/ods_standard_profile_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/ods_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/parquet_standard_profile_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/parquet_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/tsv_standard_profile_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/tsv_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/xlsx_standard_profile_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/standard_profile_writer/xlsx_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/arrow_table_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/arrow_table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/csv_table_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/csv_table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/ods_table_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/ods_table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/parquet_table_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/parquet_table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/tsv_table_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/tsv_table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/xlsx_table_reader.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/table_reader/xlsx_table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/arrow_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/arrow_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/csv_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/csv_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/ods_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/ods_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/parquet_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/parquet_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/tsv_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/tsv_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/xlsx_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/tidy_observation_table_writer/xlsx_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/arrow_wide_observation_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/arrow_wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/biom_wide_observation_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/biom_wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/csv_wide_observation_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/csv_wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/ods_wide_observation_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/ods_wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/parquet_wide_observation_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/parquet_wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/tsv_wide_observation_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/tsv_wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/xlsx_wide_observation_table_writer.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/application/wide_observation_table_writer/xlsx_wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/cli/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/cli/merge.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/cli/merge.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/cli/standardise.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/cli/standardise.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/cli/taxpasta.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/cli/taxpasta.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/domain/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/domain/service/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/domain/service/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/domain/service/taxopy_taxonomy_service.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/domain/service/taxopy_taxonomy_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/helpers/__init__.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/helpers/base_data_frame_model.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/helpers/base_data_frame_model.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/src/taxpasta/infrastructure/helpers/decorators.py` & `taxpasta-0.4.1/src/taxpasta/infrastructure/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/.gitignore` & `taxpasta-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/LICENSE` & `taxpasta-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taxpasta-0.4.0/pyproject.toml` & `taxpasta-0.4.1/pyproject.toml`

 * *Files identical despite different names*


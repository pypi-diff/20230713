# Comparing `tmp/cg-38.2.7.tar.gz` & `tmp/cg-38.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-38.2.7.tar", last modified: Thu Jul 13 06:37:25 2023, max compression
+gzip compressed data, was "dist/cg-38.2.8.tar", last modified: Thu Jul 13 09:57:23 2023, max compression
```

## Comparing `cg-38.2.7.tar` & `cg-38.2.8.tar`

### file list

```diff
@@ -1,1312 +1,1311 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 06:37:14.000000 cg-38.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-13 06:37:25.000000 cg-38.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-13 06:37:14.000000 cg-38.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 06:37:14.000000 cg-38.2.7/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/dragen_demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/db/models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/demultiplex/sample_sheet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/lims/sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-13 06:37:14.000000 cg-38.2.7/cg/apps/tb/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20219 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/demultiplex/sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/set/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/set/cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/upload/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/taxprofiler/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-13 06:37:14.000000 cg-38.2.7/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 06:37:14.000000 cg-38.2.7/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-13 06:37:14.000000 cg-38.2.7/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-13 06:37:14.000000 cg-38.2.7/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-13 06:37:14.000000 cg-38.2.7/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-13 06:37:14.000000 cg-38.2.7/cg/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-13 06:37:14.000000 cg-38.2.7/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-13 06:37:14.000000 cg-38.2.7/cg/io/validate_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-13 06:37:14.000000 cg-38.2.7/cg/io/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-13 06:37:14.000000 cg-38.2.7/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/archive/ddn_dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28406 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/demultiplex/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/demultiplex/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/demultiplex/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/rnafusion_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/report/report_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/report/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77763 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/report/templates/mip-dna_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    78381 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/report/templates/rnafusion_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/upload/upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26030 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13526 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-13 06:37:14.000000 cg-38.2.7/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12662 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/rnafusion/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/rnafusion/command_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/rnafusion/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/taxprofiler/taxprofiler_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-13 06:37:14.000000 cg-38.2.7/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-07-13 06:37:14.000000 cg-38.2.7/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-13 06:37:14.000000 cg-38.2.7/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-13 06:37:14.000000 cg-38.2.7/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 06:37:14.000000 cg-38.2.7/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29392 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38740 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_metrics_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    31064 2023-07-13 06:37:14.000000 cg-38.2.7/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-13 06:37:14.000000 cg-38.2.7/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-13 06:37:24.000000 cg-38.2.7/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    44182 2023-07-13 06:37:25.000000 cg-38.2.7/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:37:24.000000 cg-38.2.7/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 06:37:24.000000 cg-38.2.7/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:37:24.000000 cg-38.2.7/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-13 06:37:24.000000 cg-38.2.7/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-13 06:37:24.000000 cg-38.2.7/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-13 06:37:14.000000 cg-38.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 06:37:14.000000 cg-38.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 06:37:25.000000 cg-38.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-13 06:37:14.000000 cg-38.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/demultiplex/test_dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/demultiplex/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/demultiplex/test_read_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/demultiplex/test_sample_sheet_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/demultiplex/test_sample_sheet_creator_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/lims/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/lims/test_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/sequencing_metrics_parser/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/sequencing_metrics_parser/parsers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-13 06:37:14.000000 cg-38.2.7/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/delete/test_cli_delete_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/set/test_cli_set_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/test_clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/upload/test_cli_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/microsalt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/taxprofiler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-13 06:37:14.000000 cg-38.2.7/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    93270 2023-07-13 06:37:14.000000 cg-38.2.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/analysis/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/demuxcomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/copy_complete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/CopyComplete.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RTAComplete.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunCompletionStatus.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)    79276 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunInfo.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)     4459 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/run_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/sequencing_metrics_parser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/cgweb_orders/rnafusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/io/example_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/io/example_json.json
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/io/example_xml.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   257895 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/1508.28.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257305 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/1508.28.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257516 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/1508.28.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257046 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/1508.28.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257619 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/1508.28.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257428 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/1508.28.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257569 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/1508.28.rnafusion.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   165243 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/1604.17.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88532 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/1605.11.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-13 06:37:14.000000 cg-38.2.7/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-13 06:37:14.000000 cg-38.2.7/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-07-13 06:37:14.000000 cg-38.2.7/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-13 06:37:14.000000 cg-38.2.7/tests/io/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-13 06:37:14.000000 cg-38.2.7/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-13 06:37:14.000000 cg-38.2.7/tests/io/test_io_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-13 06:37:14.000000 cg-38.2.7/tests/io/test_io_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-13 06:37:14.000000 cg-38.2.7/tests/io/test_validate_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/clean/test_clean_flow_cell_run_directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/clean/test_remove_old_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29259 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/demultiplex/test_rename_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/demultiplex/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/demultiplex/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/demultiplex/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/demultiplex/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/demultiplex/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/orders/test_rnafusion_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/report/test_report_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/report/test_rnafusion_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/gisaid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    32110 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-13 06:37:14.000000 cg-38.2.7/tests/meta/workflow/test_rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-13 06:37:14.000000 cg-38.2.7/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/demultiplexing/test_flowcell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/demultiplexing/test_run_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-13 06:37:14.000000 cg-38.2.7/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-13 06:37:14.000000 cg-38.2.7/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-13 06:37:14.000000 cg-38.2.7/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-13 06:37:14.000000 cg-38.2.7/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-13 06:37:14.000000 cg-38.2.7/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_metrics_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29863 2023-07-13 06:37:14.000000 cg-38.2.7/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-13 06:37:14.000000 cg-38.2.7/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:25.000000 cg-38.2.7/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:37:14.000000 cg-38.2.7/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 06:37:14.000000 cg-38.2.7/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-13 06:37:14.000000 cg-38.2.7/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-13 06:37:14.000000 cg-38.2.7/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-13 06:37:14.000000 cg-38.2.7/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-07-13 06:37:14.000000 cg-38.2.7/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-13 06:37:14.000000 cg-38.2.7/tests/utils/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-13 06:37:14.000000 cg-38.2.7/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 09:57:12.000000 cg-38.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-13 09:57:23.000000 cg-38.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-13 09:57:12.000000 cg-38.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 09:57:12.000000 cg-38.2.8/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/dragen_demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/db/models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/demultiplex/sample_sheet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-13 09:57:12.000000 cg-38.2.8/cg/apps/tb/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20219 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/demultiplex/sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/set/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/set/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/upload/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/taxprofiler/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-13 09:57:12.000000 cg-38.2.8/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 09:57:12.000000 cg-38.2.8/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-13 09:57:12.000000 cg-38.2.8/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-13 09:57:12.000000 cg-38.2.8/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-13 09:57:12.000000 cg-38.2.8/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-13 09:57:12.000000 cg-38.2.8/cg/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-13 09:57:12.000000 cg-38.2.8/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-13 09:57:12.000000 cg-38.2.8/cg/io/validate_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-13 09:57:12.000000 cg-38.2.8/cg/io/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-13 09:57:12.000000 cg-38.2.8/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/archive/ddn_dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28769 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/demultiplex/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/demultiplex/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/demultiplex/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/rnafusion_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/report/report_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/report/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77763 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/report/templates/mip-dna_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    78381 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/report/templates/rnafusion_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/upload/upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26030 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13526 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-13 09:57:12.000000 cg-38.2.8/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12662 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/rnafusion/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/rnafusion/command_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/rnafusion/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/taxprofiler/taxprofiler_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-13 09:57:12.000000 cg-38.2.8/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-07-13 09:57:12.000000 cg-38.2.8/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-13 09:57:12.000000 cg-38.2.8/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-13 09:57:12.000000 cg-38.2.8/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 09:57:12.000000 cg-38.2.8/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29392 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38740 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_metrics_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31064 2023-07-13 09:57:12.000000 cg-38.2.8/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-13 09:57:12.000000 cg-38.2.8/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-13 09:57:22.000000 cg-38.2.8/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    44334 2023-07-13 09:57:23.000000 cg-38.2.8/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:57:22.000000 cg-38.2.8/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 09:57:23.000000 cg-38.2.8/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:57:22.000000 cg-38.2.8/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-13 09:57:23.000000 cg-38.2.8/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-13 09:57:23.000000 cg-38.2.8/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-13 09:57:12.000000 cg-38.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 09:57:12.000000 cg-38.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:57:23.000000 cg-38.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-13 09:57:12.000000 cg-38.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/demultiplex/test_dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/demultiplex/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/demultiplex/test_read_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/demultiplex/test_sample_sheet_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/demultiplex/test_sample_sheet_creator_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/lims/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/lims/test_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/sequencing_metrics_parser/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/sequencing_metrics_parser/parsers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-13 09:57:12.000000 cg-38.2.8/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/delete/test_cli_delete_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/set/test_cli_set_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/test_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/upload/test_cli_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/microsalt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/taxprofiler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-13 09:57:12.000000 cg-38.2.8/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93683 2023-07-13 09:57:12.000000 cg-38.2.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/analysis/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/demuxcomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/copy_complete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/CopyComplete.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RTAComplete.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunCompletionStatus.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    79276 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunInfo.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4459 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/run_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/sequencing_metrics_parser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/cgweb_orders/rnafusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/io/example_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/io/example_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/io/example_xml.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   257895 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/1508.28.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257305 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/1508.28.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257516 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/1508.28.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257046 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/1508.28.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257619 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/1508.28.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257428 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/1508.28.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257569 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/1508.28.rnafusion.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   165243 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/1604.17.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88532 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/1605.11.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-13 09:57:12.000000 cg-38.2.8/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-13 09:57:12.000000 cg-38.2.8/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-07-13 09:57:12.000000 cg-38.2.8/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-13 09:57:12.000000 cg-38.2.8/tests/io/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-13 09:57:12.000000 cg-38.2.8/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-13 09:57:12.000000 cg-38.2.8/tests/io/test_io_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-13 09:57:12.000000 cg-38.2.8/tests/io/test_io_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-13 09:57:12.000000 cg-38.2.8/tests/io/test_validate_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/clean/test_clean_flow_cell_run_directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/clean/test_remove_old_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29487 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/demultiplex/test_rename_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/demultiplex/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/demultiplex/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/demultiplex/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/demultiplex/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/demultiplex/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/orders/test_rnafusion_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/report/test_report_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/report/test_rnafusion_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/gisaid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32110 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-13 09:57:12.000000 cg-38.2.8/tests/meta/workflow/test_rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-13 09:57:12.000000 cg-38.2.8/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/demultiplexing/test_flowcell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/demultiplexing/test_run_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-13 09:57:12.000000 cg-38.2.8/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-13 09:57:12.000000 cg-38.2.8/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-13 09:57:12.000000 cg-38.2.8/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-13 09:57:12.000000 cg-38.2.8/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-13 09:57:12.000000 cg-38.2.8/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_metrics_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29863 2023-07-13 09:57:12.000000 cg-38.2.8/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-13 09:57:12.000000 cg-38.2.8/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:23.000000 cg-38.2.8/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:57:12.000000 cg-38.2.8/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 09:57:12.000000 cg-38.2.8/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-13 09:57:12.000000 cg-38.2.8/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-13 09:57:12.000000 cg-38.2.8/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-13 09:57:12.000000 cg-38.2.8/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-07-13 09:57:12.000000 cg-38.2.8/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-13 09:57:12.000000 cg-38.2.8/tests/utils/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-13 09:57:12.000000 cg-38.2.8/tests/utils/test_utils.py
```

### Comparing `cg-38.2.7/PKG-INFO` & `cg-38.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 38.2.7
+Version: 38.2.8
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-38.2.7/README.md` & `cg-38.2.8/README.md`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/crud/create.py` & `cg-38.2.8/cg/apps/cgstats/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/crud/delete.py` & `cg-38.2.8/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/crud/find.py` & `cg-38.2.8/cg/apps/cgstats/crud/find.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/db/models/base.py` & `cg-38.2.8/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/db/models/datasource.py` & `cg-38.2.8/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/db/models/demux.py` & `cg-38.2.8/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/db/models/demux_sample.py` & `cg-38.2.8/cg/apps/cgstats/db/models/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/db/models/dragen_demux_sample.py` & `cg-38.2.8/cg/apps/cgstats/db/models/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/db/models/sample.py` & `cg-38.2.8/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/db/models/support_params.py` & `cg-38.2.8/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/db/models/unaligned.py` & `cg-38.2.8/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/db/models/version.py` & `cg-38.2.8/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-38.2.8/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-38.2.8/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/parsers/demux_stats.py` & `cg-38.2.8/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-38.2.8/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-38.2.8/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/parsers/run_info.py` & `cg-38.2.8/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/cgstats/stats.py` & `cg-38.2.8/cg/apps/cgstats/stats.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/coverage/api.py` & `cg-38.2.8/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/crunchy/crunchy.py` & `cg-38.2.8/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/crunchy/files.py` & `cg-38.2.8/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/crunchy/sbatch.py` & `cg-38.2.8/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/demultiplex/demultiplex_api.py` & `cg-38.2.8/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/demultiplex/demux_report.py` & `cg-38.2.8/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/demultiplex/sample_sheet/create.py` & `cg-38.2.8/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/demultiplex/sample_sheet/dummy_sample.py` & `cg-38.2.8/cg/apps/demultiplex/sample_sheet/dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/demultiplex/sample_sheet/index.py` & `cg-38.2.8/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/demultiplex/sample_sheet/models.py` & `cg-38.2.8/cg/apps/demultiplex/sample_sheet/models.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py` & `cg-38.2.8/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,16 +34,19 @@
     sample_by_lane: Dict[int, List[FlowCellSample]] = get_samples_by_lane(samples)
     for lane, lane_samples in sample_by_lane.items():
         LOG.info(f"Validate that samples are unique in lane {lane}")
         validate_samples_are_unique(samples=lane_samples)
 
 
 def is_valid_sample_internal_id(sample_internal_id: str) -> bool:
-    """Check if a sample internal id has the correct structure."""
-    return bool(re.search(r"[A-Za-z]{3}\d{3}", sample_internal_id))
+    """
+    Check if a sample internal id has the correct structure:
+    starts with three letters followed by at least three digits.
+    """
+    return bool(re.search(r"^[A-Za-z]{3}\d{3}", sample_internal_id))
 
 
 def get_sample_sheet_from_file(
     infile: Path,
     flow_cell_sample_type: Type[FlowCellSample],
 ) -> SampleSheet:
     """Parse and validate a sample sheet from file."""
@@ -106,18 +109,19 @@
         if sample.lane not in sample_by_lane:
             sample_by_lane[sample.lane] = []
         sample_by_lane[sample.lane].append(sample)
     return sample_by_lane
 
 
 def get_sample_internal_ids_from_sample_sheet(
-    sample_sheet_path: Path, flow_cell_type: Type[FlowCellSample]
+    sample_sheet_path: Path, flow_cell_sample_type: Type[FlowCellSample]
 ) -> List[str]:
     """Return the sample internal ids for samples in the sample sheet."""
     sample_sheet = get_sample_sheet_from_file(
-        infile=sample_sheet_path, flow_cell_sample_type=flow_cell_type
+        infile=sample_sheet_path, flow_cell_sample_type=flow_cell_sample_type
     )
     sample_internal_ids: List[str] = []
     for sample in sample_sheet.samples:
-        if is_valid_sample_internal_id(sample_internal_id=sample.sample_id):
-            sample_internal_ids.append(sample.sample_id)
+        sample_internal_id = sample.sample_id.split("_")[0]
+        if is_valid_sample_internal_id(sample_internal_id=sample_internal_id):
+            sample_internal_ids.append(sample_internal_id)
     return list(set(sample_internal_ids))
```

### Comparing `cg-38.2.7/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py` & `cg-38.2.8/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/demultiplex/sbatch.py` & `cg-38.2.8/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/gens.py` & `cg-38.2.8/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/gt.py` & `cg-38.2.8/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/hermes/hermes_api.py` & `cg-38.2.8/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/hermes/models.py` & `cg-38.2.8/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/housekeeper/hk.py` & `cg-38.2.8/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/invoice/render.py` & `cg-38.2.8/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-38.2.8/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-38.2.8/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-38.2.8/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-38.2.8/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/lims/api.py` & `cg-38.2.8/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/lims/batch.py` & `cg-38.2.8/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/lims/order.py` & `cg-38.2.8/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/lims/sample_sheet.py` & `cg-38.2.8/cg/apps/lims/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/loqus.py` & `cg-38.2.8/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/madeline/api.py` & `cg-38.2.8/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/mip/confighandler.py` & `cg-38.2.8/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/mutacc_auto.py` & `cg-38.2.8/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/orderform/excel_orderform_parser.py` & `cg-38.2.8/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/orderform/json_orderform_parser.py` & `cg-38.2.8/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/orderform/orderform_parser.py` & `cg-38.2.8/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/osticket.py` & `cg-38.2.8/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/scout/scout_export.py` & `cg-38.2.8/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/scout/scoutapi.py` & `cg-38.2.8/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/sequencing_metrics_parser/api.py` & `cg-38.2.8/cg/apps/sequencing_metrics_parser/api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py` & `cg-38.2.8/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/sequencing_metrics_parser/models/bcl_convert.py` & `cg-38.2.8/cg/apps/sequencing_metrics_parser/models/bcl_convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 class BclConvertDemuxMetrics(BaseModel):
     """Model for the BCL Convert demultiplexing metrics."""
 
     lane: int = Field(..., alias=BclConvertDemuxMetricsColumnNames.LANE.value)
     sample_internal_id: str = Field(
         ..., alias=BclConvertDemuxMetricsColumnNames.SAMPLE_INTERNAL_ID.value
     )
-    sample_project: str = Field(..., alias=BclConvertDemuxMetricsColumnNames.SAMPLE_PROJECT.value)
     read_pair_count: int = Field(..., alias=BclConvertDemuxMetricsColumnNames.READ_PAIR_COUNT.value)
     perfect_index_reads_count: int = Field(
         ..., alias=BclConvertDemuxMetricsColumnNames.PERFECT_INDEX_READS_COUNT.value
     )
     perfect_index_reads_percent: float = Field(
         ..., alias=BclConvertDemuxMetricsColumnNames.PERFECT_INDEX_READS_PERCENT.value
     )
@@ -57,29 +56,25 @@
 class BclConvertAdapterMetrics(BaseModel):
     """Model for the BCL Convert adapter metrics."""
 
     lane: int = Field(..., alias=BclConvertAdapterMetricsColumnNames.LANE.value)
     sample_internal_id: str = Field(
         ..., alias=BclConvertAdapterMetricsColumnNames.SAMPLE_INTERNAL_ID.value
     )
-    sample_project: str = Field(..., alias=BclConvertAdapterMetricsColumnNames.SAMPLE_PROJECT.value)
     read_number: int = Field(..., alias=BclConvertAdapterMetricsColumnNames.READ_NUMBER.value)
     sample_bases: int = Field(..., alias=BclConvertAdapterMetricsColumnNames.SAMPLE_BASES.value)
 
 
 class BclConvertSampleSheetData(BaseModel):
     """Model for the BCL Convert sample sheet."""
 
     flow_cell_name: str = Field(..., alias=SampleSheetNovaSeq6000Sections.Data.FLOW_CELL_ID.value)
     lane: int = Field(..., alias=SampleSheetNovaSeq6000Sections.Data.LANE.value)
     sample_internal_id: str = Field(
         ..., alias=SampleSheetNovaSeq6000Sections.Data.SAMPLE_INTERNAL_ID_BCLCONVERT.value
     )
     sample_name: str = Field(..., alias=SampleSheetNovaSeq6000Sections.Data.SAMPLE_NAME.value)
     control: str = Field(..., alias=SampleSheetNovaSeq6000Sections.Data.CONTROL.value)
-    sample_project: str = Field(
-        ..., alias=SampleSheetNovaSeq6000Sections.Data.SAMPLE_PROJECT_BCLCONVERT.value
-    )
 
 
 class CustomConfig(BaseConfig):
     arbitrary_types_allowed = True
```

### Comparing `cg-38.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py` & `cg-38.2.8/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py` & `cg-38.2.8/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py` & `cg-38.2.8/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """This module parses metrics for files generated by the BCLConvert tool using the Dragen hardware."""
 import csv
 import re
 import logging
 from pathlib import Path
 from typing import List, Union, Dict, Callable
 from cg.io.controller import ReadFile
-from cg.constants.demultiplexing import SampleSheetNovaSeq6000Sections
+
 from cg.constants.constants import FileFormat, SCALE_TO_READ_PAIRS
+
 from cg.constants.bcl_convert_metrics import (
     DEMUX_METRICS_FILE_NAME,
     QUALITY_METRICS_FILE_NAME,
     ADAPTER_METRICS_FILE_NAME,
-    SAMPLE_SHEET_FILE_NAME,
 )
 from cg.apps.sequencing_metrics_parser.models.bcl_convert import (
     BclConvertAdapterMetrics,
     BclConvertDemuxMetrics,
     BclConvertQualityMetrics,
-    BclConvertSampleSheetData,
 )
-from cg.constants.demultiplexing import INDEX_CHECK, UNDETERMINED
+from cg.apps.demultiplex.sample_sheet.read_sample_sheet import (
+    is_valid_sample_internal_id,
+)
 from cg.utils.files import get_file_in_directory
 
 LOG = logging.getLogger(__name__)
 
 
 class BclConvertMetricsParser:
     def __init__(
@@ -37,91 +38,52 @@
         )
         self.demux_metrics_path: Path = get_file_in_directory(
             directory=self.bcl_convert_demultiplex_dir, file_name=DEMUX_METRICS_FILE_NAME
         )
         self.adapter_metrics_path: Path = get_file_in_directory(
             directory=self.bcl_convert_demultiplex_dir, file_name=ADAPTER_METRICS_FILE_NAME
         )
-        self.sample_sheet_path: Path = get_file_in_directory(
-            directory=self.bcl_convert_demultiplex_dir, file_name=SAMPLE_SHEET_FILE_NAME
-        )
         self.quality_metrics: List[BclConvertQualityMetrics] = self.parse_metrics_file(
             metrics_file_path=self.quality_metrics_path,
             metrics_model=BclConvertQualityMetrics,
         )
         self.demux_metrics: List[BclConvertDemuxMetrics] = self.parse_metrics_file(
             metrics_file_path=self.demux_metrics_path,
             metrics_model=BclConvertDemuxMetrics,
         )
         self.adapter_metrics: List[BclConvertAdapterMetrics] = self.parse_metrics_file(
             self.adapter_metrics_path,
             metrics_model=BclConvertAdapterMetrics,
         )
-        self.sample_sheet: List[BclConvertSampleSheetData] = self.parse_sample_sheet_file(
-            sample_sheet_path=self.sample_sheet_path
-        )
 
     def parse_metrics_file(
         self, metrics_file_path, metrics_model: Callable
     ) -> List[Union[BclConvertQualityMetrics, BclConvertDemuxMetrics, BclConvertAdapterMetrics]]:
         """Parse specified BCL convert metrics file."""
-        if not metrics_file_path.exists():
-            raise FileNotFoundError(f"File {metrics_file_path} does not exist.")
         LOG.info(f"Parsing BCLConvert metrics file: {metrics_file_path}")
         parsed_metrics: List[
             Union[BclConvertQualityMetrics, BclConvertDemuxMetrics, BclConvertAdapterMetrics]
         ] = []
         metrics_content: List[Dict] = ReadFile.get_content_from_file(
             file_format=FileFormat.CSV, file_path=metrics_file_path, read_to_dict=True
         )
         for sample_metrics_dict in metrics_content:
             parsed_metrics.append(metrics_model(**sample_metrics_dict))
         return parsed_metrics
 
-    def get_nr_of_header_lines_in_sample_sheet(self, sample_sheet_path: Path) -> int:
-        """Return the number of header lines in a sample sheet.
-        Any lines before and including the line starting with [Data] is considered the header."""
-        sample_sheet_content = ReadFile.get_content_from_file(FileFormat.CSV, sample_sheet_path)
-        header_line_count: int = 1
-        for line in sample_sheet_content:
-            if SampleSheetNovaSeq6000Sections.Data.HEADER.value in line:
-                break
-            header_line_count += 1
-        return header_line_count
-
-    def parse_sample_sheet_file(self, sample_sheet_path: Path) -> List[BclConvertSampleSheetData]:
-        """Return sample sheet sample lines."""
-        LOG.info(f"Parsing BCLConvert sample sheet file: {sample_sheet_path}")
-        header_line_count: int = self.get_nr_of_header_lines_in_sample_sheet(
-            sample_sheet_path=sample_sheet_path
-        )
-        sample_sheet_sample_lines: List[BclConvertSampleSheetData] = []
-        with open(sample_sheet_path, "r") as sample_sheet_file:
-            for _ in range(header_line_count):
-                next(sample_sheet_file)
-            sample_sheet_content = csv.DictReader(sample_sheet_file)
-            for line in sample_sheet_content:
-                sample_sheet_sample_lines.append(BclConvertSampleSheetData(**line))
-        return sample_sheet_sample_lines
-
     def get_sample_internal_ids(self) -> List[str]:
         """Return a list of sample internal ids."""
         sample_internal_ids: List[str] = []
         for sample_demux_metric in self.demux_metrics:
-            if self.is_valid_sample(sample_internal_id=sample_demux_metric.sample_internal_id):
+            if is_valid_sample_internal_id(
+                sample_internal_id=sample_demux_metric.sample_internal_id
+            ):
                 sample_internal_ids.append(sample_demux_metric.sample_internal_id)
         return list(set(sample_internal_ids))
 
-    def is_valid_sample(self, sample_internal_id: str) -> bool:
-        """Return True if the sample project is valid."""
-        pattern = r"^[A-Za-z]{3}\d{3}.*"
-        if re.match(pattern, sample_internal_id) is not None:
-            return True
-        return False
-
     def get_lanes_for_sample(self, sample_internal_id: str) -> List[int]:
         """Return a list of lanes for a sample."""
         lanes_for_sample: List[int] = []
         for sample_demux_metric in self.demux_metrics:
             if sample_demux_metric.sample_internal_id == sample_internal_id:
                 lanes_for_sample.append(sample_demux_metric.lane)
         return lanes_for_sample
@@ -152,18 +114,14 @@
     def calculate_total_reads_for_sample_in_lane(self, sample_internal_id: str, lane: int) -> int:
         """Calculate the total reads for a sample in a lane."""
         metric: BclConvertDemuxMetrics = self.get_metrics_for_sample_and_lane(
             metrics=self.demux_metrics, sample_internal_id=sample_internal_id, lane=lane
         )
         return metric.read_pair_count * SCALE_TO_READ_PAIRS
 
-    def get_flow_cell_name(self) -> str:
-        """Return the flow cell name of the demultiplexed flow cell."""
-        return self.sample_sheet[0].flow_cell_name
-
     def get_q30_bases_percent_for_sample_in_lane(self, sample_internal_id: str, lane: int) -> float:
         """Return the percent of bases that are Q30 for a sample and lane."""
         metrics: List[BclConvertQualityMetrics] = self.get_read_pair_metrics_for_sample_and_lane(
             sample_internal_id=sample_internal_id, lane=lane
         )
         return self.calculate_mean_read_pair_q30_bases_percent(metrics=metrics)
```

### Comparing `cg-38.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py` & `cg-38.2.8/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Module to parse the BCL convert metrics data into the sequencing statistics model."""
 
 from pathlib import Path
 from typing import List
 from cg.store.models import SampleLaneSequencingMetrics
 from cg.apps.sequencing_metrics_parser.parsers.bcl_convert import BclConvertMetricsParser
+from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from datetime import datetime
+from cg.constants.demultiplexing import BclConverter
 
 
 def create_sample_lane_sequencing_metrics_from_bcl_convert_metrics_for_flow_cell(
     flow_cell_dir: Path,
 ) -> List[SampleLaneSequencingMetrics]:
     """Parse the BCL convert metrics data into the sequencing statistics model."""
     metrics_parser: BclConvertMetricsParser = BclConvertMetricsParser(
@@ -17,15 +19,17 @@
     sample_internal_ids: List[str] = metrics_parser.get_sample_internal_ids()
     sample_lane_sequencing_metrics: List[SampleLaneSequencingMetrics] = []
     for sample_internal_id in sample_internal_ids:
         for lane in metrics_parser.get_lanes_for_sample(sample_internal_id=sample_internal_id):
             sample_lane_sequencing_metrics.append(
                 SampleLaneSequencingMetrics(
                     sample_internal_id=sample_internal_id,
-                    flow_cell_name=metrics_parser.get_flow_cell_name(),
+                    flow_cell_name=FlowCellDirectoryData(
+                        flow_cell_path=flow_cell_dir, bcl_converter=BclConverter.BCLCONVERT
+                    ).flow_cell_name,
                     flow_cell_lane_number=lane,
                     sample_total_reads_in_lane=metrics_parser.calculate_total_reads_for_sample_in_lane(
                         sample_internal_id=sample_internal_id, lane=lane
                     ),
                     sample_base_fraction_passing_q30=metrics_parser.get_q30_bases_percent_for_sample_in_lane(
                         sample_internal_id=sample_internal_id, lane=lane
                     ),
```

### Comparing `cg-38.2.7/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py` & `cg-38.2.8/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/slurm/sbatch.py` & `cg-38.2.8/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/slurm/slurm_api.py` & `cg-38.2.8/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/tb/api.py` & `cg-38.2.8/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/apps/tb/models.py` & `cg-38.2.8/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/add.py` & `cg-38.2.8/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/backup.py` & `cg-38.2.8/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/base.py` & `cg-38.2.8/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/clean.py` & `cg-38.2.8/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/compress/base.py` & `cg-38.2.8/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/compress/fastq.py` & `cg-38.2.8/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/compress/helpers.py` & `cg-38.2.8/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/delete/base.py` & `cg-38.2.8/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/delete/case.py` & `cg-38.2.8/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/delete/cases.py` & `cg-38.2.8/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/delete/observations.py` & `cg-38.2.8/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/deliver/base.py` & `cg-38.2.8/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/demultiplex/add.py` & `cg-38.2.8/cg/cli/demultiplex/add.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/demultiplex/base.py` & `cg-38.2.8/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/demultiplex/demux.py` & `cg-38.2.8/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/demultiplex/finish.py` & `cg-38.2.8/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/demultiplex/report.py` & `cg-38.2.8/cg/cli/demultiplex/report.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/demultiplex/sample_sheet.py` & `cg-38.2.8/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/generate/report/base.py` & `cg-38.2.8/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/generate/report/options.py` & `cg-38.2.8/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/generate/report/utils.py` & `cg-38.2.8/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/get.py` & `cg-38.2.8/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/set/base.py` & `cg-38.2.8/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/set/case.py` & `cg-38.2.8/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/set/cases.py` & `cg-38.2.8/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/store/fastq.py` & `cg-38.2.8/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/store/store.py` & `cg-38.2.8/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/transfer.py` & `cg-38.2.8/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/base.py` & `cg-38.2.8/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/clinical_delivery.py` & `cg-38.2.8/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/coverage.py` & `cg-38.2.8/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/delivery_report.py` & `cg-38.2.8/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/fohm.py` & `cg-38.2.8/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/genotype.py` & `cg-38.2.8/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/gens.py` & `cg-38.2.8/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/gisaid.py` & `cg-38.2.8/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/mutacc.py` & `cg-38.2.8/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/nipt/base.py` & `cg-38.2.8/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/nipt/ftp.py` & `cg-38.2.8/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/nipt/statina.py` & `cg-38.2.8/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/observations/observations.py` & `cg-38.2.8/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/observations/utils.py` & `cg-38.2.8/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/scout.py` & `cg-38.2.8/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/utils.py` & `cg-38.2.8/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/upload/validate.py` & `cg-38.2.8/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/balsamic/base.py` & `cg-38.2.8/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/balsamic/options.py` & `cg-38.2.8/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/balsamic/pon.py` & `cg-38.2.8/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/balsamic/qc.py` & `cg-38.2.8/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/balsamic/umi.py` & `cg-38.2.8/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/base.py` & `cg-38.2.8/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/commands.py` & `cg-38.2.8/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/fastq/base.py` & `cg-38.2.8/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/fluffy/base.py` & `cg-38.2.8/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/microsalt/base.py` & `cg-38.2.8/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/mip/base.py` & `cg-38.2.8/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/mip/options.py` & `cg-38.2.8/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/mip_dna/base.py` & `cg-38.2.8/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/mip_rna/base.py` & `cg-38.2.8/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/mutant/base.py` & `cg-38.2.8/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/nextflow/options.py` & `cg-38.2.8/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/rnafusion/base.py` & `cg-38.2.8/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/rnafusion/options.py` & `cg-38.2.8/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/taxprofiler/base.py` & `cg-38.2.8/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/cli/workflow/taxprofiler/options.py` & `cg-38.2.8/cg/cli/workflow/taxprofiler/options.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/__init__.py` & `cg-38.2.8/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/bcl_convert_metrics.py` & `cg-38.2.8/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/compression.py` & `cg-38.2.8/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/constants.py` & `cg-38.2.8/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/delivery.py` & `cg-38.2.8/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/demultiplexing.py` & `cg-38.2.8/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/encryption.py` & `cg-38.2.8/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/gene_panel.py` & `cg-38.2.8/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/housekeeper_tags.py` & `cg-38.2.8/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/lims.py` & `cg-38.2.8/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/nextflow.py` & `cg-38.2.8/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/observations.py` & `cg-38.2.8/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/orderforms.py` & `cg-38.2.8/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/priority.py` & `cg-38.2.8/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/report.py` & `cg-38.2.8/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/rnafusion.py` & `cg-38.2.8/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/scout_upload.py` & `cg-38.2.8/cg/constants/scout_upload.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/sequencing.py` & `cg-38.2.8/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/subject.py` & `cg-38.2.8/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/constants/taxprofiler.py` & `cg-38.2.8/cg/constants/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/exc.py` & `cg-38.2.8/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/io/api.py` & `cg-38.2.8/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/io/controller.py` & `cg-38.2.8/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/io/csv.py` & `cg-38.2.8/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/io/json.py` & `cg-38.2.8/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/io/validate_path.py` & `cg-38.2.8/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/io/xml.py` & `cg-38.2.8/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/io/yaml.py` & `cg-38.2.8/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/archive/ddn_dataflow.py` & `cg-38.2.8/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/backup/backup.py` & `cg-38.2.8/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/backup/pdc.py` & `cg-38.2.8/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/clean/api.py` & `cg-38.2.8/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-38.2.8/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/clean/flow_cell_run_directories.py` & `cg-38.2.8/cg/meta/clean/flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/compress/compress.py` & `cg-38.2.8/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/compress/files.py` & `cg-38.2.8/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/deliver.py` & `cg-38.2.8/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/deliver_ticket.py` & `cg-38.2.8/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-38.2.8/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/demultiplex/demux_post_processing.py` & `cg-38.2.8/cg/meta/demultiplex/demux_post_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 from cg.meta.demultiplex import files
 from cg.meta.demultiplex.utils import (
     create_delivery_file_in_flow_cell_directory,
     get_bcl_converter_name,
     get_lane_from_sample_fastq,
     get_q30_threshold,
     get_sample_fastqs_from_flow_cell,
-    get_sample_internal_ids_from_flow_cell,
     get_sample_sheet_path,
     parse_flow_cell_directory_data,
 )
+from cg.apps.demultiplex.sample_sheet.read_sample_sheet import (
+    get_sample_internal_ids_from_sample_sheet,
+)
 from cg.meta.transfer import TransferFlowCell
 from cg.models.cg_config import CGConfig
 from cg.models.cgstats.stats_sample import StatsSample
 from cg.models.demultiplex.demux_results import DemuxResults
 from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from cg.store import Store
 from cg.store.models import Flowcell, SampleLaneSequencingMetrics
@@ -161,15 +163,18 @@
         )
         self.status_db.session.add(metric)
 
     def update_sample_read_counts_in_status_db(self, flow_cell_data: FlowCellDirectoryData) -> None:
         """Update samples in status db with the sum of all read counts for the sample in the sequencing metrics table."""
 
         q30_threshold: int = get_q30_threshold(flow_cell_data.sequencer_type)
-        sample_internal_ids: List[str] = get_sample_internal_ids_from_flow_cell(flow_cell_data)
+        sample_internal_ids: List[str] = get_sample_internal_ids_from_sample_sheet(
+            sample_sheet_path=flow_cell_data.sample_sheet_path,
+            flow_cell_sample_type=flow_cell_data.sample_type,
+        )
 
         for sample_id in sample_internal_ids:
             self.update_sample_read_count(sample_id=sample_id, q30_threshold=q30_threshold)
 
         self.status_db.session.commit()
 
     def update_sample_read_count(self, sample_id: str, q30_threshold: int) -> None:
@@ -200,15 +205,18 @@
             flow_cell_directory=flow_cell.path, flow_cell_name=flow_cell.id
         )
         self.add_sample_fastq_files_to_housekeeper(flow_cell)
 
     def add_sample_fastq_files_to_housekeeper(self, flow_cell: FlowCellDirectoryData) -> None:
         """Add sample fastq files from flow cell to Housekeeper."""
 
-        sample_internal_ids: List[str] = get_sample_internal_ids_from_flow_cell(flow_cell)
+        sample_internal_ids: List[str] = get_sample_internal_ids_from_sample_sheet(
+            sample_sheet_path=flow_cell.sample_sheet_path,
+            flow_cell_sample_type=flow_cell.sample_type,
+        )
 
         for sample_internal_id in sample_internal_ids:
             self.add_bundle_and_version_if_non_existent(sample_internal_id)
 
             sample_fastq_paths: Optional[List[Path]] = get_sample_fastqs_from_flow_cell(
                 flow_cell_directory=flow_cell.path, sample_internal_id=sample_internal_id
             )
@@ -276,15 +284,17 @@
 
     def add_sample_sheet_path_to_housekeeper(
         self, flow_cell_directory: Path, flow_cell_name: str
     ) -> None:
         """Add sample sheet path to Housekeeper."""
 
         try:
-            sample_sheet_file_path: Path = get_sample_sheet_path(flow_cell_directory)
+            sample_sheet_file_path: Path = get_sample_sheet_path(
+                flow_cell_directory=flow_cell_directory
+            )
 
             self.add_file_to_bundle_if_non_existent(
                 file_path=sample_sheet_file_path,
                 bundle_name=flow_cell_name,
                 tag_names=[SequencingFileTag.SAMPLE_SHEET, flow_cell_name],
             )
         except FileNotFoundError as e:
```

### Comparing `cg-38.2.7/cg/meta/demultiplex/files.py` & `cg-38.2.8/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/demultiplex/utils.py` & `cg-38.2.8/cg/meta/demultiplex/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from cg.constants.constants import FileExtensions
 from cg.constants.demultiplexing import BclConverter, DemultiplexingDirsAndFiles
 from cg.constants.sequencing import FLOWCELL_Q30_THRESHOLD, Sequencers
 from cg.exc import FlowCellError
 from cg.meta.demultiplex.validation import (
     is_bcl2fastq_demux_folder_structure,
     is_flow_cell_directory_valid,
-    is_valid_sample_id,
     is_valid_sample_fastq_file,
 )
 from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
-from cg.utils.utils import get_files_matching_pattern
+
+from cg.utils.files import get_file_in_directory, get_files_matching_pattern
 
 LOG = logging.getLogger(__name__)
 
 
 def get_lane_from_sample_fastq(sample_fastq_path: Path) -> int:
     """
     Extract the lane number from the sample fastq path.
@@ -70,47 +70,24 @@
     return BclConverter.BCLCONVERT
 
 
 def create_delivery_file_in_flow_cell_directory(flow_cell_directory: Path) -> None:
     Path(flow_cell_directory, DemultiplexingDirsAndFiles.DELIVERY).touch()
 
 
-def get_sample_internal_ids_from_flow_cell(flow_cell_data: FlowCellDirectoryData) -> List[str]:
-    samples: List[FlowCellSample] = flow_cell_data.get_sample_sheet().samples
-    return get_valid_sample_ids(samples)
-
-
-def get_valid_sample_ids(samples: List[FlowCellSample]) -> List[str]:
-    """Get all valid sample ids from sample sheet."""
-    valid_sample_ids = [
-        sample.sample_id for sample in samples if is_valid_sample_id(sample.sample_id)
-    ]
-    formatted_sample_ids = [sample_id_index.split("_")[0] for sample_id_index in valid_sample_ids]
-    return formatted_sample_ids
-
-
 def get_q30_threshold(sequencer_type: Sequencers) -> int:
     return FLOWCELL_Q30_THRESHOLD[sequencer_type]
 
 
-def get_sample_sheet_path(flow_cell_directory: Path) -> Path:
-    """
-    Recursively searches for the given sample sheet file in the provided flow cell directory.
-
-    Raises:
-        FileNotFoundError: If the sample sheet file is not found in the flow cell directory.
-    """
-    for directory_path, _, files in os.walk(flow_cell_directory):
-        if DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME in files:
-            LOG.info(f"Found sample sheet in {directory_path}")
-            return Path(directory_path, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME)
-
-    raise FileNotFoundError(
-        f"Sample sheet not found in given flow cell directory: {flow_cell_directory}"
-    )
+def get_sample_sheet_path(
+    flow_cell_directory: Path,
+    sample_sheet_file_name: str = DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME,
+) -> Path:
+    """Return the path to the sample sheet in the flow cell directory."""
+    return get_file_in_directory(directory=flow_cell_directory, file_name=sample_sheet_file_name)
 
 
 def parse_flow_cell_directory_data(
     flow_cell_directory: Path, bcl_converter: str
 ) -> FlowCellDirectoryData:
     """Parse flow cell data from the flow cell directory."""
```

### Comparing `cg-38.2.7/cg/meta/demultiplex/validation.py` & `cg-38.2.8/cg/meta/demultiplex/validation.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,13 +66,7 @@
         raise FlowCellError(
             f"Demultiplexing not completed for flow cell directory {flow_cell_directory}."
         )
 
 
 def is_demultiplexing_complete(flow_cell_directory: Path) -> bool:
     return Path(flow_cell_directory, DemultiplexingDirsAndFiles.DEMUX_COMPLETE).exists()
-
-
-def is_valid_sample_id(sample_id: str) -> bool:
-    sample_id_is_index_check = INDEX_CHECK in sample_id
-    sample_id_is_non_empty = bool(sample_id)
-    return sample_id_is_non_empty and not sample_id_is_index_check
```

### Comparing `cg-38.2.7/cg/meta/encryption/encryption.py` & `cg-38.2.8/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/invoice.py` & `cg-38.2.8/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/meta.py` & `cg-38.2.8/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/observations/balsamic_observations_api.py` & `cg-38.2.8/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/observations/mip_dna_observations_api.py` & `cg-38.2.8/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/observations/observations_api.py` & `cg-38.2.8/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/orders/api.py` & `cg-38.2.8/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/orders/case_submitter.py` & `cg-38.2.8/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/orders/fastq_submitter.py` & `cg-38.2.8/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/orders/lims.py` & `cg-38.2.8/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/orders/metagenome_submitter.py` & `cg-38.2.8/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/orders/microbial_submitter.py` & `cg-38.2.8/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/orders/pool_submitter.py` & `cg-38.2.8/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/orders/rnafusion_submitter.py` & `cg-38.2.8/cg/meta/orders/rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/orders/sars_cov_2_submitter.py` & `cg-38.2.8/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/orders/submitter.py` & `cg-38.2.8/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/orders/ticket_handler.py` & `cg-38.2.8/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/report/balsamic.py` & `cg-38.2.8/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/report/balsamic_umi.py` & `cg-38.2.8/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/report/field_validators.py` & `cg-38.2.8/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/report/mip_dna.py` & `cg-38.2.8/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/report/report_api.py` & `cg-38.2.8/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/report/rnafusion.py` & `cg-38.2.8/cg/meta/report/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/report/templates/balsamic_report.html` & `cg-38.2.8/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/report/templates/bootstrap.html` & `cg-38.2.8/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/report/templates/mip-dna_report.html` & `cg-38.2.8/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/report/templates/rnafusion_report.html` & `cg-38.2.8/cg/meta/report/templates/rnafusion_report.html`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/rsync/rsync_api.py` & `cg-38.2.8/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/tar/tar.py` & `cg-38.2.8/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/transfer/external_data.py` & `cg-38.2.8/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/transfer/flowcell.py` & `cg-38.2.8/cg/meta/transfer/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/transfer/lims.py` & `cg-38.2.8/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/balsamic/balsamic.py` & `cg-38.2.8/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/coverage.py` & `cg-38.2.8/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/fohm/fohm.py` & `cg-38.2.8/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/gisaid/constants.py` & `cg-38.2.8/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/gisaid/gisaid.py` & `cg-38.2.8/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/gisaid/models.py` & `cg-38.2.8/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/gt.py` & `cg-38.2.8/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/mip/mip_dna.py` & `cg-38.2.8/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/mip/mip_rna.py` & `cg-38.2.8/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/mutacc.py` & `cg-38.2.8/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/nipt/nipt.py` & `cg-38.2.8/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/rnafusion/rnafusion.py` & `cg-38.2.8/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-38.2.8/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-38.2.8/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/scout/hk_tags.py` & `cg-38.2.8/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/scout/mip_config_builder.py` & `cg-38.2.8/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-38.2.8/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/scout/scout_config_builder.py` & `cg-38.2.8/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/scout/uploadscoutapi.py` & `cg-38.2.8/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/upload/upload_api.py` & `cg-38.2.8/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/analysis.py` & `cg-38.2.8/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/balsamic.py` & `cg-38.2.8/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/balsamic_pon.py` & `cg-38.2.8/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/balsamic_qc.py` & `cg-38.2.8/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/balsamic_umi.py` & `cg-38.2.8/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/fastq.py` & `cg-38.2.8/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/fluffy.py` & `cg-38.2.8/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/microsalt.py` & `cg-38.2.8/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/mip.py` & `cg-38.2.8/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/mip_dna.py` & `cg-38.2.8/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/mip_rna.py` & `cg-38.2.8/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/mutant.py` & `cg-38.2.8/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/nextflow_common.py` & `cg-38.2.8/cg/meta/workflow/nextflow_common.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/prepare_fastq.py` & `cg-38.2.8/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/rnafusion.py` & `cg-38.2.8/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/taxprofiler.py` & `cg-38.2.8/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/meta/workflow/tower_common.py` & `cg-38.2.8/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/balsamic/config.py` & `cg-38.2.8/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/balsamic/metrics.py` & `cg-38.2.8/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/cg_config.py` & `cg-38.2.8/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/cgstats/stats_sample.py` & `cg-38.2.8/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/compression_data.py` & `cg-38.2.8/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/deliverables/metric_deliverables.py` & `cg-38.2.8/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/demultiplex/demux_results.py` & `cg-38.2.8/cg/models/demultiplex/demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/demultiplex/flow_cell.py` & `cg-38.2.8/cg/models/demultiplex/flow_cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from cg.constants.sequencing import Sequencers, sequencer_types
 from cg.exc import FlowCellError, SampleSheetError
 from cg.models.demultiplex.run_parameters import (
     RunParameters,
     RunParametersNovaSeq6000,
     RunParametersNovaSeqX,
 )
+from cg.utils.files import get_file_in_directory
 
 LOG = logging.getLogger(__name__)
 
 
 class FlowCellDirectoryData:
     """Class to collect information about flow cell directories and their particular files."""
 
@@ -40,48 +41,52 @@
         self._run_parameters: Optional[RunParameters] = None
         self.run_date: datetime.datetime = datetime.datetime.now()
         self.machine_name: str = ""
         self.machine_number: int = 0
         self.base_name: str = ""  # Base name is flow cell-id + flow cell position
         self.id: str = ""
         self.position: Literal["A", "B"] = "A"
-        self.parse_flow_cell_name()
+        self.flow_cell_name: str = ""
+        self.parse_flow_cell_dir_name()
 
-    def parse_flow_cell_name(self):
+    def parse_flow_cell_dir_name(self):
         """Parse relevant information from flow cell name.
 
         This will assume that the flow cell naming convention is used. If not we skip the flow cell.
         Convention is: <date>_<machine>_<run_numbers>_<A|B><flow_cell_id>
         Example: '201203_A00689_0200_AHVKJCDRXX'.
         """
 
-        self.validate_flow_cell_name()
+        self.validate_flow_cell_dir_name()
         self.run_date = self._parse_date()
         self.machine_name = self.split_flow_cell_name[1]
         self.machine_number = int(self.split_flow_cell_name[2])
         base_name: str = self.split_flow_cell_name[-1]
         self.base_name = base_name
         LOG.debug(f"Set flow cell id to {base_name}")
         self.id = base_name[1:]
         self.position = base_name[0]
+        self.flow_cell_name = base_name[1:]
 
     @property
     def split_flow_cell_name(self) -> List[str]:
         """Return split flow cell name."""
         return self.path.name.split("_")
 
     @property
     def full_name(self) -> str:
         """Return flow cell full name."""
         return self.path.name
 
     @property
     def sample_sheet_path(self) -> Path:
-        """Return sample sheet path."""
-        return Path(self.path, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME)
+        """
+        Return sample sheet path.
+        """
+        return Path(self.path, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME.value)
 
     @property
     def run_parameters_path(self) -> Path:
         """Return path to run parameters file."""
         return Path(self.path, DemultiplexingDirsAndFiles.RUN_PARAMETERS)
 
     @property
@@ -165,15 +170,15 @@
 
     def _parse_date(self):
         """Return the parsed date in the correct format."""
         if len(self.split_flow_cell_name[0]) == LENGTH_LONG_DATE:
             return datetime.datetime.strptime(self.split_flow_cell_name[0], "%Y%m%d")
         return datetime.datetime.strptime(self.split_flow_cell_name[0], "%y%m%d")
 
-    def validate_flow_cell_name(self) -> None:
+    def validate_flow_cell_dir_name(self) -> None:
         """
         Validate on the following criteria:
         Convention is: <date>_<machine>_<run_numbers>_<A|B><flow_cell_id>
         Example: '201203_A00689_0200_AHVKJCDRXX'.
         """
         if len(self.split_flow_cell_name) != 4:
             message = f"Flowcell {self.full_name} does not follow the flow cell naming convention"
```

### Comparing `cg-38.2.7/cg/models/demultiplex/run_parameters.py` & `cg-38.2.8/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/demultiplex/sbatch.py` & `cg-38.2.8/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/file_data.py` & `cg-38.2.8/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/invoice/invoice.py` & `cg-38.2.8/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/lims/sample.py` & `cg-38.2.8/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/mip/mip_config.py` & `cg-38.2.8/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/mip/mip_metrics_deliverables.py` & `cg-38.2.8/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/mip/mip_sample_info.py` & `cg-38.2.8/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/nextflow/deliverables.py` & `cg-38.2.8/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/nextflow/sample.py` & `cg-38.2.8/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/observations/input_files.py` & `cg-38.2.8/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/orders/constants.py` & `cg-38.2.8/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/orders/excel_sample.py` & `cg-38.2.8/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/orders/json_sample.py` & `cg-38.2.8/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/orders/order.py` & `cg-38.2.8/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/orders/orderform_schema.py` & `cg-38.2.8/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/orders/sample_base.py` & `cg-38.2.8/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/orders/samples.py` & `cg-38.2.8/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/report/metadata.py` & `cg-38.2.8/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/report/report.py` & `cg-38.2.8/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/report/sample.py` & `cg-38.2.8/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/report/validators.py` & `cg-38.2.8/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/rnafusion/command_args.py` & `cg-38.2.8/cg/models/rnafusion/command_args.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/rnafusion/metrics.py` & `cg-38.2.8/cg/models/rnafusion/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/rnafusion/rnafusion_sample.py` & `cg-38.2.8/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/scout/scout_load_config.py` & `cg-38.2.8/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/slurm/sbatch.py` & `cg-38.2.8/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/models/workflow/mutant.py` & `cg-38.2.8/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/resources/20181012_Indices.csv` & `cg-38.2.8/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/resources/rnafusion_bundle_filenames.csv` & `cg-38.2.8/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/server/admin.py` & `cg-38.2.8/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/server/api.py` & `cg-38.2.8/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/server/app.py` & `cg-38.2.8/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/server/config.py` & `cg-38.2.8/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/server/ext.py` & `cg-38.2.8/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/server/invoices/templates/invoices/index.html` & `cg-38.2.8/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/server/invoices/templates/invoices/invoice.html` & `cg-38.2.8/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/server/invoices/templates/invoices/layout.html` & `cg-38.2.8/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/server/invoices/templates/invoices/new.html` & `cg-38.2.8/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/server/invoices/views.py` & `cg-38.2.8/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/api/add.py` & `cg-38.2.8/cg/store/api/add.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/api/base.py` & `cg-38.2.8/cg/store/api/base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/api/core.py` & `cg-38.2.8/cg/store/api/core.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/api/delete.py` & `cg-38.2.8/cg/store/api/delete.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/api/find_basic_data.py` & `cg-38.2.8/cg/store/api/find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/api/find_business_data.py` & `cg-38.2.8/cg/store/api/find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/api/status.py` & `cg-38.2.8/cg/store/api/status.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_analysis_filters.py` & `cg-38.2.8/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_application_filters.py` & `cg-38.2.8/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_application_version_filters.py` & `cg-38.2.8/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_bed_filters.py` & `cg-38.2.8/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_bed_version_filters.py` & `cg-38.2.8/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_case_filters.py` & `cg-38.2.8/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_case_sample_filters.py` & `cg-38.2.8/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_collaboration_filters.py` & `cg-38.2.8/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_customer_filters.py` & `cg-38.2.8/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_flow_cell_filters.py` & `cg-38.2.8/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_invoice_filters.py` & `cg-38.2.8/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_metrics_filters.py` & `cg-38.2.8/cg/store/filters/status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_organism_filters.py` & `cg-38.2.8/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_panel_filters.py` & `cg-38.2.8/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_pool_filters.py` & `cg-38.2.8/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_sample_filters.py` & `cg-38.2.8/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/filters/status_user_filters.py` & `cg-38.2.8/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/store/models.py` & `cg-38.2.8/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/utils/checksum/checksum.py` & `cg-38.2.8/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/utils/click/EnumChoice.py` & `cg-38.2.8/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/utils/commands.py` & `cg-38.2.8/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/utils/date.py` & `cg-38.2.8/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/utils/dict.py` & `cg-38.2.8/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/utils/dispatcher.py` & `cg-38.2.8/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/utils/email.py` & `cg-38.2.8/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/utils/files.py` & `cg-38.2.8/cg/utils/files.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """Some helper functions for working with files"""
 from pathlib import Path
-from typing import Optional
 import os
+from typing import List
 
 
 def get_file_in_directory(directory: Path, file_name: str) -> Path:
     """Get a file in a directory and subdirectories.
     Raises:
         FileNotFoundError: If the directory does not exist.
     """
     if not directory.is_dir() or not directory.exists():
         raise FileNotFoundError(f"Directory {directory} does not exist")
     for directory_path, _, files in os.walk(directory):
         for file in files:
             if file_name == file:
                 path_to_file = Path(directory_path, file)
                 return path_to_file
+    raise FileNotFoundError(f"File {file_name} not found in {directory}")
+
+
+def get_files_matching_pattern(directory: Path, pattern: str) -> List[Path]:
+    """Search for all files in a directory that match a pattern."""
+    return list(directory.glob(pattern))
```

### Comparing `cg-38.2.7/cg/utils/flask/enum.py` & `cg-38.2.8/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/cg/utils/utils.py` & `cg-38.2.8/cg/utils/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,12 +28,7 @@
 
     Raises:
         KeyError: When the strings have the same length.
     """
     if len(str_1) != len(str_2):
         raise KeyError("The two strings must have the same length to calculate distance!")
     return sum(n1 != n2 for n1, n2 in zip(str_1, str_2))
-
-
-def get_files_matching_pattern(directory: Path, pattern: str) -> List[Path]:
-    """Search for all files in a directory that match a pattern."""
-    return list(directory.glob(pattern))
```

### Comparing `cg-38.2.7/cg.egg-info/PKG-INFO` & `cg-38.2.8/cg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 38.2.7
+Version: 38.2.8
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-38.2.7/cg.egg-info/SOURCES.txt` & `cg-38.2.8/cg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -793,18 +793,18 @@
 tests/fixtures/apps/scout/643594.config.yaml
 tests/fixtures/apps/scout/case_export.json
 tests/fixtures/apps/scout/export_causatives.json
 tests/fixtures/apps/scout/none_case_export.json
 tests/fixtures/apps/scout/other_sex_case.json
 tests/fixtures/apps/scout/panel_export.bed
 tests/fixtures/apps/scout/panel_export.csv
-tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Adapter_Metrics.csv
-tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Demultiplex_Stats.csv
-tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Quality_Metrics.csv
-tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/SampleSheet.csv
+tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
 tests/fixtures/apps/shipping/scout-deploy.yaml
 tests/fixtures/cgweb_orders/balsamic.json
 tests/fixtures/cgweb_orders/fastq.json
 tests/fixtures/cgweb_orders/metagenome.json
 tests/fixtures/cgweb_orders/microsalt.json
 tests/fixtures/cgweb_orders/mip.json
 tests/fixtures/cgweb_orders/mip_rna.json
@@ -868,14 +868,15 @@
 tests/meta/demultiplex/conftest.py
 tests/meta/demultiplex/test_delete_demultiplex_api.py
 tests/meta/demultiplex/test_demux_post_processing.py
 tests/meta/demultiplex/test_rename_files.py
 tests/meta/demultiplex/test_utils.py
 tests/meta/demultiplex/test_validation.py
 tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+tests/meta/demultiplex/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
 tests/meta/encryption/conftest.py
 tests/meta/encryption/test_encryption.py
 tests/meta/observations/conftest.py
 tests/meta/observations/test_meta_upload_observations.py
 tests/meta/orders/conftest.py
 tests/meta/orders/test_PoolSubmitter_validate_order.py
 tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
@@ -1012,15 +1013,14 @@
 tests/store/filters/test_status_invoice_filters.py
 tests/store/filters/test_status_metrics_filters.py
 tests/store/filters/test_status_organism_filters.py
 tests/store/filters/test_status_panel_filters.py
 tests/store/filters/test_status_pool_filters.py
 tests/store/filters/test_status_samples_filters.py
 tests/store/filters/test_status_user_filters.py
-tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
 tests/tests/fixtures/data/fastq.fastq.gz
 tests/utils/__init__.py
 tests/utils/conftest.py
 tests/utils/test_commands.py
 tests/utils/test_date.py
 tests/utils/test_dict.py
 tests/utils/test_dispatcher.py
```

### Comparing `cg-38.2.7/requirements.txt` & `cg-38.2.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/setup.py` & `cg-38.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="38.2.7",
+    version="38.2.8",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-38.2.7/tests/apps/cgstats/conftest.py` & `cg-38.2.8/tests/apps/cgstats/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-38.2.8/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/cgstats/crud/test_delete.py` & `cg-38.2.8/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-38.2.8/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-38.2.8/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/cgstats/parsers/test_run_info.py` & `cg-38.2.8/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/cgstats/test_cgstats_create.py` & `cg-38.2.8/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/cgstats/test_stats.py` & `cg-38.2.8/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/conftest.py` & `cg-38.2.8/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/coverage/test_coverage.py` & `cg-38.2.8/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/crunchy/conftest.py` & `cg-38.2.8/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/crunchy/test_compress_fastq.py` & `cg-38.2.8/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/crunchy/test_config.py` & `cg-38.2.8/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/crunchy/test_crunchy.py` & `cg-38.2.8/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/crunchy/test_spring_decompression.py` & `cg-38.2.8/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/demultiplex/conftest.py` & `cg-38.2.8/tests/apps/demultiplex/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,11 +353,12 @@
 def fixture_novaseq6000_sample_sheet_path() -> Path:
     """Return the path to a NovaSeq 6000 BCL convert sample sheet."""
     return Path(
         "tests",
         "fixtures",
         "apps",
         "sequencing_metrics_parser",
+        "230622_A00621_0864_AHY7FFDRX2",
         "Unaligned",
         "Reports",
         "SampleSheet.csv",
     )
```

### Comparing `cg-38.2.7/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-38.2.8/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/demultiplex/test_dummy_sample.py` & `cg-38.2.8/tests/apps/demultiplex/test_dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/demultiplex/test_index.py` & `cg-38.2.8/tests/apps/demultiplex/test_index.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/demultiplex/test_read_sample_sheet.py` & `cg-38.2.8/tests/apps/demultiplex/test_read_sample_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 ):
     """Test that getting sample internal ids from a sample sheet returns a unique list of strings."""
     # GIVEN a path to a sample sheet with only valid samples
 
     # WHEN getting the valid sample internal ids
     sample_internal_ids: List[str] = get_sample_internal_ids_from_sample_sheet(
         sample_sheet_path=novaseq6000_bcl_convert_sample_sheet_path,
-        flow_cell_type=flow_cell_type,
+        flow_cell_sample_type=flow_cell_type,
     )
 
     # THEN the returned value is a list
     assert isinstance(sample_internal_ids, List)
     # THEN the list contains strings
     assert isinstance(sample_internal_ids[0], str)
     # THEN the sample internal ids are unique
```

### Comparing `cg-38.2.7/tests/apps/demultiplex/test_sample_sheet_creator.py` & `cg-38.2.8/tests/apps/demultiplex/test_sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/demultiplex/test_sample_sheet_creator_factory.py` & `cg-38.2.8/tests/apps/demultiplex/test_sample_sheet_creator_factory.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/gens/test_gens_api.py` & `cg-38.2.8/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/gt/conftest.py` & `cg-38.2.8/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/gt/test_gt_api.py` & `cg-38.2.8/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/hk/conftest.py` & `cg-38.2.8/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/hk/test__getattr__.py` & `cg-38.2.8/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/hk/test_add_file.py` & `cg-38.2.8/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/hk/test_bundles.py` & `cg-38.2.8/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/hk/test_core.py` & `cg-38.2.8/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/hk/test_file.py` & `cg-38.2.8/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/hk/test_version.py` & `cg-38.2.8/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/lims/conftest.py` & `cg-38.2.8/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/lims/test_api.py` & `cg-38.2.8/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/lims/test_sample_sheet.py` & `cg-38.2.8/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/loqus/conftest.py` & `cg-38.2.8/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/loqus/test_loqusdb_api.py` & `cg-38.2.8/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/madeline/conftest.py` & `cg-38.2.8/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/madeline/test_madeline.py` & `cg-38.2.8/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/mip/conftest.py` & `cg-38.2.8/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/mip/test_config_mip.py` & `cg-38.2.8/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/mutacc_auto/conftest.py` & `cg-38.2.8/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-38.2.8/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/orderform/conftest.py` & `cg-38.2.8/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-38.2.8/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/orderform/test_excel_sample_schema.py` & `cg-38.2.8/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/orderform/test_json_orderform_parser.py` & `cg-38.2.8/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/orderform/test_orderform_parser.py` & `cg-38.2.8/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/scout/conftest.py` & `cg-38.2.8/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/scout/test_get_causative_variants.py` & `cg-38.2.8/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/scout/test_get_scout_cases.py` & `cg-38.2.8/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/scout/test_scout_load_config.py` & `cg-38.2.8/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/scout/test_scout_models.py` & `cg-38.2.8/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-38.2.8/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from cg.store.models import SampleLaneSequencingMetrics
 from datetime import datetime
 
 
 @pytest.fixture(name="bcl_convert_metrics_dir_path", scope="session")
 def fixture_bcl_convert_metrics_dir_path() -> Path:
     """Return a path to a BCLConvert metrics directory."""
-    return Path("tests", "fixtures", "apps", "sequencing_metrics_parser")
+    return Path(
+        "tests", "fixtures", "apps", "sequencing_metrics_parser", "230622_A00621_0864_AHY7FFDRX2"
+    )
 
 
 @pytest.fixture(name="test_sample_internal_id", scope="session")
 def fixture_test_sample_internal_id() -> str:
     """Return a test sample internal id."""
     return "ACC11927A2"
```

### Comparing `cg-38.2.7/tests/apps/sequencing_metrics_parser/parsers/conftest.py` & `cg-38.2.8/tests/apps/sequencing_metrics_parser/parsers/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py` & `cg-38.2.8/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py` & `cg-38.2.8/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-38.2.8/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,16 +24,15 @@
     )
 
     # THEN assert that the metrics are parsed
     assert bcl_convert_metrics_parser.quality_metrics
     assert isinstance(bcl_convert_metrics_parser.quality_metrics[0], BclConvertQualityMetrics)
     assert bcl_convert_metrics_parser.demux_metrics
     assert isinstance(bcl_convert_metrics_parser.demux_metrics[0], BclConvertDemuxMetrics)
-    assert bcl_convert_metrics_parser.sample_sheet
-    assert isinstance(bcl_convert_metrics_parser.sample_sheet[0], BclConvertSampleSheetData)
+
     assert bcl_convert_metrics_parser.adapter_metrics
     assert isinstance(bcl_convert_metrics_parser.adapter_metrics[0], BclConvertAdapterMetrics)
 
 
 def test_parse_metrics_files_not_existing():
     """Test to parse BCLConvert metrics with non-existing path."""
     # GIVEN paths to a BCLConvert metrics files that do not exist
@@ -92,32 +91,14 @@
     assert isinstance(demux_metrics_model, BclConvertDemuxMetrics)
 
     # ASSERT that the parsed demux metrics has the correct values
     for attr_name, attr_value in demux_metrics_model.dict().items():
         assert getattr(bcl_convert_demux_metric_model_with_data, attr_name) == attr_value
 
 
-def test_parse_bcl_convert_sample_sheet(
-    parsed_bcl_convert_metrics: BclConvertMetricsParser,
-    bcl_convert_sample_sheet_model_with_data: BclConvertSampleSheetData,
-):
-    """Test to parse BCLConvert sample sheet."""
-    # GIVEN a parsed BCLConvert metrics
-
-    # ASSERT that the parsed sample sheet is correct
-    sample_sheet_model: BclConvertSampleSheetData = parsed_bcl_convert_metrics.sample_sheet[0]
-
-    # ASSERT that the parsed sample sheet is of the correct type
-    assert isinstance(sample_sheet_model, BclConvertSampleSheetData)
-
-    # ASSERT that the parsed sample sheet has the correct values
-    for attr_name, attr_value in sample_sheet_model.dict().items():
-        assert getattr(bcl_convert_sample_sheet_model_with_data, attr_name) == attr_value
-
-
 def test_get_sample_internal_ids(
     parsed_bcl_convert_metrics: BclConvertMetricsParser,
     test_sample_internal_id: str,
 ):
     """Test to get sample internal ids from BclConvertMetricsParser."""
     # GIVEN a parsed BCLConvert metrics
 
@@ -186,27 +167,14 @@
         sample_internal_id=test_sample_internal_id, lane=test_lane
     )
     expected_total_reads_per_lane: int = bcl_convert_reads_for_test_sample * 2
     # THEN assert that the total reads per lane is correct
     assert total_reads_per_lane == expected_total_reads_per_lane
 
 
-def test_get_flow_cell_name(
-    parsed_bcl_convert_metrics: BclConvertMetricsParser, bcl_convert_test_flow_cell_name: str
-):
-    """Test to get flow cell name from BclConvertMetricsParser."""
-    # GIVEN a parsed BCLConvert metrics
-
-    # WHEN getting flow cell name
-    flow_cell_name: str = parsed_bcl_convert_metrics.get_flow_cell_name()
-
-    # THEN assert that the flow cell name is correct
-    assert flow_cell_name == bcl_convert_test_flow_cell_name
-
-
 def test_get_q30_bases_percent_per_lane(
     parsed_bcl_convert_metrics,
     bcl_convert_test_q30_bases_percent: float,
     test_lane: int,
     test_sample_internal_id,
 ):
     """Test to get q30 bases percent per lane from BclConvertMetricsParser."""
@@ -237,25 +205,7 @@
         parsed_bcl_convert_metrics.get_mean_quality_score_for_sample_in_lane(
             sample_internal_id=test_sample_internal_id, lane=test_lane
         )
     )
 
     # THEN assert that the mean quality score per lane is correct
     assert mean_quality_score_per_lane == bcl_convert_test_mean_quality_score_per_lane
-
-
-def test_is_valid_sample_project(
-    parsed_bcl_convert_metrics: BclConvertMetricsParser, test_sample_internal_id: str
-):
-    """Test to check if a sample project is valid."""
-    # GIVEN a sample project
-
-    # WHEN checking if the sample project is valid
-    sample_project_list: List[str] = [test_sample_internal_id, INDEX_CHECK, UNDETERMINED]
-    expected_outcome: List[bool] = [True, False, False]
-
-    # THEN assert that the outcome is correct
-    for index in range(len(sample_project_list)):
-        assert (
-            parsed_bcl_convert_metrics.is_valid_sample(sample_project_list[index])
-            == expected_outcome[index]
-        )
```

### Comparing `cg-38.2.7/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py` & `cg-38.2.8/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/slurm/conftest.py` & `cg-38.2.8/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/slurm/test_slurm_api.py` & `cg-38.2.8/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/test_apps_environ.py` & `cg-38.2.8/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/apps/test_osticket.py` & `cg-38.2.8/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/add/test_cli_add.py` & `cg-38.2.8/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/add/test_cli_add_customer.py` & `cg-38.2.8/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/add/test_cli_add_family.py` & `cg-38.2.8/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/add/test_cli_add_relationship.py` & `cg-38.2.8/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/add/test_cli_add_sample.py` & `cg-38.2.8/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/backup/conftest.py` & `cg-38.2.8/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/backup/test_backup_command.py` & `cg-38.2.8/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/clean/conftest.py` & `cg-38.2.8/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/clean/test_balsamic_clean.py` & `cg-38.2.8/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-38.2.8/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/clean/test_hk_bundle_files.py` & `cg-38.2.8/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-38.2.8/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/clean/test_microbial_clean.py` & `cg-38.2.8/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-38.2.8/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/compress/conftest.py` & `cg-38.2.8/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/compress/test_cli_compress_fastq.py` & `cg-38.2.8/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/compress/test_cli_decompress_spring.py` & `cg-38.2.8/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/compress/test_compress_helpers.py` & `cg-38.2.8/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/compress/test_store_fastq.py` & `cg-38.2.8/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/conftest.py` & `cg-38.2.8/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/delete/test_cli_delete_case.py` & `cg-38.2.8/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/delete/test_cli_delete_cases.py` & `cg-38.2.8/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/deliver/conftest.py` & `cg-38.2.8/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/deliver/test_deliver_base.py` & `cg-38.2.8/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/deliver/test_rsync_base.py` & `cg-38.2.8/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-38.2.8/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/demultiplex/test_add_flowcell.py` & `cg-38.2.8/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-38.2.8/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,17 @@
         FLOW_CELL_FUNCTION_NAME,
         return_value=lims_novaseq_bcl2fastq_samples,
     )
     # GIVEN a lims api that returns some samples
 
     # WHEN creating a sample sheet
     result = cli_runner.invoke(
-        create_sheet, [str(flow_cell_working_directory)], obj=sample_sheet_context
+        create_sheet,
+        [str(flow_cell_working_directory)],
+        obj=sample_sheet_context,
     )
 
     # THEN the process finishes successfully
     assert result.exit_code == EXIT_SUCCESS
 
     # THEN the sample sheet was created
     assert flowcell.sample_sheet_exists()
```

### Comparing `cg-38.2.7/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-38.2.8/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/demultiplex/test_finish_demux.py` & `cg-38.2.8/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/demultiplex/test_stats_command.py` & `cg-38.2.8/tests/cli/demultiplex/test_stats_command.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-38.2.8/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/generate/report/conftest.py` & `cg-38.2.8/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-38.2.8/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/generate/report/test_utils.py` & `cg-38.2.8/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/generate/test_cli_base.py` & `cg-38.2.8/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/get/test_cli_get.py` & `cg-38.2.8/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/get/test_cli_get_analysis.py` & `cg-38.2.8/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/get/test_cli_get_case.py` & `cg-38.2.8/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/get/test_cli_get_flow_cell.py` & `cg-38.2.8/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/get/test_cli_get_sample.py` & `cg-38.2.8/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/set/conftest.py` & `cg-38.2.8/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/set/test_cli_set_case.py` & `cg-38.2.8/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/set/test_cli_set_cases.py` & `cg-38.2.8/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/set/test_cli_set_flowcell.py` & `cg-38.2.8/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/set/test_cli_set_list_keys.py` & `cg-38.2.8/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/set/test_cli_set_sample.py` & `cg-38.2.8/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/set/test_cli_set_samples.py` & `cg-38.2.8/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/store/test_fastq.py` & `cg-38.2.8/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/test_base.py` & `cg-38.2.8/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/test_clean.py` & `cg-38.2.8/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/conftest.py` & `cg-38.2.8/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/test_cli_scout.py` & `cg-38.2.8/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/test_cli_upload.py` & `cg-38.2.8/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/test_cli_upload_auto.py` & `cg-38.2.8/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-38.2.8/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/test_cli_upload_fastq.py` & `cg-38.2.8/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/test_cli_upload_genotype.py` & `cg-38.2.8/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/test_cli_upload_gens.py` & `cg-38.2.8/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/test_cli_upload_nipt.py` & `cg-38.2.8/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-38.2.8/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-38.2.8/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/upload/test_cli_upload_observations.py` & `cg-38.2.8/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/balsamic/conftest.py` & `cg-38.2.8/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-38.2.8/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-38.2.8/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/balsamic/test_link.py` & `cg-38.2.8/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-38.2.8/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/balsamic/test_run.py` & `cg-38.2.8/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-38.2.8/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/conftest.py` & `cg-38.2.8/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-38.2.8/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/fluffy/conftest.py` & `cg-38.2.8/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-38.2.8/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-38.2.8/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-38.2.8/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-38.2.8/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-38.2.8/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/microsalt/conftest.py` & `cg-38.2.8/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-38.2.8/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-38.2.8/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/mip/conftest.py` & `cg-38.2.8/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-38.2.8/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py` & `cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-38.2.8/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/taxprofiler/conftest.py` & `cg-38.2.8/tests/cli/workflow/taxprofiler/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py` & `cg-38.2.8/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py` & `cg-38.2.8/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/test_cli_workflow.py` & `cg-38.2.8/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-38.2.8/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/conftest.py` & `cg-38.2.8/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -772,24 +772,24 @@
 
 
 @pytest.fixture(name="flow_cell_runs_working_directory_bcl2fastq")
 def fixture_flow_cell_runs_working_directory_bcl2fastq(
     flow_cell_runs_working_directory: Path,
 ) -> Path:
     """Return the path to a working directory with flow cells ready for demux."""
-    working_dir: Path = Path(flow_cell_runs_working_directory, "bcl2fastq")
-    working_dir.mkdir(parents=True)
+    working_dir: Path = Path(flow_cell_runs_working_directory)
+    # working_dir.mkdir(parents=True)
     return working_dir
 
 
 @pytest.fixture(name="flow_cell_runs_working_directory_dragen")
 def fixture_flow_cell_runs_working_directory_dragen(flow_cell_runs_working_directory: Path) -> Path:
     """Return the path to a working directory with flow cells ready for demux."""
-    working_dir: Path = Path(flow_cell_runs_working_directory, "dragen")
-    working_dir.mkdir(parents=True)
+    working_dir: Path = Path(flow_cell_runs_working_directory)
+    # working_dir.mkdir(parents=True)
     return working_dir
 
 
 @pytest.fixture(name="demultiplexed_flow_cells_working_directory")
 def fixture_demultiplexed_flow_cells_working_directory(project_dir: Path) -> Path:
     """Return the path to a working directory with flow cells that have been demultiplexed."""
     working_dir: Path = Path(project_dir, "demultiplexed-runs")
@@ -833,14 +833,15 @@
 ) -> Path:
     """Return the path to a working directory that will be deleted after test is run.
 
     This is a path to a flow cell directory with the run parameters present.
     """
     working_dir: Path = Path(flow_cell_runs_working_directory, bcl2fastq_flow_cell_dir.name)
     working_dir.mkdir(parents=True)
+
     existing_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
         flow_cell_path=bcl2fastq_flow_cell_dir
     )
     working_flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(flow_cell_path=working_dir)
     shutil.copy(
         existing_flow_cell.run_parameters_path.as_posix(),
         working_flow_cell.run_parameters_path.as_posix(),
@@ -986,55 +987,58 @@
 @pytest.fixture(name="sample_sheet_context")
 def fixture_sample_sheet_context(cg_context: CGConfig, lims_api: LimsAPI) -> CGConfig:
     """Return cg context with an added lims API."""
     cg_context.lims_api_ = lims_api
     return cg_context
 
 
-@pytest.fixture
-def bcl_convert_demultiplexed_flow_cell_sample_ids() -> List[str]:
+@pytest.fixture(name="bcl_convert_demultiplexed_flow_cell_sample_internal_ids", scope="session")
+def fixture_bcl_convert_demultiplexed_flow_cell_sample_internal_ids() -> List[str]:
     """
     Sample id:s present in sample sheet for dummy flow cell demultiplexed with BCL Convert in
     cg/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2.
     """
     return ["ACC11927A2", "ACC11927A5"]
 
 
-@pytest.fixture(name="bcl2fastq_demultiplexed_flow_cell_sample_ids", scope="session")
-def fixture_bcl2fastq_demultiplexed_flow_cell_sample_ids() -> List[str]:
+@pytest.fixture(name="bcl2fastq_demultiplexed_flow_cell_sample_internal_ids", scope="session")
+def fixture_bcl2fastq_demultiplexed_flow_cell_sample_internal_ids() -> List[str]:
     """
     Sample id:s present in sample sheet for dummy flow cell demultiplexed with BCL Convert in
     cg/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX.
     """
     return ["SVE2528A1"]
 
 
 @pytest.fixture(name="flow_cell_name_demultiplexed_with_bcl2fastq", scope="session")
 def fixture_flow_cell_name_demultiplexed_with_bcl2fastq() -> str:
+    """Return the name of a flow cell that has been demultiplexed with BCL2Fastq."""
     return "HHKVCALXX"
 
 
 @pytest.fixture(name="flow_cell_directory_name_demultiplexed_with_bcl2fastq", scope="session")
 def flow_cell_directory_name_demultiplexed_with_bcl2fastq(
     flow_cell_name_demultiplexed_with_bcl2fastq: str,
 ):
+    """Return the name of a flow cell directory that has been demultiplexed with BCL2Fastq."""
     return f"170407_ST-E00198_0209_B{flow_cell_name_demultiplexed_with_bcl2fastq}"
 
 
 @pytest.fixture
 def store_with_demultiplexed_samples(
     store: Store,
     helpers: StoreHelpers,
-    bcl_convert_demultiplexed_flow_cell_sample_ids: List[str],
-    bcl2fastq_demultiplexed_flow_cell_sample_ids: List[str],
+    bcl_convert_demultiplexed_flow_cell_sample_internal_ids: List[str],
+    bcl2fastq_demultiplexed_flow_cell_sample_internal_ids: List[str],
 ) -> Store:
-    for i, sample_id in enumerate(bcl_convert_demultiplexed_flow_cell_sample_ids):
+    """Return a store with samples that have been demultiplexed with BCL Convert and BCL2Fastq."""
+    for i, sample_id in enumerate(bcl_convert_demultiplexed_flow_cell_sample_internal_ids):
         helpers.add_sample(store, internal_id=sample_id, name=f"sample_bcl_convert_{i}")
 
-    for i, sample_id in enumerate(bcl2fastq_demultiplexed_flow_cell_sample_ids):
+    for i, sample_id in enumerate(bcl2fastq_demultiplexed_flow_cell_sample_internal_ids):
         helpers.add_sample(store, internal_id=sample_id, name=f"sample_bcl2fastq_{i}")
     return store
 
 
 @pytest.fixture(name="demultiplex_context")
 def fixture_demultiplex_context(
     demultiplexing_api: DemultiplexingAPI,
```

### Comparing `cg-38.2.7/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-38.2.8/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-38.2.8/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-38.2.8/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/analysis/sample_coverage.bed` & `cg-38.2.8/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/balsamic/case/config.json` & `cg-38.2.8/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-38.2.8/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-38.2.8/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-38.2.8/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/hiseq/180522_ST-E00198_0301_BHLCKNCCXY/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_6000/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunCompletionStatus.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunCompletionStatus.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunInfo.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/flow-cell-runs/nova_seq_x/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml` & `cg-38.2.8/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-38.2.8/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-38.2.8/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/madeline/madeline.xml` & `cg-38.2.8/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-38.2.8/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-38.2.8/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-38.2.8/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-38.2.8/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-38.2.8/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-38.2.8/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-38.2.8/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-38.2.8/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-38.2.8/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-38.2.8/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-38.2.8/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/scout/643594.config.yaml` & `cg-38.2.8/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/scout/case_export.json` & `cg-38.2.8/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/scout/export_causatives.json` & `cg-38.2.8/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/scout/none_case_export.json` & `cg-38.2.8/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/scout/other_sex_case.json` & `cg-38.2.8/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/scout/panel_export.bed` & `cg-38.2.8/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/scout/panel_export.csv` & `cg-38.2.8/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Adapter_Metrics.csv` & `cg-38.2.8/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-38.2.8/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/apps/sequencing_metrics_parser/Unaligned/Reports/Quality_Metrics.csv` & `cg-38.2.8/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/cgweb_orders/balsamic.json` & `cg-38.2.8/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/cgweb_orders/fastq.json` & `cg-38.2.8/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/cgweb_orders/metagenome.json` & `cg-38.2.8/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/cgweb_orders/microsalt.json` & `cg-38.2.8/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/cgweb_orders/mip.json` & `cg-38.2.8/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-38.2.8/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/cgweb_orders/rml.json` & `cg-38.2.8/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/cgweb_orders/rnafusion.json` & `cg-38.2.8/tests/fixtures/cgweb_orders/rnafusion.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-38.2.8/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/data/SampleSheet.csv` & `cg-38.2.8/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/data/cgfixture.db` & `cg-38.2.8/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/data/hkstore.db` & `cg-38.2.8/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/io/example_json.json` & `cg-38.2.8/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/1508.28.balsamic.xlsx` & `cg-38.2.8/tests/fixtures/orderforms/1508.28.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/1508.28.balsamic_qc.xlsx` & `cg-38.2.8/tests/fixtures/orderforms/1508.28.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/1508.28.balsamic_umi.xlsx` & `cg-38.2.8/tests/fixtures/orderforms/1508.28.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/1508.28.fastq.xlsx` & `cg-38.2.8/tests/fixtures/orderforms/1508.28.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/1508.28.mip.xlsx` & `cg-38.2.8/tests/fixtures/orderforms/1508.28.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/1508.28.mip_rna.xlsx` & `cg-38.2.8/tests/fixtures/orderforms/1508.28.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/1508.28.rnafusion.xlsx` & `cg-38.2.8/tests/fixtures/orderforms/1508.28.rnafusion.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-38.2.8/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/1604.17.rml.xlsx` & `cg-38.2.8/tests/fixtures/orderforms/1604.17.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/1605.11.metagenome.xlsx` & `cg-38.2.8/tests/fixtures/orderforms/1605.11.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-38.2.8/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/NIPT-json.json` & `cg-38.2.8/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-38.2.8/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-38.2.8/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/report/case_data.json` & `cg-38.2.8/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/report/lims_exported_samples.json` & `cg-38.2.8/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/fixtures/report/lims_family.json` & `cg-38.2.8/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/io/conftest.py` & `cg-38.2.8/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/io/test_io_controller.py` & `cg-38.2.8/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/io/test_io_csv.py` & `cg-38.2.8/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/io/test_io_json.py` & `cg-38.2.8/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/io/test_io_xml.py` & `cg-38.2.8/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/io/test_io_yaml.py` & `cg-38.2.8/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/io/test_validate_path.py` & `cg-38.2.8/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/archive/conftest.py` & `cg-38.2.8/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/archive/test_archiving.py` & `cg-38.2.8/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/backup/conftest.py` & `cg-38.2.8/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/backup/test_meta_backup.py` & `cg-38.2.8/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/backup/test_meta_pdc.py` & `cg-38.2.8/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/clean/conftest.py` & `cg-38.2.8/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-38.2.8/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-38.2.8/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/clean/test_remove_old_dirs.py` & `cg-38.2.8/tests/meta/clean/test_remove_old_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/compress/conftest.py` & `cg-38.2.8/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/compress/test_clean_fastq.py` & `cg-38.2.8/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/compress/test_compress_files.py` & `cg-38.2.8/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/compress/test_compress_meta_fastq.py` & `cg-38.2.8/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/compress/test_decompress_spring_meta.py` & `cg-38.2.8/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-38.2.8/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/conftest.py` & `cg-38.2.8/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/deliver/conftest.py` & `cg-38.2.8/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/deliver/test_deliver_ticket.py` & `cg-38.2.8/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/deliver/test_delivery_api.py` & `cg-38.2.8/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/demultiplex/conftest.py` & `cg-38.2.8/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-38.2.8/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-38.2.8/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import logging
 from pathlib import Path
 from typing import Generator, List
-from mock import MagicMock, call
+from mock import MagicMock, call, patch
 
+import cg.apps.demultiplex.sample_sheet.models
 from cg.constants.demultiplexing import BclConverter, DemultiplexingDirsAndFiles
 from cg.constants.housekeeper_tags import SequencingFileTag
 from cg.meta.demultiplex.demux_post_processing import (
     DemuxPostProcessingAPI,
     DemuxPostProcessingHiseqXAPI,
 )
 from cg.meta.transfer import TransferFlowCell
 from cg.models.cg_config import CGConfig
 from cg.models.demultiplex.demux_results import DemuxResults
 from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 from cg.store import Store
 from cg.store.models import SampleLaneSequencingMetrics
+from cg.apps.demultiplex.sample_sheet.read_sample_sheet import (
+    get_sample_internal_ids_from_sample_sheet,
+)
 
 
 def test_set_dry_run(
     demultiplex_context: CGConfig,
 ):
     # GIVEN a demultiplex context
 
@@ -599,14 +603,30 @@
     # Assert that the expected methods were called with the expected arguments
     demux_post_processing_api.hk_api.get_tag.assert_has_calls(
         [call(name="tag1"), call(name="tag2")]
     )
     demux_post_processing_api.hk_api.add_tag.assert_not_called()
 
 
+def test_add_fastq_files_without_sample_id(
+    demultiplex_context: CGConfig, dragen_flow_cell: FlowCellDirectoryData
+):
+    # GIVEN a DemuxPostProcessing API
+    demux_post_processing_api = DemuxPostProcessingAPI(demultiplex_context)
+
+    demux_post_processing_api.add_file_to_bundle_if_non_existent = MagicMock()
+
+    # WHEN add_fastq_files is called
+
+    demux_post_processing_api.add_sample_fastq_files_to_housekeeper(flow_cell=dragen_flow_cell)
+
+    # THEN add_file_if_non_existent was not called
+    demux_post_processing_api.add_file_to_bundle_if_non_existent.assert_not_called()
+
+
 def test_add_existing_sample_sheet(demultiplex_context: CGConfig, tmpdir_factory):
     # GIVEN a DemuxPostProcessing API
     demux_post_processing_api = DemuxPostProcessingAPI(demultiplex_context)
     demux_post_processing_api.add_file_to_bundle_if_non_existent = MagicMock()
 
     # GIVEN a flow cell directory and name
     flow_cell_directory: Path = Path(tmpdir_factory.mktemp("flow_cell_directory"))
@@ -628,30 +648,14 @@
     demux_post_processing_api.add_file_to_bundle_if_non_existent.assert_called_once_with(
         file_path=expected_file_path,
         bundle_name=flow_cell_name,
         tag_names=expected_tag_names,
     )
 
 
-def test_add_fastq_files_without_sample_id(demultiplex_context: CGConfig):
-    # GIVEN a DemuxPostProcessing API
-    demux_post_processing_api = DemuxPostProcessingAPI(demultiplex_context)
-
-    get_sample_id_from_sample_fastq_path = MagicMock()
-    get_sample_id_from_sample_fastq_path.return_value = None
-
-    demux_post_processing_api.add_file_to_bundle_if_non_existent = MagicMock()
-
-    # WHEN add_fastq_files is called
-    demux_post_processing_api.add_sample_fastq_files_to_housekeeper(MagicMock())
-
-    # THEN add_file_if_non_existent was not called
-    demux_post_processing_api.add_file_to_bundle_if_non_existent.assert_not_called()
-
-
 def test_add_single_sequencing_metrics_entry_to_statusdb(
     store_with_sequencing_metrics: Store,
     demultiplex_context: CGConfig,
     flow_cell_name: str,
     sample_id: str,
     lane: int = 1,
 ):
@@ -709,15 +713,15 @@
 
 
 def test_post_processing_of_flow_cell_demultiplexed_with_bclconvert(
     demultiplex_context: CGConfig,
     flow_cell_directory_name_demultiplexed_with_bcl_convert: str,
     flow_cell_name_demultiplexed_with_bcl_convert: str,
     demultiplexed_flow_cells_directory: Path,
-    bcl_convert_demultiplexed_flow_cell_sample_ids: List[str],
+    bcl_convert_demultiplexed_flow_cell_sample_internal_ids,
 ):
     # GIVEN a DemuxPostProcessing API
     demux_post_processing_api = DemuxPostProcessingAPI(demultiplex_context)
 
     # GIVEN a directory with a flow cell demultiplexed with BCL Convert
     demux_post_processing_api.demux_api.out_dir = demultiplexed_flow_cells_directory
 
@@ -731,36 +735,35 @@
         flow_cell_name_demultiplexed_with_bcl_convert
     )
 
     # THEN sequencing metrics were created for the flow cell
     assert demux_post_processing_api.status_db.get_sample_lane_sequencing_metrics_by_flow_cell_name(
         flow_cell_name=flow_cell_name_demultiplexed_with_bcl_convert
     )
-
     # THEN the read count was calculated for all samples in the flow cell directory
-    for sample_id in bcl_convert_demultiplexed_flow_cell_sample_ids:
+    for sample_id in bcl_convert_demultiplexed_flow_cell_sample_internal_ids:
         sample = demux_post_processing_api.status_db.get_sample_by_internal_id(sample_id)
         assert sample is not None
         assert sample.calculated_read_count
 
     # THEN a bundle was added to Housekeeper for the flow cell
     assert demux_post_processing_api.hk_api.bundle(flow_cell_name_demultiplexed_with_bcl_convert)
 
     # THEN a bundle was added to Housekeeper for each sample
-    for sample_id in bcl_convert_demultiplexed_flow_cell_sample_ids:
+    for sample_id in bcl_convert_demultiplexed_flow_cell_sample_internal_ids:
         assert demux_post_processing_api.hk_api.bundle(sample_id)
 
     # THEN a sample sheet was added to Housekeeper
     assert demux_post_processing_api.hk_api.get_files(
         tags=[SequencingFileTag.SAMPLE_SHEET],
         bundle=flow_cell_name_demultiplexed_with_bcl_convert,
     ).all()
 
     # THEN sample fastq files were added to Housekeeper tagged with FASTQ and the flow cell name
-    for sample_id in bcl_convert_demultiplexed_flow_cell_sample_ids:
+    for sample_id in bcl_convert_demultiplexed_flow_cell_sample_internal_ids:
         assert demux_post_processing_api.hk_api.get_files(
             tags=[SequencingFileTag.FASTQ, flow_cell_name_demultiplexed_with_bcl_convert],
             bundle=sample_id,
         ).all()
 
     # THEN a delivery file was created in the flow cell directory
     delivery_path = Path(
@@ -773,15 +776,15 @@
 
 
 def test_post_processing_of_flow_cell_demultiplexed_with_bcl2fastq(
     demultiplex_context: CGConfig,
     flow_cell_directory_name_demultiplexed_with_bcl2fastq: str,
     flow_cell_name_demultiplexed_with_bcl2fastq: str,
     demultiplexed_flow_cells_directory: Path,
-    bcl2fastq_demultiplexed_flow_cell_sample_ids: List[str],
+    bcl2fastq_demultiplexed_flow_cell_sample_internal_ids: List[str],
 ):
     # GIVEN a DemuxPostProcessing API
     demux_post_processing_api = DemuxPostProcessingAPI(demultiplex_context)
 
     # GIVEN a directory with a flow cell demultiplexed with bcl2fastq
     demux_post_processing_api.demux_api.out_dir = demultiplexed_flow_cells_directory
 
@@ -797,37 +800,37 @@
 
     # THEN sequencing metrics were created for the flow cell
     assert demux_post_processing_api.status_db.get_sample_lane_sequencing_metrics_by_flow_cell_name(
         flow_cell_name=flow_cell_name_demultiplexed_with_bcl2fastq
     )
 
     # THEN the read count was calculated for all samples in the flow cell directory
-    for sample_id in bcl2fastq_demultiplexed_flow_cell_sample_ids:
-        sample = demux_post_processing_api.status_db.get_sample_by_internal_id(sample_id)
+    for sample_internal_id in bcl2fastq_demultiplexed_flow_cell_sample_internal_ids:
+        sample = demux_post_processing_api.status_db.get_sample_by_internal_id(sample_internal_id)
         assert sample is not None
         assert sample.calculated_read_count
 
     # THEN a bundle was added to Housekeeper for the flow cell
     assert demux_post_processing_api.hk_api.bundle(flow_cell_name_demultiplexed_with_bcl2fastq)
 
     # THEN a bundle was added to Housekeeper for each sample
-    for sample_id in bcl2fastq_demultiplexed_flow_cell_sample_ids:
-        assert demux_post_processing_api.hk_api.bundle(sample_id)
+    for sample_internal_id in bcl2fastq_demultiplexed_flow_cell_sample_internal_ids:
+        assert demux_post_processing_api.hk_api.bundle(sample_internal_id)
 
     # THEN a sample sheet was added to Housekeeper
     assert demux_post_processing_api.hk_api.get_files(
         tags=[SequencingFileTag.SAMPLE_SHEET],
         bundle=flow_cell_name_demultiplexed_with_bcl2fastq,
     ).all()
 
     # THEN sample fastq files were added to Housekeeper tagged with FASTQ and the flow cell name
-    for sample_id in bcl2fastq_demultiplexed_flow_cell_sample_ids:
+    for sample_internal_id in bcl2fastq_demultiplexed_flow_cell_sample_internal_ids:
         assert demux_post_processing_api.hk_api.get_files(
             tags=[SequencingFileTag.FASTQ, flow_cell_name_demultiplexed_with_bcl2fastq],
-            bundle=sample_id,
+            bundle=sample_internal_id,
         ).all()
 
     # THEN a delivery file was created in the flow cell directory
     delivery_path = Path(
         demux_post_processing_api.demux_api.out_dir,
         flow_cell_directory_name_demultiplexed_with_bcl2fastq,
         DemultiplexingDirsAndFiles.DELIVERY,
```

### Comparing `cg-38.2.7/tests/meta/demultiplex/test_rename_files.py` & `cg-38.2.8/tests/meta/demultiplex/test_rename_files.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/demultiplex/test_utils.py` & `cg-38.2.8/tests/meta/demultiplex/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from cg.constants.sequencing import FLOWCELL_Q30_THRESHOLD, Sequencers
 from cg.exc import FlowCellError
 from cg.meta.demultiplex.utils import (
     create_delivery_file_in_flow_cell_directory,
     get_bcl_converter_name,
     get_lane_from_sample_fastq,
     get_q30_threshold,
-    get_sample_internal_ids_from_flow_cell,
     get_sample_sheet_path,
     parse_flow_cell_directory_data,
 )
 from cg.meta.demultiplex.validation import is_bcl2fastq_demux_folder_structure
 from cg.models.demultiplex.flow_cell import FlowCellDirectoryData
 
 
@@ -161,37 +160,14 @@
 
     # WHEN the sample sheet is retrieved
     # THEN a FileNotFoundError should be raised
     with pytest.raises(FileNotFoundError):
         get_sample_sheet_path(flow_cell_directory)
 
 
-def test_get_sample_ids_from_sample_sheet():
-    # GIVEN some flow cell samples
-    mock_sample1 = MagicMock()
-    mock_sample1.sample_id = "sample1_index1"
-    mock_sample2 = MagicMock()
-    mock_sample2.sample_id = "sample2_index2"
-    mock_samples = [mock_sample1, mock_sample2]
-
-    # GIVEN a sample sheet with the samples
-    mock_sample_sheet = MagicMock()
-    type(mock_sample_sheet).samples = PropertyMock(return_value=mock_samples)
-
-    # GIVEN a flow cell data with the parsed sample sheet object
-    mock_flow_cell_data = MagicMock()
-    mock_flow_cell_data.get_sample_sheet.return_value = mock_sample_sheet
-
-    # WHEN extracting the sample ids from the sample sheet in the flow cell directory data
-    result = get_sample_internal_ids_from_flow_cell(mock_flow_cell_data)
-
-    # THEN the sample ids are returned without the index
-    assert result == ["sample1", "sample2"]
-
-
 @patch("cg.meta.demultiplex.utils.is_flow_cell_directory_valid", return_value=False)
 # GIVEN a flow cell directory which is not valid
 # WHEN parsing the flow cell directory data
 # THEN a FlowCellError should be raised
 def test_parse_flow_cell_directory_data_invalid(mocked_function):
     with pytest.raises(FlowCellError):
         parse_flow_cell_directory_data(Path("dummy_path"), "dummy_bcl_converter")
```

### Comparing `cg-38.2.7/tests/meta/demultiplex/test_validation.py` & `cg-38.2.8/tests/meta/demultiplex/test_validation.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/encryption/conftest.py` & `cg-38.2.8/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/encryption/test_encryption.py` & `cg-38.2.8/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/observations/conftest.py` & `cg-38.2.8/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/observations/test_meta_upload_observations.py` & `cg-38.2.8/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/orders/conftest.py` & `cg-38.2.8/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-38.2.8/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-38.2.8/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-38.2.8/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-38.2.8/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/orders/test_meta_orders_api.py` & `cg-38.2.8/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/orders/test_meta_orders_lims.py` & `cg-38.2.8/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/orders/test_meta_orders_status.py` & `cg-38.2.8/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/orders/test_rnafusion_submitter.py` & `cg-38.2.8/tests/meta/orders/test_rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/orders/test_ticket_handler.py` & `cg-38.2.8/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/report/conftest.py` & `cg-38.2.8/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/report/test_balsamic_api.py` & `cg-38.2.8/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/report/test_field_validators.py` & `cg-38.2.8/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/report/test_mip_dna_api.py` & `cg-38.2.8/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/report/test_report_api.py` & `cg-38.2.8/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/report/test_rnafusion_api.py` & `cg-38.2.8/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/rsync/conftest.py` & `cg-38.2.8/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/rsync/test_rsync.py` & `cg-38.2.8/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/test_invoice.py` & `cg-38.2.8/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/transfer/conftest.py` & `cg-38.2.8/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/transfer/test_external_data.py` & `cg-38.2.8/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-38.2.8/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-38.2.8/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/balsamic/test_balsamic.py` & `cg-38.2.8/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/conftest.py` & `cg-38.2.8/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-38.2.8/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/mutacc/conftest.py` & `cg-38.2.8/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-38.2.8/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/nipt/conftest.py` & `cg-38.2.8/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-38.2.8/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/scout/conftest.py` & `cg-38.2.8/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/scout/test_generate_load_config.py` & `cg-38.2.8/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-38.2.8/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-38.2.8/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-38.2.8/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/test_meta_upload_coverage.py` & `cg-38.2.8/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/test_upload_api.py` & `cg-38.2.8/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/upload/test_upload_genotypes_api.py` & `cg-38.2.8/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/workflow/conftest.py` & `cg-38.2.8/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/workflow/test_analysis.py` & `cg-38.2.8/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/workflow/test_balsamic.py` & `cg-38.2.8/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/workflow/test_microsalt.py` & `cg-38.2.8/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-38.2.8/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/meta/workflow/test_rnafusion.py` & `cg-38.2.8/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/balsamic_analysis_mock.py` & `cg-38.2.8/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/crunchy.py` & `cg-38.2.8/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/hk_mock.py` & `cg-38.2.8/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/limsmock.py` & `cg-38.2.8/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/madeline.py` & `cg-38.2.8/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/mip_analysis_mock.py` & `cg-38.2.8/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/osticket.py` & `cg-38.2.8/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/process_mock.py` & `cg-38.2.8/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/report.py` & `cg-38.2.8/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/scout.py` & `cg-38.2.8/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/store_model.py` & `cg-38.2.8/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/mocks/tb_mock.py` & `cg-38.2.8/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/balsamic/conftest.py` & `cg-38.2.8/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/balsamic/test_balsamic_analysis.py` & `cg-38.2.8/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/conftest.py` & `cg-38.2.8/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/demultiplexing/conftest.py` & `cg-38.2.8/tests/models/demultiplexing/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/demultiplexing/test_demux_results.py` & `cg-38.2.8/tests/models/demultiplexing/test_demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/demultiplexing/test_flowcell_model.py` & `cg-38.2.8/tests/models/demultiplexing/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/demultiplexing/test_run_parameters.py` & `cg-38.2.8/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/mip/conftest.py` & `cg-38.2.8/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/mip/test_mip_analysis.py` & `cg-38.2.8/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/mip/test_mip_config.py` & `cg-38.2.8/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-38.2.8/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/mip/test_mip_sample_info.py` & `cg-38.2.8/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/nextflow/conftest.py` & `cg-38.2.8/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/nextflow/test_nextflow_deliver.py` & `cg-38.2.8/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/observations/conftest.py` & `cg-38.2.8/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/observations/test_observations_input_files.py` & `cg-38.2.8/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/report/test_validators.py` & `cg-38.2.8/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/rnafusion/conftest.py` & `cg-38.2.8/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-38.2.8/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/test_cg_models.py` & `cg-38.2.8/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/test_compression_data.py` & `cg-38.2.8/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/test_file_data.py` & `cg-38.2.8/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/models/test_flowcell_class.py` & `cg-38.2.8/tests/models/test_flowcell_class.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/server/conftest.py` & `cg-38.2.8/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/add/test_store_add_application_version.py` & `cg-38.2.8/tests/store/api/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/add/test_store_add_base.py` & `cg-38.2.8/tests/store/api/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/add/test_store_add_customer.py` & `cg-38.2.8/tests/store/api/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/add/test_store_add_flow_celll.py` & `cg-38.2.8/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/conftest.py` & `cg-38.2.8/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/delete/test_store_api_delete.py` & `cg-38.2.8/tests/store/api/delete/test_store_api_delete.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/find/test_find_basic_data.py` & `cg-38.2.8/tests/store/api/find/test_find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-38.2.8/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/find/test_find_business_data.py` & `cg-38.2.8/tests/store/api/find/test_find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/find/test_find_business_data_analysis.py` & `cg-38.2.8/tests/store/api/find/test_find_business_data_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/find/test_find_business_data_case.py` & `cg-38.2.8/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/find/test_find_business_data_sample.py` & `cg-38.2.8/tests/store/api/find/test_find_business_data_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/status/test_analyses_to_clean.py` & `cg-38.2.8/tests/store/api/status/test_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-38.2.8/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/status/test_store_api_status.py` & `cg-38.2.8/tests/store/api/status/test_store_api_status.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/status/test_store_api_status_analysis.py` & `cg-38.2.8/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/status/test_store_api_status_cases.py` & `cg-38.2.8/tests/store/api/status/test_store_api_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/status/test_store_api_status_customer.py` & `cg-38.2.8/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/status/test_store_api_status_pool.py` & `cg-38.2.8/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/status/test_store_api_status_sample.py` & `cg-38.2.8/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/api/test_base.py` & `cg-38.2.8/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/conftest.py` & `cg-38.2.8/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_analyses_filters.py` & `cg-38.2.8/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_application_filters.py` & `cg-38.2.8/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_application_version_filters.py` & `cg-38.2.8/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_bed_filters.py` & `cg-38.2.8/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_bed_version_filters.py` & `cg-38.2.8/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_case_sample_filters.py` & `cg-38.2.8/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_cases_filters.py` & `cg-38.2.8/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_collaboration_filters.py` & `cg-38.2.8/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_customer_filters.py` & `cg-38.2.8/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_flow_cell_filters.py` & `cg-38.2.8/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_invoice_filters.py` & `cg-38.2.8/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_metrics_filters.py` & `cg-38.2.8/tests/store/filters/test_status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_organism_filters.py` & `cg-38.2.8/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_panel_filters.py` & `cg-38.2.8/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_pool_filters.py` & `cg-38.2.8/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_samples_filters.py` & `cg-38.2.8/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/filters/test_status_user_filters.py` & `cg-38.2.8/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/test_delivery.py` & `cg-38.2.8/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store/test_store_models.py` & `cg-38.2.8/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/store_helpers.py` & `cg-38.2.8/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/test_store_helpers.py` & `cg-38.2.8/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/utils/conftest.py` & `cg-38.2.8/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/utils/test_commands.py` & `cg-38.2.8/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/utils/test_date.py` & `cg-38.2.8/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/utils/test_dict.py` & `cg-38.2.8/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/utils/test_dispatcher.py` & `cg-38.2.8/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-38.2.7/tests/utils/test_utils.py` & `cg-38.2.8/tests/utils/test_utils.py`

 * *Files identical despite different names*


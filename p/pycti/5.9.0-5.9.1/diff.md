# Comparing `tmp/pycti-5.9.0.tar.gz` & `tmp/pycti-5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-5.9.0.tar", last modified: Mon Jul 10 16:03:45 2023, max compression
+gzip compressed data, was "pycti-5.9.1.tar", last modified: Wed Jul 12 19:19:07 2023, max compression
```

## Comparing `pycti-5.9.0.tar` & `pycti-5.9.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.404688 pycti-5.9.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-07-10 16:03:33.000000 pycti-5.9.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-10 16:03:45.404688 pycti-5.9.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-10 16:03:33.000000 pycti-5.9.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.396688 pycti-5.9.0/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4457 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.396688 pycti-5.9.0/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28771 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.396688 pycti-5.9.0/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45760 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/connector/opencti_connector_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.404688 pycti-5.9.0/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13376 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25352 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24724 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24705 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14512 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14598 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14155 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10891 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23072 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17564 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14162 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23083 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15950 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22773 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23099 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21404 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23941 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23507 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10147 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18610 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18872 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.404688 pycti-5.9.0/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6827 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106041 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14515 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.396688 pycti-5.9.0/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-10 16:03:45.000000 pycti-5.9.0/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-10 16:03:45.000000 pycti-5.9.0/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-10 16:03:45.000000 pycti-5.9.0/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-07-10 16:03:45.000000 pycti-5.9.0/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-10 16:03:45.000000 pycti-5.9.0/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-07-10 16:03:33.000000 pycti-5.9.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-07-10 16:03:45.408688 pycti-5.9.0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:19:07.558012 pycti-5.9.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-07-12 19:18:53.000000 pycti-5.9.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-12 19:19:07.558012 pycti-5.9.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-12 19:18:53.000000 pycti-5.9.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:19:07.550011 pycti-5.9.1/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4457 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:19:07.550011 pycti-5.9.1/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28771 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:19:07.550011 pycti-5.9.1/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45760 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/connector/opencti_connector_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:19:07.558012 pycti-5.9.1/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14340 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25352 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24724 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24705 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15508 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15549 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15139 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11897 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23072 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18533 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15126 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23083 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15950 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22773 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23099 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21404 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23941 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23507 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10147 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18610 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18872 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:19:07.558012 pycti-5.9.1/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6827 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106225 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14515 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-07-12 19:18:53.000000 pycti-5.9.1/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:19:07.550011 pycti-5.9.1/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-12 19:19:07.000000 pycti-5.9.1/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-12 19:19:07.000000 pycti-5.9.1/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-12 19:19:07.000000 pycti-5.9.1/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-07-12 19:19:07.000000 pycti-5.9.1/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-12 19:19:07.000000 pycti-5.9.1/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-07-12 19:18:53.000000 pycti-5.9.1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-07-12 19:19:07.558012 pycti-5.9.1/setup.cfg
```

### Comparing `pycti-5.9.0/LICENSE` & `pycti-5.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/PKG-INFO` & `pycti-5.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.9.0
+Version: 5.9.1
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.9.0 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.9.1 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.9.0/README.md` & `pycti-5.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/__init__.py` & `pycti-5.9.1/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "5.9.0"
+__version__ = "5.9.1"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-5.9.0/pycti/api/opencti_api_client.py` & `pycti-5.9.1/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/api/opencti_api_connector.py` & `pycti-5.9.1/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/api/opencti_api_work.py` & `pycti-5.9.1/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/connector/opencti_connector.py` & `pycti-5.9.1/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/connector/opencti_connector_helper.py` & `pycti-5.9.1/pycti/connector/opencti_connector_helper.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_attack_pattern.py` & `pycti-5.9.1/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_campaign.py` & `pycti-5.9.1/pycti/entities/opencti_incident.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # coding: utf-8
 
+import datetime
 import json
 import uuid
 
 from stix2.canonicalization.Canonicalize import canonicalize
 
 from pycti.entities import LOGGER
 
 
-class Campaign:
+class Incident:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             standard_id
             entity_type
             parent_types
@@ -112,14 +113,17 @@
             modified
             name
             description
             aliases
             first_seen
             last_seen
             objective
+            incident_type
+            severity
+            source
             importFiles {
                 edges {
                     node {
                         id
                         name
                         size
                         metaData {
@@ -128,49 +132,51 @@
                         }
                     }
                 }
             }
         """
 
     @staticmethod
-    def generate_id(name):
+    def generate_id(name, created):
         name = name.lower().strip()
-        data = {"name": name}
+        if isinstance(created, datetime.datetime):
+            created = created.isoformat()
+        data = {"name": name, "created": created}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
-        return "campaign--" + id
+        return "incident--" + id
 
     """
-        List Campaign objects
+        List Incident objects
 
         :param filters: the filters to apply
         :param search: the search keyword
         :param first: return the first n rows from the after ID (or the beginning if not set)
         :param after: ID of the first row for pagination
-        :return List of Campaign objects
+        :return List of Incident objects
     """
 
     def list(self, **kwargs):
         filters = kwargs.get("filters", None)
         search = kwargs.get("search", None)
         first = kwargs.get("first", 500)
         after = kwargs.get("after", None)
         order_by = kwargs.get("orderBy", None)
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
-            first = 500
+            first = 100
 
-        LOGGER.info("Listing Campaigns with filters %s.", json.dumps(filters))
+        LOGGER.info("Listing Incidents with filters %s.", json.dumps(filters))
         query = (
             """
-            query Campaigns($filters: [CampaignsFiltering], $search: String, $first: Int, $after: ID, $orderBy: CampaignsOrdering, $orderMode: OrderingMode) {
-                campaigns(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
+            query Incidents($filters: [IncidentsFiltering], $search: String, $first: Int, $after: ID, $orderBy: IncidentsOrdering, $orderMode: OrderingMode) {
+                incidents(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
                     edges {
                         node {
                             """
             + (custom_attributes if custom_attributes is not None else self.properties)
             + """
                         }
                     }
@@ -192,64 +198,86 @@
                 "search": search,
                 "first": first,
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
-        return self.opencti.process_multiple(
-            result["data"]["campaigns"], with_pagination
-        )
+        if get_all:
+            final_data = []
+            data = self.opencti.process_multiple(result["data"]["incidents"])
+            final_data = final_data + data
+            while result["data"]["incidents"]["pageInfo"]["hasNextPage"]:
+                after = result["data"]["incidents"]["pageInfo"]["endCursor"]
+                LOGGER.info("Listing Incidents after " + after)
+                result = self.opencti.query(
+                    query,
+                    {
+                        "filters": filters,
+                        "search": search,
+                        "first": first,
+                        "after": after,
+                        "orderBy": order_by,
+                        "orderMode": order_mode,
+                    },
+                )
+                data = self.opencti.process_multiple(result["data"]["incidents"])
+                final_data = final_data + data
+            return final_data
+        else:
+            return self.opencti.process_multiple(
+                result["data"]["incidents"], with_pagination
+            )
 
     """
-        Read a Campaign object
+        Read a Incident object
 
-        :param id: the id of the Campaign
+        :param id: the id of the Incident
         :param filters: the filters to apply if no id provided
-        :return Campaign object
+        :return Incident object
     """
 
     def read(self, **kwargs):
         id = kwargs.get("id", None)
         filters = kwargs.get("filters", None)
         custom_attributes = kwargs.get("customAttributes", None)
         if id is not None:
-            LOGGER.info("Reading Campaign {%s}.", id)
+            LOGGER.info("Reading Incident {%s}.", id)
             query = (
                 """
-                query Campaign($id: String!) {
-                    campaign(id: $id) {
+                query Incident($id: String!) {
+                    incident(id: $id) {
                         """
                 + (
                     custom_attributes
                     if custom_attributes is not None
                     else self.properties
                 )
                 + """
                     }
                 }
              """
             )
             result = self.opencti.query(query, {"id": id})
-            return self.opencti.process_multiple_fields(result["data"]["campaign"])
+            return self.opencti.process_multiple_fields(result["data"]["incident"])
         elif filters is not None:
             result = self.list(filters=filters)
             if len(result) > 0:
                 return result[0]
             else:
                 return None
         else:
-            LOGGER.error("[opencti_campaign] Missing parameters: id or filters")
+            LOGGER.error("[opencti_incident] Missing parameters: id or filters")
             return None
 
     """
-        Create a Campaign object
+        Create a Incident object
 
-        :param name: the name of the Campaign
-        :return Campaign object
+        :param name: the name of the Incident
+        :return Incident object
     """
 
     def create(self, **kwargs):
         stix_id = kwargs.get("stix_id", None)
         created_by = kwargs.get("createdBy", None)
         object_marking = kwargs.get("objectMarking", None)
         object_label = kwargs.get("objectLabel", None)
@@ -261,65 +289,71 @@
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
         description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         first_seen = kwargs.get("first_seen", None)
         last_seen = kwargs.get("last_seen", None)
         objective = kwargs.get("objective", None)
-        granted_refs = kwargs.get("objectOrganization", None)
+        incident_type = kwargs.get("incident_type", None)
+        severity = kwargs.get("severity", None)
+        source = kwargs.get("source", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
+        granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if name is not None:
-            LOGGER.info("Creating Campaign {%s}.", name)
+            LOGGER.info("Creating Incident {%s}.", name)
             query = """
-                mutation CampaignAdd($input: CampaignAddInput!) {
-                    campaignAdd(input: $input) {
+                mutation IncidentAdd($input: IncidentAddInput!) {
+                    incidentAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
-                }
+               }
             """
             result = self.opencti.query(
                 query,
                 {
                     "input": {
                         "stix_id": stix_id,
                         "createdBy": created_by,
                         "objectMarking": object_marking,
-                        "objectOrganization": granted_refs,
                         "objectLabel": object_label,
+                        "objectOrganization": granted_refs,
                         "externalReferences": external_references,
                         "revoked": revoked,
                         "confidence": confidence,
                         "lang": lang,
                         "created": created,
                         "modified": modified,
                         "name": name,
                         "description": description,
                         "aliases": aliases,
                         "first_seen": first_seen,
                         "last_seen": last_seen,
+                        "incident_type": incident_type,
                         "objective": objective,
-                        "update": update,
+                        "severity": severity,
+                        "source": source,
                         "x_opencti_stix_ids": x_opencti_stix_ids,
+                        "update": update,
                     }
                 },
             )
-            return self.opencti.process_multiple_fields(result["data"]["campaignAdd"])
+            return self.opencti.process_multiple_fields(result["data"]["incidentAdd"])
         else:
-            LOGGER.error("[opencti_campaign] Missing parameters: name and description")
+            LOGGER.error("Missing parameters: name and description")
 
     """
-        Import a Campaign object from a STIX2 object
+        Import a Incident object from a STIX2 object
 
-        :param stixObject: the Stix-Object Campaign
-        :return Campaign object
+        :param stixObject: the Stix-Object Incident
+        :return Incident object
     """
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
         extras = kwargs.get("extras", {})
         update = kwargs.get("update", False)
         if stix_object is not None:
@@ -366,17 +400,22 @@
                 else None,
                 first_seen=stix_object["first_seen"]
                 if "first_seen" in stix_object
                 else None,
                 last_seen=stix_object["last_seen"]
                 if "last_seen" in stix_object
                 else None,
+                incident_type=stix_object["incident_type"]
+                if "incident_type" in stix_object
+                else None,
+                severity=stix_object["severity"] if "severity" in stix_object else None,
+                source=stix_object["source"] if "source" in stix_object else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_campaign] Missing parameters: stixObject")
+            LOGGER.error("[opencti_incident] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.0/pycti/entities/opencti_case_incident.py` & `pycti-5.9.1/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_case_rfi.py` & `pycti-5.9.1/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_case_rft.py` & `pycti-5.9.1/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_channel.py` & `pycti-5.9.1/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_course_of_action.py` & `pycti-5.9.1/pycti/entities/opencti_campaign.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import uuid
 
 from stix2.canonicalization.Canonicalize import canonicalize
 
 from pycti.entities import LOGGER
 
 
-class CourseOfAction:
+class Campaign:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             standard_id
             entity_type
             parent_types
@@ -108,16 +108,18 @@
             }
             revoked
             confidence
             created
             modified
             name
             description
-            x_opencti_aliases
-            x_mitre_id
+            aliases
+            first_seen
+            last_seen
+            objective
             importFiles {
                 edges {
                     node {
                         id
                         name
                         size
                         metaData {
@@ -126,52 +128,49 @@
                         }
                     }
                 }
             }
         """
 
     @staticmethod
-    def generate_id(name, x_mitre_id=None):
+    def generate_id(name):
         name = name.lower().strip()
-        if x_mitre_id is not None:
-            data = {"x_mitre_id": x_mitre_id}
-        else:
-            data = {"name": name}
+        data = {"name": name}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
-        return "course-of-action--" + id
+        return "campaign--" + id
 
     """
-        List Course-Of-Action objects
+        List Campaign objects
 
         :param filters: the filters to apply
         :param search: the search keyword
         :param first: return the first n rows from the after ID (or the beginning if not set)
         :param after: ID of the first row for pagination
-        :return List of Course-Of-Action objects
+        :return List of Campaign objects
     """
 
     def list(self, **kwargs):
         filters = kwargs.get("filters", None)
         search = kwargs.get("search", None)
         first = kwargs.get("first", 500)
         after = kwargs.get("after", None)
         order_by = kwargs.get("orderBy", None)
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
-            first = 500
+            first = 100
 
-        LOGGER.info("Listing Course-Of-Actions with filters %s.", json.dumps(filters))
+        LOGGER.info("Listing Campaigns with filters %s.", json.dumps(filters))
         query = (
             """
-            query CoursesOfAction($filters: [CoursesOfActionFiltering], $search: String, $first: Int, $after: ID, $orderBy: CoursesOfActionOrdering, $orderMode: OrderingMode) {
-                coursesOfAction(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
+            query Campaigns($filters: [CampaignsFiltering], $search: String, $first: Int, $after: ID, $orderBy: CampaignsOrdering, $orderMode: OrderingMode) {
+                campaigns(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
                     edges {
                         node {
                             """
             + (custom_attributes if custom_attributes is not None else self.properties)
             + """
                         }
                     }
@@ -193,66 +192,86 @@
                 "search": search,
                 "first": first,
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
-        return self.opencti.process_multiple(
-            result["data"]["coursesOfAction"], with_pagination
-        )
+        if get_all:
+            final_data = []
+            data = self.opencti.process_multiple(result["data"]["campaigns"])
+            final_data = final_data + data
+            while result["data"]["campaigns"]["pageInfo"]["hasNextPage"]:
+                after = result["data"]["campaigns"]["pageInfo"]["endCursor"]
+                LOGGER.info("Listing Campaigns after " + after)
+                result = self.opencti.query(
+                    query,
+                    {
+                        "filters": filters,
+                        "search": search,
+                        "first": first,
+                        "after": after,
+                        "orderBy": order_by,
+                        "orderMode": order_mode,
+                    },
+                )
+                data = self.opencti.process_multiple(result["data"]["campaigns"])
+                final_data = final_data + data
+            return final_data
+        else:
+            return self.opencti.process_multiple(
+                result["data"]["campaigns"], with_pagination
+            )
 
     """
-        Read a Course-Of-Action object
+        Read a Campaign object
 
-        :param id: the id of the Course-Of-Action
+        :param id: the id of the Campaign
         :param filters: the filters to apply if no id provided
-        :return Course-Of-Action object
+        :return Campaign object
     """
 
     def read(self, **kwargs):
         id = kwargs.get("id", None)
         filters = kwargs.get("filters", None)
         custom_attributes = kwargs.get("customAttributes", None)
         if id is not None:
-            LOGGER.info("Reading Course-Of-Action {%s}.", id)
+            LOGGER.info("Reading Campaign {%s}.", id)
             query = (
                 """
-                query CourseOfAction($id: String!) {
-                    courseOfAction(id: $id) {
+                query Campaign($id: String!) {
+                    campaign(id: $id) {
                         """
                 + (
                     custom_attributes
                     if custom_attributes is not None
                     else self.properties
                 )
                 + """
                     }
                 }
              """
             )
             result = self.opencti.query(query, {"id": id})
-            return self.opencti.process_multiple_fields(
-                result["data"]["courseOfAction"]
-            )
+            return self.opencti.process_multiple_fields(result["data"]["campaign"])
         elif filters is not None:
             result = self.list(filters=filters)
             if len(result) > 0:
                 return result[0]
             else:
                 return None
         else:
-            LOGGER.error("[opencti_course_of_action] Missing parameters: id or filters")
+            LOGGER.error("[opencti_campaign] Missing parameters: id or filters")
             return None
 
     """
-        Create a Course Of Action object
+        Create a Campaign object
 
-        :param name: the name of the Course Of Action
-        :return Course Of Action object
+        :param name: the name of the Campaign
+        :return Campaign object
     """
 
     def create(self, **kwargs):
         stix_id = kwargs.get("stix_id", None)
         created_by = kwargs.get("createdBy", None)
         object_marking = kwargs.get("objectMarking", None)
         object_label = kwargs.get("objectLabel", None)
@@ -260,102 +279,77 @@
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
         description = kwargs.get("description", None)
-        x_opencti_aliases = kwargs.get("x_opencti_aliases", None)
-        x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
-        x_mitre_id = kwargs.get("x_mitre_id", None)
+        aliases = kwargs.get("aliases", None)
+        first_seen = kwargs.get("first_seen", None)
+        last_seen = kwargs.get("last_seen", None)
+        objective = kwargs.get("objective", None)
         granted_refs = kwargs.get("objectOrganization", None)
+        x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         update = kwargs.get("update", False)
 
         if name is not None:
-            LOGGER.info("Creating Course Of Action {%s}.", name)
+            LOGGER.info("Creating Campaign {%s}.", name)
             query = """
-                mutation CourseOfActionAdd($input: CourseOfActionAddInput!) {
-                    courseOfActionAdd(input: $input) {
+                mutation CampaignAdd($input: CampaignAddInput!) {
+                    campaignAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
             """
             result = self.opencti.query(
                 query,
                 {
                     "input": {
                         "stix_id": stix_id,
                         "createdBy": created_by,
                         "objectMarking": object_marking,
-                        "objectLabel": object_label,
                         "objectOrganization": granted_refs,
+                        "objectLabel": object_label,
                         "externalReferences": external_references,
                         "revoked": revoked,
                         "confidence": confidence,
                         "lang": lang,
                         "created": created,
                         "modified": modified,
                         "name": name,
                         "description": description,
-                        "x_opencti_aliases": x_opencti_aliases,
-                        "x_opencti_stix_ids": x_opencti_stix_ids,
-                        "x_mitre_id": x_mitre_id,
+                        "aliases": aliases,
+                        "first_seen": first_seen,
+                        "last_seen": last_seen,
+                        "objective": objective,
                         "update": update,
+                        "x_opencti_stix_ids": x_opencti_stix_ids,
                     }
                 },
             )
-            return self.opencti.process_multiple_fields(
-                result["data"]["courseOfActionAdd"]
-            )
+            return self.opencti.process_multiple_fields(result["data"]["campaignAdd"])
         else:
-            LOGGER.error(
-                "[opencti_course_of_action] Missing parameters: name and description"
-            )
+            LOGGER.error("[opencti_campaign] Missing parameters: name and description")
 
     """
-        Import an Course-Of-Action object from a STIX2 object
+        Import a Campaign object from a STIX2 object
 
-        :param stixObject: the Stix-Object Course-Of-Action
-        :return Course-Of-Action object
+        :param stixObject: the Stix-Object Campaign
+        :return Campaign object
     """
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
         extras = kwargs.get("extras", {})
         update = kwargs.get("update", False)
         if stix_object is not None:
-            # Extract external ID
-            x_mitre_id = None
-            if "x_mitre_id" in stix_object:
-                x_mitre_id = stix_object["x_mitre_id"]
-            elif (
-                self.opencti.get_attribute_in_mitre_extension("id", stix_object)
-                is not None
-            ):
-                x_mitre_id = self.opencti.get_attribute_in_mitre_extension(
-                    "id", stix_object
-                )
-            elif "external_references" in stix_object:
-                for external_reference in stix_object["external_references"]:
-                    if (
-                        external_reference["source_name"] == "mitre-attack"
-                        or external_reference["source_name"] == "mitre-pre-attack"
-                        or external_reference["source_name"] == "mitre-mobile-attack"
-                        or external_reference["source_name"] == "amitt-attack"
-                    ):
-                        x_mitre_id = external_reference["external_id"]
-
             # Search in extensions
-            if "x_opencti_aliases" not in stix_object:
-                stix_object[
-                    "x_opencti_aliases"
-                ] = self.opencti.get_attribute_in_extension("aliases", stix_object)
             if "x_opencti_stix_ids" not in stix_object:
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
             if "granted_refs" not in stix_object:
                 stix_object["granted_refs"] = self.opencti.get_attribute_in_extension(
                     "granted_refs", stix_object
@@ -384,19 +378,27 @@
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
                 else None,
+                aliases=self.opencti.stix2.pick_aliases(stix_object),
+                objective=stix_object["objective"]
+                if "objective" in stix_object
+                else None,
+                first_seen=stix_object["first_seen"]
+                if "first_seen" in stix_object
+                else None,
+                last_seen=stix_object["last_seen"]
+                if "last_seen" in stix_object
+                else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                x_opencti_aliases=self.opencti.stix2.pick_aliases(stix_object),
-                x_mitre_id=x_mitre_id,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_course_of_action] Missing parameters: stixObject")
+            LOGGER.error("[opencti_campaign] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.0/pycti/entities/opencti_data_component.py` & `pycti-5.9.1/pycti/entities/opencti_data_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # coding: utf-8
 
 import json
 import uuid
 
 from stix2.canonicalization.Canonicalize import canonicalize
 
+from pycti.entities import LOGGER
+
 
 class DataComponent:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             standard_id
@@ -169,20 +171,17 @@
         after = kwargs.get("after", None)
         order_by = kwargs.get("orderBy", None)
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
-            first = 500
+            first = 100
 
-        self.opencti.log(
-            "info",
-            "Listing Data-Components with filters " + json.dumps(filters) + ".",
-        )
+        LOGGER.info("Listing Data-Components with filters " + json.dumps(filters) + ".")
         query = (
             """
             query DataComponents($filters: [DataComponentsFiltering!], $search: String, $first: Int, $after: ID, $orderBy: DataComponentsOrdering, $orderMode: OrderingMode) {
                 dataComponents(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
                     edges {
                         node {
                             """
@@ -208,18 +207,39 @@
                 "search": search,
                 "first": first,
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
-        # TODO: get_all ?
-        return self.opencti.process_multiple(
-            result["data"]["dataComponents"], with_pagination
-        )
+        if get_all:
+            final_data = []
+            data = self.opencti.process_multiple(result["data"]["dataComponents"])
+            final_data = final_data + data
+            while result["data"]["dataComponents"]["pageInfo"]["hasNextPage"]:
+                after = result["data"]["dataComponents"]["pageInfo"]["endCursor"]
+                LOGGER.info("Listing Data-Components after " + after)
+                result = self.opencti.query(
+                    query,
+                    {
+                        "filters": filters,
+                        "search": search,
+                        "first": first,
+                        "after": after,
+                        "orderBy": order_by,
+                        "orderMode": order_mode,
+                    },
+                )
+                data = self.opencti.process_multiple(result["data"]["dataComponents"])
+                final_data = final_data + data
+            return final_data
+        else:
+            return self.opencti.process_multiple(
+                result["data"]["dataComponents"], with_pagination
+            )
 
     """
         Read a Data-Component object
 
         :param id: the id of the Data-Component
         :param filters: the filters to apply if no id provided
         :return Data-Component object
```

### Comparing `pycti-5.9.0/pycti/entities/opencti_data_source.py` & `pycti-5.9.1/pycti/entities/opencti_data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # coding: utf-8
 
 import json
 import uuid
 
 from stix2.canonicalization.Canonicalize import canonicalize
 
+from pycti.entities import LOGGER
+
 
 class DataSource:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             standard_id
@@ -153,15 +155,15 @@
         after = kwargs.get("after", None)
         order_by = kwargs.get("orderBy", None)
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
-            first = 500
+            first = 100
 
         self.opencti.log(
             "info",
             "Listing Data-Sources with filters " + json.dumps(filters) + ".",
         )
         query = (
             """
@@ -192,18 +194,39 @@
                 "search": search,
                 "first": first,
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
-        # TODO: get_all ?
-        return self.opencti.process_multiple(
-            result["data"]["dataSources"], with_pagination
-        )
+        if get_all:
+            final_data = []
+            data = self.opencti.process_multiple(result["data"]["dataSources"])
+            final_data = final_data + data
+            while result["data"]["dataSources"]["pageInfo"]["hasNextPage"]:
+                after = result["data"]["dataSources"]["pageInfo"]["endCursor"]
+                LOGGER.info("Listing Data-Sources after " + after)
+                result = self.opencti.query(
+                    query,
+                    {
+                        "filters": filters,
+                        "search": search,
+                        "first": first,
+                        "after": after,
+                        "orderBy": order_by,
+                        "orderMode": order_mode,
+                    },
+                )
+                data = self.opencti.process_multiple(result["data"]["dataSources"])
+                final_data = final_data + data
+            return final_data
+        else:
+            return self.opencti.process_multiple(
+                result["data"]["dataSources"], with_pagination
+            )
 
     """
         Read a Data-Source object
 
         :param id: the id of the Data-Source
         :param filters: the filters to apply if no id provided
         :return Data-Source object
```

### Comparing `pycti-5.9.0/pycti/entities/opencti_event.py` & `pycti-5.9.1/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_external_reference.py` & `pycti-5.9.1/pycti/entities/opencti_external_reference.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         after = kwargs.get("after", None)
         order_by = kwargs.get("orderBy", None)
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
-            first = 500
+            first = 100
 
         LOGGER.info("Listing External-Reference with filters %s.", json.dumps(filters))
         query = (
             """
             query ExternalReferences($filters: [ExternalReferencesFiltering], $first: Int, $after: ID, $orderBy: ExternalReferencesOrdering, $orderMode: OrderingMode) {
                 externalReferences(filters: $filters, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
                     edges {
@@ -105,17 +105,40 @@
                 "filters": filters,
                 "first": first,
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
-        return self.opencti.process_multiple(
-            result["data"]["externalReferences"], with_pagination
-        )
+        if get_all:
+            final_data = []
+            data = self.opencti.process_multiple(result["data"]["externalReferences"])
+            final_data = final_data + data
+            while result["data"]["externalReferences"]["pageInfo"]["hasNextPage"]:
+                after = result["data"]["externalReferences"]["pageInfo"]["endCursor"]
+                LOGGER.info("Listing External-References after " + after)
+                result = self.opencti.query(
+                    query,
+                    {
+                        "filters": filters,
+                        "first": first,
+                        "after": after,
+                        "orderBy": order_by,
+                        "orderMode": order_mode,
+                    },
+                )
+                data = self.opencti.process_multiple(
+                    result["data"]["externalReferences"]
+                )
+                final_data = final_data + data
+            return final_data
+        else:
+            return self.opencti.process_multiple(
+                result["data"]["externalReferences"], with_pagination
+            )
 
     """
         Read a External-Reference object
 
         :param id: the id of the External-Reference
         :param filters: the filters to apply if no id provided
         :return External-Reference object
```

### Comparing `pycti-5.9.0/pycti/entities/opencti_feedback.py` & `pycti-5.9.1/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_grouping.py` & `pycti-5.9.1/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_identity.py` & `pycti-5.9.1/pycti/entities/opencti_identity.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,17 +203,39 @@
                 "search": search,
                 "first": first,
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
-        return self.opencti.process_multiple(
-            result["data"]["identities"], with_pagination
-        )
+        if get_all:
+            final_data = []
+            data = self.opencti.process_multiple(result["data"]["identities"])
+            final_data = final_data + data
+            while result["data"]["identities"]["pageInfo"]["hasNextPage"]:
+                after = result["data"]["identities"]["pageInfo"]["endCursor"]
+                LOGGER.info("Listing Identities after " + after)
+                result = self.opencti.query(
+                    query,
+                    {
+                        "filters": filters,
+                        "search": search,
+                        "first": first,
+                        "after": after,
+                        "orderBy": order_by,
+                        "orderMode": order_mode,
+                    },
+                )
+                data = self.opencti.process_multiple(result["data"]["identities"])
+                final_data = final_data + data
+            return final_data
+        else:
+            return self.opencti.process_multiple(
+                result["data"]["identities"], with_pagination
+            )
 
     """
         Read a Identity object
 
         :param id: the id of the Identity
         :param filters: the filters to apply if no id provided
         :return Identity object
```

### Comparing `pycti-5.9.0/pycti/entities/opencti_incident.py` & `pycti-5.9.1/pycti/entities/opencti_narrative.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding: utf-8
 
-import datetime
 import json
 import uuid
 
 from stix2.canonicalization.Canonicalize import canonicalize
 
 from pycti.entities import LOGGER
 
 
-class Incident:
+class Narrative:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             standard_id
             entity_type
             parent_types
@@ -110,20 +109,15 @@
             revoked
             confidence
             created
             modified
             name
             description
             aliases
-            first_seen
-            last_seen
-            objective
-            incident_type
-            severity
-            source
+            narrative_types
             importFiles {
                 edges {
                     node {
                         id
                         name
                         size
                         metaData {
@@ -132,51 +126,49 @@
                         }
                     }
                 }
             }
         """
 
     @staticmethod
-    def generate_id(name, created):
+    def generate_id(name):
         name = name.lower().strip()
-        if isinstance(created, datetime.datetime):
-            created = created.isoformat()
-        data = {"name": name, "created": created}
+        data = {"name": name}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
-        return "incident--" + id
+        return "narrative--" + id
 
     """
-        List Incident objects
+        List Narrative objects
 
         :param filters: the filters to apply
         :param search: the search keyword
         :param first: return the first n rows from the after ID (or the beginning if not set)
         :param after: ID of the first row for pagination
-        :return List of Incident objects
+        :return List of Narrative objects
     """
 
     def list(self, **kwargs):
         filters = kwargs.get("filters", None)
         search = kwargs.get("search", None)
-        first = kwargs.get("first", 500)
+        first = kwargs.get("first", 100)
         after = kwargs.get("after", None)
         order_by = kwargs.get("orderBy", None)
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
-            first = 500
+            first = 100
 
-        LOGGER.info("Listing Incidents with filters %s.", json.dumps(filters))
+        LOGGER.info("Listing Narratives with filters %s.", json.dumps(filters))
         query = (
             """
-            query Incidents($filters: [IncidentsFiltering], $search: String, $first: Int, $after: ID, $orderBy: IncidentsOrdering, $orderMode: OrderingMode) {
-                incidents(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
+            query Narratives($filters: [NarrativesFiltering!], $search: String, $first: Int, $after: ID, $orderBy: NarrativesOrdering, $orderMode: OrderingMode) {
+                narratives(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
                     edges {
                         node {
                             """
             + (custom_attributes if custom_attributes is not None else self.properties)
             + """
                         }
                     }
@@ -198,64 +190,86 @@
                 "search": search,
                 "first": first,
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
-        return self.opencti.process_multiple(
-            result["data"]["incidents"], with_pagination
-        )
+        if get_all:
+            final_data = []
+            data = self.opencti.process_multiple(result["data"]["narratives"])
+            final_data = final_data + data
+            while result["data"]["narratives"]["pageInfo"]["hasNextPage"]:
+                after = result["data"]["narratives"]["pageInfo"]["endCursor"]
+                LOGGER.info("Listing Narratives after " + after)
+                result = self.opencti.query(
+                    query,
+                    {
+                        "filters": filters,
+                        "search": search,
+                        "first": first,
+                        "after": after,
+                        "orderBy": order_by,
+                        "orderMode": order_mode,
+                    },
+                )
+                data = self.opencti.process_multiple(result["data"]["narratives"])
+                final_data = final_data + data
+            return final_data
+        else:
+            return self.opencti.process_multiple(
+                result["data"]["narratives"], with_pagination
+            )
 
     """
-        Read a Incident object
+        Read a Narrative object
 
-        :param id: the id of the Incident
+        :param id: the id of the Narrative
         :param filters: the filters to apply if no id provided
-        :return Incident object
+        :return Narrative object
     """
 
     def read(self, **kwargs):
         id = kwargs.get("id", None)
         filters = kwargs.get("filters", None)
         custom_attributes = kwargs.get("customAttributes", None)
         if id is not None:
-            LOGGER.info("Reading Incident {%s}.", id)
+            LOGGER.info("Reading Narrative {%s}.", id)
             query = (
                 """
-                query Incident($id: String!) {
-                    incident(id: $id) {
+                query Narrative($id: String!) {
+                    narrative(id: $id) {
                         """
                 + (
                     custom_attributes
                     if custom_attributes is not None
                     else self.properties
                 )
                 + """
                     }
                 }
              """
             )
             result = self.opencti.query(query, {"id": id})
-            return self.opencti.process_multiple_fields(result["data"]["incident"])
+            return self.opencti.process_multiple_fields(result["data"]["narrative"])
         elif filters is not None:
             result = self.list(filters=filters)
             if len(result) > 0:
                 return result[0]
             else:
                 return None
         else:
-            LOGGER.error("[opencti_incident] Missing parameters: id or filters")
+            LOGGER.error("[opencti_narrative] Missing parameters: id or filters")
             return None
 
     """
-        Create a Incident object
+        Create a Narrative object
 
-        :param name: the name of the Incident
-        :return Incident object
+        :param name: the name of the Narrative
+        :return Narrative object
     """
 
     def create(self, **kwargs):
         stix_id = kwargs.get("stix_id", None)
         created_by = kwargs.get("createdBy", None)
         object_marking = kwargs.get("objectMarking", None)
         object_label = kwargs.get("objectLabel", None)
@@ -264,35 +278,30 @@
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
         description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
-        first_seen = kwargs.get("first_seen", None)
-        last_seen = kwargs.get("last_seen", None)
-        objective = kwargs.get("objective", None)
-        incident_type = kwargs.get("incident_type", None)
-        severity = kwargs.get("severity", None)
-        source = kwargs.get("source", None)
+        narrative_types = kwargs.get("narrative_types", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if name is not None:
-            LOGGER.info("Creating Incident {%s}.", name)
+            LOGGER.info("Creating Narrative {%s}.", name)
             query = """
-                mutation IncidentAdd($input: IncidentAddInput!) {
-                    incidentAdd(input: $input) {
+                mutation NarrativeAdd($input: NarrativeAddInput!) {
+                    narrativeAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
-               }
+                }
             """
             result = self.opencti.query(
                 query,
                 {
                     "input": {
                         "stix_id": stix_id,
                         "createdBy": created_by,
@@ -304,34 +313,29 @@
                         "confidence": confidence,
                         "lang": lang,
                         "created": created,
                         "modified": modified,
                         "name": name,
                         "description": description,
                         "aliases": aliases,
-                        "first_seen": first_seen,
-                        "last_seen": last_seen,
-                        "incident_type": incident_type,
-                        "objective": objective,
-                        "severity": severity,
-                        "source": source,
+                        "narrative_types": narrative_types,
                         "x_opencti_stix_ids": x_opencti_stix_ids,
                         "update": update,
                     }
                 },
             )
-            return self.opencti.process_multiple_fields(result["data"]["incidentAdd"])
+            return self.opencti.process_multiple_fields(result["data"]["narrativeAdd"])
         else:
-            LOGGER.error("Missing parameters: name and description")
+            LOGGER.error("[opencti_narrative] Missing parameters: name and description")
 
     """
-        Import a Incident object from a STIX2 object
+        Import an Narrative object from a STIX2 object
 
-        :param stixObject: the Stix-Object Incident
-        :return Incident object
+        :param stixObject: the Stix-Object Narrative
+        :return Narrative object
     """
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
         extras = kwargs.get("extras", {})
         update = kwargs.get("update", False)
         if stix_object is not None:
@@ -341,15 +345,15 @@
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
             if "granted_refs" not in stix_object:
                 stix_object["granted_refs"] = self.opencti.get_attribute_in_extension(
                     "granted_refs", stix_object
                 )
 
-            return self.create(
+            return self.opencti.narrative.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
@@ -369,31 +373,20 @@
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
                 else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
-                objective=stix_object["objective"]
-                if "objective" in stix_object
-                else None,
-                first_seen=stix_object["first_seen"]
-                if "first_seen" in stix_object
-                else None,
-                last_seen=stix_object["last_seen"]
-                if "last_seen" in stix_object
-                else None,
-                incident_type=stix_object["incident_type"]
-                if "incident_type" in stix_object
+                narrative_types=stix_object["narrative_types"]
+                if "narrative_types" in stix_object
                 else None,
-                severity=stix_object["severity"] if "severity" in stix_object else None,
-                source=stix_object["source"] if "source" in stix_object else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_incident] Missing parameters: stixObject")
+            LOGGER.error("[opencti_narrative] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.0/pycti/entities/opencti_indicator.py` & `pycti-5.9.1/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_infrastructure.py` & `pycti-5.9.1/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_intrusion_set.py` & `pycti-5.9.1/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_kill_chain_phase.py` & `pycti-5.9.1/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_label.py` & `pycti-5.9.1/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_language.py` & `pycti-5.9.1/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_location.py` & `pycti-5.9.1/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_malware.py` & `pycti-5.9.1/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_malware_analysis.py` & `pycti-5.9.1/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_marking_definition.py` & `pycti-5.9.1/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_narrative.py` & `pycti-5.9.1/pycti/entities/opencti_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import uuid
 
 from stix2.canonicalization.Canonicalize import canonicalize
 
 from pycti.entities import LOGGER
 
 
-class Narrative:
+class Tool:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             standard_id
             entity_type
             parent_types
@@ -109,15 +109,30 @@
             revoked
             confidence
             created
             modified
             name
             description
             aliases
-            narrative_types
+            tool_types
+            tool_version
+            killChainPhases {
+                edges {
+                    node {
+                        id
+                        standard_id
+                        entity_type
+                        kill_chain_name
+                        phase_name
+                        x_opencti_order
+                        created
+                        modified
+                    }
+                }
+            }
             importFiles {
                 edges {
                     node {
                         id
                         name
                         size
                         metaData {
@@ -131,24 +146,24 @@
 
     @staticmethod
     def generate_id(name):
         name = name.lower().strip()
         data = {"name": name}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
-        return "narrative--" + id
+        return "tool--" + id
 
     """
-        List Narrative objects
+        List Tool objects
 
         :param filters: the filters to apply
         :param search: the search keyword
         :param first: return the first n rows from the after ID (or the beginning if not set)
         :param after: ID of the first row for pagination
-        :return List of Narrative objects
+        :return List of Tool objects
     """
 
     def list(self, **kwargs):
         filters = kwargs.get("filters", None)
         search = kwargs.get("search", None)
         first = kwargs.get("first", 100)
         after = kwargs.get("after", None)
@@ -156,19 +171,19 @@
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
             first = 100
 
-        LOGGER.info("Listing Narratives with filters %s.", json.dumps(filters))
+        LOGGER.info("Listing Tools with filters %s.", json.dumps(filters))
         query = (
             """
-            query Narratives($filters: [NarrativesFiltering!], $search: String, $first: Int, $after: ID, $orderBy: NarrativesOrdering, $orderMode: OrderingMode) {
-                narratives(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
+            query Tools($filters: [ToolsFiltering], $search: String, $first: Int, $after: ID, $orderBy: ToolsOrdering, $orderMode: OrderingMode) {
+                tools(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
                     edges {
                         node {
                             """
             + (custom_attributes if custom_attributes is not None else self.properties)
             + """
                         }
                     }
@@ -192,84 +207,84 @@
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
         if get_all:
             final_data = []
-            data = self.opencti.process_multiple(result["data"]["narratives"])
+            data = self.opencti.process_multiple(result["data"]["tools"])
             final_data = final_data + data
-            while result["data"]["narratives"]["pageInfo"]["hasNextPage"]:
-                after = result["data"]["narratives"]["pageInfo"]["endCursor"]
-                LOGGER.info("Listing Narratives after " + after)
+            while result["data"]["tools"]["pageInfo"]["hasNextPage"]:
+                after = result["data"]["tools"]["pageInfo"]["endCursor"]
+                LOGGER.info("Listing Tools after " + after)
                 result = self.opencti.query(
                     query,
                     {
                         "filters": filters,
                         "search": search,
                         "first": first,
                         "after": after,
                         "orderBy": order_by,
                         "orderMode": order_mode,
                     },
                 )
-                data = self.opencti.process_multiple(result["data"]["narratives"])
+                data = self.opencti.process_multiple(result["data"]["tools"])
                 final_data = final_data + data
             return final_data
         else:
             return self.opencti.process_multiple(
-                result["data"]["narratives"], with_pagination
+                result["data"]["tools"], with_pagination
             )
 
     """
-        Read a Narrative object
+        Read a Tool object
 
-        :param id: the id of the Narrative
+        :param id: the id of the Tool
         :param filters: the filters to apply if no id provided
-        :return Narrative object
+        :return Tool object
     """
 
     def read(self, **kwargs):
         id = kwargs.get("id", None)
         filters = kwargs.get("filters", None)
         custom_attributes = kwargs.get("customAttributes", None)
         if id is not None:
-            LOGGER.info("Reading Narrative {%s}.", id)
+            LOGGER.info("Reading Tool {%s}.", id)
             query = (
                 """
-                query Narrative($id: String!) {
-                    narrative(id: $id) {
+                query Tool($id: String!) {
+                    tool(id: $id) {
                         """
                 + (
                     custom_attributes
                     if custom_attributes is not None
                     else self.properties
                 )
                 + """
                     }
                 }
              """
             )
             result = self.opencti.query(query, {"id": id})
-            return self.opencti.process_multiple_fields(result["data"]["narrative"])
+            return self.opencti.process_multiple_fields(result["data"]["tool"])
         elif filters is not None:
             result = self.list(filters=filters)
             if len(result) > 0:
                 return result[0]
             else:
                 return None
         else:
-            LOGGER.error("[opencti_narrative] Missing parameters: id or filters")
+            LOGGER.error("[opencti_tool] Missing parameters: id or filters")
             return None
 
     """
-        Create a Narrative object
+        Create a Tool object
 
-        :param name: the name of the Narrative
-        :return Narrative object
+        :param name: the name of the Tool
+        :return Tool object
     """
 
     def create(self, **kwargs):
         stix_id = kwargs.get("stix_id", None)
         created_by = kwargs.get("createdBy", None)
         object_marking = kwargs.get("objectMarking", None)
         object_label = kwargs.get("objectLabel", None)
@@ -278,24 +293,25 @@
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
         description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
-        narrative_types = kwargs.get("narrative_types", None)
+        tool_types = kwargs.get("tool_types", None)
+        tool_version = kwargs.get("tool_version", None)
+        kill_chain_phases = kwargs.get("killChainPhases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
-        granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if name is not None:
-            LOGGER.info("Creating Narrative {%s}.", name)
+            LOGGER.info("Creating Tool {%s}.", name)
             query = """
-                mutation NarrativeAdd($input: NarrativeAddInput!) {
-                    narrativeAdd(input: $input) {
+                mutation ToolAdd($input: ToolAddInput!) {
+                    toolAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
             """
@@ -303,57 +319,54 @@
                 query,
                 {
                     "input": {
                         "stix_id": stix_id,
                         "createdBy": created_by,
                         "objectMarking": object_marking,
                         "objectLabel": object_label,
-                        "objectOrganization": granted_refs,
                         "externalReferences": external_references,
                         "revoked": revoked,
                         "confidence": confidence,
                         "lang": lang,
                         "created": created,
                         "modified": modified,
                         "name": name,
                         "description": description,
                         "aliases": aliases,
-                        "narrative_types": narrative_types,
+                        "tool_types": tool_types,
+                        "tool_version": tool_version,
+                        "killChainPhases": kill_chain_phases,
                         "x_opencti_stix_ids": x_opencti_stix_ids,
                         "update": update,
                     }
                 },
             )
-            return self.opencti.process_multiple_fields(result["data"]["narrativeAdd"])
+            return self.opencti.process_multiple_fields(result["data"]["toolAdd"])
         else:
-            LOGGER.error("[opencti_narrative] Missing parameters: name and description")
+            LOGGER.error("[opencti_tool] Missing parameters: name and description")
 
     """
-        Import an Narrative object from a STIX2 object
+        Import an Tool object from a STIX2 object
 
-        :param stixObject: the Stix-Object Narrative
-        :return Narrative object
+        :param stixObject: the Stix-Object Tool
+        :return Tool object
     """
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
         extras = kwargs.get("extras", {})
         update = kwargs.get("update", False)
         if stix_object is not None:
             # Search in extensions
             if "x_opencti_stix_ids" not in stix_object:
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
-            if "granted_refs" not in stix_object:
-                stix_object["granted_refs"] = self.opencti.get_attribute_in_extension(
-                    "granted_refs", stix_object
-                )
 
-            return self.opencti.narrative.create(
+            return self.opencti.tool.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
@@ -373,20 +386,23 @@
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
                 else None,
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
-                narrative_types=stix_object["narrative_types"]
-                if "narrative_types" in stix_object
+                tool_types=stix_object["tool_types"]
+                if "tool_types" in stix_object
+                else None,
+                tool_version=stix_object["tool_version"]
+                if "tool_version" in stix_object
+                else None,
+                killChainPhases=extras["kill_chain_phases_ids"]
+                if "kill_chain_phases_ids" in extras
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
-                else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_narrative] Missing parameters: stixObject")
+            LOGGER.error("[opencti_tool] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.0/pycti/entities/opencti_note.py` & `pycti-5.9.1/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_observed_data.py` & `pycti-5.9.1/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_opinion.py` & `pycti-5.9.1/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_report.py` & `pycti-5.9.1/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_stix.py` & `pycti-5.9.1/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_stix_core_object.py` & `pycti-5.9.1/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_stix_core_relationship.py` & `pycti-5.9.1/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-5.9.1/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_stix_domain_object.py` & `pycti-5.9.1/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-5.9.1/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-5.9.1/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-5.9.1/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_task.py` & `pycti-5.9.1/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_threat_actor.py` & `pycti-5.9.1/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_threat_actor_group.py` & `pycti-5.9.1/pycti/entities/opencti_threat_actor_group.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_threat_actor_individual.py` & `pycti-5.9.1/pycti/entities/opencti_threat_actor_individual.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_tool.py` & `pycti-5.9.1/pycti/entities/opencti_course_of_action.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import uuid
 
 from stix2.canonicalization.Canonicalize import canonicalize
 
 from pycti.entities import LOGGER
 
 
-class Tool:
+class CourseOfAction:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             standard_id
             entity_type
             parent_types
@@ -108,31 +108,16 @@
             }
             revoked
             confidence
             created
             modified
             name
             description
-            aliases
-            tool_types
-            tool_version
-            killChainPhases {
-                edges {
-                    node {
-                        id
-                        standard_id
-                        entity_type
-                        kill_chain_name
-                        phase_name
-                        x_opencti_order
-                        created
-                        modified
-                    }
-                }
-            }
+            x_opencti_aliases
+            x_mitre_id
             importFiles {
                 edges {
                     node {
                         id
                         name
                         size
                         metaData {
@@ -141,49 +126,52 @@
                         }
                     }
                 }
             }
         """
 
     @staticmethod
-    def generate_id(name):
+    def generate_id(name, x_mitre_id=None):
         name = name.lower().strip()
-        data = {"name": name}
+        if x_mitre_id is not None:
+            data = {"x_mitre_id": x_mitre_id}
+        else:
+            data = {"name": name}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
-        return "tool--" + id
+        return "course-of-action--" + id
 
     """
-        List Tool objects
+        List Course-Of-Action objects
 
         :param filters: the filters to apply
         :param search: the search keyword
         :param first: return the first n rows from the after ID (or the beginning if not set)
         :param after: ID of the first row for pagination
-        :return List of Tool objects
+        :return List of Course-Of-Action objects
     """
 
     def list(self, **kwargs):
         filters = kwargs.get("filters", None)
         search = kwargs.get("search", None)
-        first = kwargs.get("first", 100)
+        first = kwargs.get("first", 500)
         after = kwargs.get("after", None)
         order_by = kwargs.get("orderBy", None)
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
             first = 100
 
-        LOGGER.info("Listing Tools with filters %s.", json.dumps(filters))
+        LOGGER.info("Listing Courses-Of-Action with filters %s.", json.dumps(filters))
         query = (
             """
-            query Tools($filters: [ToolsFiltering], $search: String, $first: Int, $after: ID, $orderBy: ToolsOrdering, $orderMode: OrderingMode) {
-                tools(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
+            query CoursesOfAction($filters: [CoursesOfActionFiltering], $search: String, $first: Int, $after: ID, $orderBy: CoursesOfActionOrdering, $orderMode: OrderingMode) {
+                coursesOfAction(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
                     edges {
                         node {
                             """
             + (custom_attributes if custom_attributes is not None else self.properties)
             + """
                         }
                     }
@@ -207,84 +195,86 @@
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
         if get_all:
             final_data = []
-            data = self.opencti.process_multiple(result["data"]["tools"])
+            data = self.opencti.process_multiple(result["data"]["coursesOfAction"])
             final_data = final_data + data
-            while result["data"]["tools"]["pageInfo"]["hasNextPage"]:
-                after = result["data"]["tools"]["pageInfo"]["endCursor"]
-                LOGGER.info("Listing Tools after " + after)
+            while result["data"]["coursesOfAction"]["pageInfo"]["hasNextPage"]:
+                after = result["data"]["coursesOfAction"]["pageInfo"]["endCursor"]
+                LOGGER.info("Listing Courses-Of-Action after " + after)
                 result = self.opencti.query(
                     query,
                     {
                         "filters": filters,
                         "search": search,
                         "first": first,
                         "after": after,
                         "orderBy": order_by,
                         "orderMode": order_mode,
                     },
                 )
-                data = self.opencti.process_multiple(result["data"]["tools"])
+                data = self.opencti.process_multiple(result["data"]["coursesOfAction"])
                 final_data = final_data + data
             return final_data
         else:
             return self.opencti.process_multiple(
-                result["data"]["tools"], with_pagination
+                result["data"]["coursesOfAction"], with_pagination
             )
 
     """
-        Read a Tool object
+        Read a Course-Of-Action object
 
-        :param id: the id of the Tool
+        :param id: the id of the Course-Of-Action
         :param filters: the filters to apply if no id provided
-        :return Tool object
+        :return Course-Of-Action object
     """
 
     def read(self, **kwargs):
         id = kwargs.get("id", None)
         filters = kwargs.get("filters", None)
         custom_attributes = kwargs.get("customAttributes", None)
         if id is not None:
-            LOGGER.info("Reading Tool {%s}.", id)
+            LOGGER.info("Reading Course-Of-Action {%s}.", id)
             query = (
                 """
-                query Tool($id: String!) {
-                    tool(id: $id) {
+                query CourseOfAction($id: String!) {
+                    courseOfAction(id: $id) {
                         """
                 + (
                     custom_attributes
                     if custom_attributes is not None
                     else self.properties
                 )
                 + """
                     }
                 }
              """
             )
             result = self.opencti.query(query, {"id": id})
-            return self.opencti.process_multiple_fields(result["data"]["tool"])
+            return self.opencti.process_multiple_fields(
+                result["data"]["courseOfAction"]
+            )
         elif filters is not None:
             result = self.list(filters=filters)
             if len(result) > 0:
                 return result[0]
             else:
                 return None
         else:
-            LOGGER.error("[opencti_tool] Missing parameters: id or filters")
+            LOGGER.error("[opencti_course_of_action] Missing parameters: id or filters")
             return None
 
     """
-        Create a Tool object
+        Create a Course Of Action object
 
-        :param name: the name of the Tool
-        :return Tool object
+        :param name: the name of the Course Of Action
+        :return Course Of Action object
     """
 
     def create(self, **kwargs):
         stix_id = kwargs.get("stix_id", None)
         created_by = kwargs.get("createdBy", None)
         object_marking = kwargs.get("objectMarking", None)
         object_label = kwargs.get("objectLabel", None)
@@ -292,26 +282,25 @@
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
         description = kwargs.get("description", None)
-        aliases = kwargs.get("aliases", None)
-        tool_types = kwargs.get("tool_types", None)
-        tool_version = kwargs.get("tool_version", None)
-        kill_chain_phases = kwargs.get("killChainPhases", None)
+        x_opencti_aliases = kwargs.get("x_opencti_aliases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
+        x_mitre_id = kwargs.get("x_mitre_id", None)
+        granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if name is not None:
-            LOGGER.info("Creating Tool {%s}.", name)
+            LOGGER.info("Creating Course Of Action {%s}.", name)
             query = """
-                mutation ToolAdd($input: ToolAddInput!) {
-                    toolAdd(input: $input) {
+                mutation CourseOfActionAdd($input: CourseOfActionAddInput!) {
+                    courseOfActionAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
             """
@@ -319,54 +308,86 @@
                 query,
                 {
                     "input": {
                         "stix_id": stix_id,
                         "createdBy": created_by,
                         "objectMarking": object_marking,
                         "objectLabel": object_label,
+                        "objectOrganization": granted_refs,
                         "externalReferences": external_references,
                         "revoked": revoked,
                         "confidence": confidence,
                         "lang": lang,
                         "created": created,
                         "modified": modified,
                         "name": name,
                         "description": description,
-                        "aliases": aliases,
-                        "tool_types": tool_types,
-                        "tool_version": tool_version,
-                        "killChainPhases": kill_chain_phases,
+                        "x_opencti_aliases": x_opencti_aliases,
                         "x_opencti_stix_ids": x_opencti_stix_ids,
+                        "x_mitre_id": x_mitre_id,
                         "update": update,
                     }
                 },
             )
-            return self.opencti.process_multiple_fields(result["data"]["toolAdd"])
+            return self.opencti.process_multiple_fields(
+                result["data"]["courseOfActionAdd"]
+            )
         else:
-            LOGGER.error("[opencti_tool] Missing parameters: name and description")
+            LOGGER.error(
+                "[opencti_course_of_action] Missing parameters: name and description"
+            )
 
     """
-        Import an Tool object from a STIX2 object
+        Import an Course-Of-Action object from a STIX2 object
 
-        :param stixObject: the Stix-Object Tool
-        :return Tool object
+        :param stixObject: the Stix-Object Course-Of-Action
+        :return Course-Of-Action object
     """
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
         extras = kwargs.get("extras", {})
         update = kwargs.get("update", False)
         if stix_object is not None:
+            # Extract external ID
+            x_mitre_id = None
+            if "x_mitre_id" in stix_object:
+                x_mitre_id = stix_object["x_mitre_id"]
+            elif (
+                self.opencti.get_attribute_in_mitre_extension("id", stix_object)
+                is not None
+            ):
+                x_mitre_id = self.opencti.get_attribute_in_mitre_extension(
+                    "id", stix_object
+                )
+            elif "external_references" in stix_object:
+                for external_reference in stix_object["external_references"]:
+                    if (
+                        external_reference["source_name"] == "mitre-attack"
+                        or external_reference["source_name"] == "mitre-pre-attack"
+                        or external_reference["source_name"] == "mitre-mobile-attack"
+                        or external_reference["source_name"] == "amitt-attack"
+                    ):
+                        x_mitre_id = external_reference["external_id"]
+
             # Search in extensions
+            if "x_opencti_aliases" not in stix_object:
+                stix_object[
+                    "x_opencti_aliases"
+                ] = self.opencti.get_attribute_in_extension("aliases", stix_object)
             if "x_opencti_stix_ids" not in stix_object:
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
+            if "granted_refs" not in stix_object:
+                stix_object["granted_refs"] = self.opencti.get_attribute_in_extension(
+                    "granted_refs", stix_object
+                )
 
-            return self.opencti.tool.create(
+            return self.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
                 else None,
@@ -385,24 +406,19 @@
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
                 else None,
-                aliases=self.opencti.stix2.pick_aliases(stix_object),
-                tool_types=stix_object["tool_types"]
-                if "tool_types" in stix_object
-                else None,
-                tool_version=stix_object["tool_version"]
-                if "tool_version" in stix_object
-                else None,
-                killChainPhases=extras["kill_chain_phases_ids"]
-                if "kill_chain_phases_ids" in extras
-                else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
+                x_opencti_aliases=self.opencti.stix2.pick_aliases(stix_object),
+                x_mitre_id=x_mitre_id,
+                objectOrganization=stix_object["granted_refs"]
+                if "granted_refs" in stix_object
+                else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_tool] Missing parameters: stixObject")
+            LOGGER.error("[opencti_course_of_action] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.0/pycti/entities/opencti_vocabulary.py` & `pycti-5.9.1/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/entities/opencti_vulnerability.py` & `pycti-5.9.1/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/utils/constants.py` & `pycti-5.9.1/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/utils/opencti_stix2.py` & `pycti-5.9.1/pycti/utils/opencti_stix2.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,15 +557,15 @@
                             file_name=file["name"],
                             data=base64.b64decode(file["data"]),
                             mime_type=file["mime_type"],
                         )
                 self.mapping_cache[generated_ref_id] = generated_ref_id
                 external_references_ids.append(external_reference_id)
                 if stix_object["type"] in [
-                    "threat-actor-group",
+                    "threat-actor",
                     "intrusion-set",
                     "campaign",
                     "incident",
                     "malware",
                     "relationship",
                 ] and (types is not None and "external-reference-as-report" in types):
                     # Add a corresponding report
@@ -1842,14 +1842,15 @@
                 "Indicator": self.opencti.indicator.read,
                 "Infrastructure": self.opencti.infrastructure.read,
                 "Intrusion-Set": self.opencti.intrusion_set.read,
                 "Location": self.opencti.location.read,
                 "Language": self.opencti.language.read,
                 "Malware": self.opencti.malware.read,
                 "Malware-Analysis": self.opencti.malware_analysis.read,
+                "Threat-Actor": self.opencti.threat_actor.read,
                 "Threat-Actor-Group": self.opencti.threat_actor_group.read,
                 "Threat-Actor-Individual": self.opencti.threat_actor_individual.read,
                 "Tool": self.opencti.tool.read,
                 "Vulnerability": self.opencti.vulnerability.read,
                 "Incident": self.opencti.incident.read,
                 "Stix-Core-Object": self.opencti.stix_core_object.read,
                 "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.read,
@@ -2011,14 +2012,15 @@
             "Indicator": self.opencti.indicator.read,
             "Infrastructure": self.opencti.infrastructure.read,
             "Intrusion-Set": self.opencti.intrusion_set.read,
             "Location": self.opencti.location.read,
             "Language": self.opencti.language.read,
             "Malware": self.opencti.malware.read,
             "Malware-Analysis": self.opencti.malware_analysis.read,
+            "Threat-Actor": self.opencti.threat_actor.read,
             "Threat-Actor-Group": self.opencti.threat_actor_group.read,
             "Threat-Actor-Individual": self.opencti.threat_actor_individual.read,
             "Tool": self.opencti.tool.read,
             "Narrative": self.opencti.narrative.read,
             "Vulnerability": self.opencti.vulnerability.read,
             "Incident": self.opencti.incident.read,
             "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.read,
@@ -2155,14 +2157,15 @@
             "Indicator": self.opencti.indicator.list,
             "Infrastructure": self.opencti.infrastructure.list,
             "Intrusion-Set": self.opencti.intrusion_set.list,
             "Location": self.opencti.location.list,
             "Language": self.opencti.language.list,
             "Malware": self.opencti.malware.list,
             "Malware-Analysis": self.opencti.malware_analysis.list,
+            "Threat-Actor": self.opencti.threat_actor_group.list,
             "Threat-Actor-Group": self.opencti.threat_actor_group.list,
             "Threat-Actor-Individual": self.opencti.threat_actor_individual.list,
             "Tool": self.opencti.tool.list,
             "Narrative": self.opencti.narrative.list,
             "Vulnerability": self.opencti.vulnerability.list,
             "Incident": self.opencti.incident.list,
             "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.list,
```

### Comparing `pycti-5.9.0/pycti/utils/opencti_stix2_splitter.py` & `pycti-5.9.1/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/utils/opencti_stix2_update.py` & `pycti-5.9.1/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti/utils/opencti_stix2_utils.py` & `pycti-5.9.1/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti.egg-info/PKG-INFO` & `pycti-5.9.1/pycti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.9.0
+Version: 5.9.1
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.9.0 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.9.1 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.9.0/pycti.egg-info/SOURCES.txt` & `pycti-5.9.1/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/pycti.egg-info/requires.txt` & `pycti-5.9.1/pycti.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 [:sys_platform == "linux" or sys_platform == "darwin"]
 python-magic~=0.4.27
 
 [:sys_platform == "win32"]
 python-magic-bin~=0.4.14
 
 [dev]
-black~=23.3.0
+black~=23.7.0
 build~=0.10.0
 isort~=5.12.0
 types-pytz~=2023.3.0.0
 pre-commit~=3.3.2
 pytest-cases~=3.6.13
 pytest-cov~=4.1.0
-pytest_randomly~=3.12.0
+pytest_randomly~=3.13.0
 pytest~=7.4.0
 types-python-dateutil~=2.8.19
 wheel~=0.40.0
 
 [doc]
 autoapi~=2.0.1
 sphinx-autodoc-typehints~=1.23.0
```

### Comparing `pycti-5.9.0/pyproject.toml` & `pycti-5.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-5.9.0/setup.cfg` & `pycti-5.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 	setuptools~=68.0.0
 	filigran-sseclient~=1.0.0
 	stix2~=3.0.1
 	cachetools~=5.3.0
 
 [options.extras_require]
 dev = 
-	black~=23.3.0
+	black~=23.7.0
 	build~=0.10.0
 	isort~=5.12.0
 	types-pytz~=2023.3.0.0
 	pre-commit~=3.3.2
 	pytest-cases~=3.6.13
 	pytest-cov~=4.1.0
-	pytest_randomly~=3.12.0
+	pytest_randomly~=3.13.0
 	pytest~=7.4.0
 	types-python-dateutil~=2.8.19
 	wheel~=0.40.0
 doc = 
 	autoapi~=2.0.1
 	sphinx-autodoc-typehints~=1.23.0
 	sphinx-rtd-theme~=1.2.1
```


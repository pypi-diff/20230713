# Comparing `tmp/contentctl-1.0.1.tar.gz` & `tmp/contentctl-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contentctl-1.0.1.tar", max compression
+gzip compressed data, was "contentctl-2.0.0.tar", max compression
```

## Comparing `contentctl-1.0.1.tar` & `contentctl-2.0.0.tar`

### file list

```diff
@@ -1,124 +1,132 @@
--rw-r--r--   0        0        0    11344 2023-06-12 22:32:39.582106 contentctl-1.0.1/LICENSE.md
--rw-r--r--   0        0        0    17554 2023-06-12 22:32:39.582106 contentctl-1.0.1/README.md
--rw-r--r--   0        0        0       22 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/__init__.py
--rw-r--r--   0        0        0     5844 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/deploy.py
--rw-r--r--   0        0        0     5580 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/DataManipulation.py
--rw-r--r--   0        0        0     7180 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/DetectionTestingManager.py
--rw-r--r--   0        0        0    16208 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/GitHubService.py
--rw-r--r--   0        0        0     2259 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
--rw-r--r--   0        0        0    27291 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
--rw-r--r--   0        0        0     4051 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
--rw-r--r--   0        0        0      363 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
--rw-r--r--   0        0        0     3902 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingView.py
--rw-r--r--   0        0        0     2050 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
--rw-r--r--   0        0        0     1363 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
--rw-r--r--   0        0        0     4711 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
--rw-r--r--   0        0        0      857 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/doc_gen.py
--rw-r--r--   0        0        0     3288 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/generate.py
--rw-r--r--   0        0        0     1921 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/initialize.py
--rw-r--r--   0        0        0     9333 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/initialize_old.py
--rw-r--r--   0        0        0      920 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/new_content.py
--rw-r--r--   0        0        0     1022 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/reporting.py
--rw-r--r--   0        0        0     3014 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/test.py
--rw-r--r--   0        0        0     2741 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/validate.py
--rw-r--r--   0        0        0    13836 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/contentctl.py
--rw-r--r--   0        0        0     3885 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/enrichments/attack_enrichment.py
--rw-r--r--   0        0        0      713 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/enrichments/cve_enrichment.py
--rw-r--r--   0        0        0     1944 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/enrichments/splunk_app_enrichment.py
--rw-r--r--   0        0        0      584 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/helper/config_handler.py
--rw-r--r--   0        0        0     1070 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/helper/link_validator.py
--rw-r--r--   0        0        0        0 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/helper/logger.py
--rw-r--r--   0        0        0    15314 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/helper/utils.py
--rw-r--r--   0        0        0     1857 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/baseline_builder.py
--rw-r--r--   0        0        0     2227 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/basic_builder.py
--rw-r--r--   0        0        0    11747 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/detection_builder.py
--rw-r--r--   0        0        0    11127 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/director.py
--rw-r--r--   0        0        0     1244 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/investigation_builder.py
--rw-r--r--   0        0        0     4485 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/new_content_generator.py
--rw-r--r--   0        0        0     4576 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/new_content_questions.py
--rw-r--r--   0        0        0     1954 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/playbook_builder.py
--rw-r--r--   0        0        0     4738 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/story_builder.py
--rw-r--r--   0        0        0      814 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/yml_reader.py
--rw-r--r--   0        0        0     7621 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/app.py
--rw-r--r--   0        0        0     2560 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/baseline.py
--rw-r--r--   0        0        0      711 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/baseline_tags.py
--rw-r--r--   0        0        0     1864 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/config.py
--rw-r--r--   0        0        0     2290 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/constants.py
--rw-r--r--   0        0        0     1913 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment.py
--rw-r--r--   0        0        0      141 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_email.py
--rw-r--r--   0        0        0      164 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_notable.py
--rw-r--r--   0        0        0      201 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_phantom.py
--rw-r--r--   0        0        0      111 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_rba.py
--rw-r--r--   0        0        0      193 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_scheduling.py
--rw-r--r--   0        0        0      129 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_slack.py
--rw-r--r--   0        0        0     6191 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/detection.py
--rw-r--r--   0        0        0     4283 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/detection_tags.py
--rw-r--r--   0        0        0     1647 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/enums.py
--rw-r--r--   0        0        0     2444 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/investigation.py
--rw-r--r--   0        0        0      191 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/investigation_tags.py
--rw-r--r--   0        0        0      425 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/lookup.py
--rw-r--r--   0        0        0      271 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/macro.py
--rw-r--r--   0        0        0      219 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/mitre_attack_enrichment.py
--rw-r--r--   0        0        0      589 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/playbook.py
--rw-r--r--   0        0        0      315 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/playbook_tags.py
--rw-r--r--   0        0        0     6522 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/repo_config.py
--rw-r--r--   0        0        0      139 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/security_content_object.py
--rw-r--r--   0        0        0     1696 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/story.py
--rw-r--r--   0        0        0      926 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/story_tags.py
--rw-r--r--   0        0        0    22399 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/test_config.py
--rw-r--r--   0        0        0      316 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/unit_test.py
--rw-r--r--   0        0        0      605 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/unit_test_attack_data.py
--rw-r--r--   0        0        0      255 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/unit_test_baseline.py
--rw-r--r--   0        0        0     8186 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/unit_test_result.py
--rw-r--r--   0        0        0      602 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/unit_test_test.py
--rw-r--r--   0        0        0     3089 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/api_json_output.py
--rw-r--r--   0        0        0     1701 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/attack_nav_output.py
--rw-r--r--   0        0        0     2130 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/attack_nav_writer.py
--rw-r--r--   0        0        0     3946 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/ba_yml_output.py
--rw-r--r--   0        0        0     5756 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/conf_output.py
--rw-r--r--   0        0        0     2728 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/conf_writer.py
--rw-r--r--   0        0        0     3238 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/doc_md_output.py
--rw-r--r--   0        0        0     3050 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/finding_report_writer.py
--rw-r--r--   0        0        0     1089 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/jinja_writer.py
--rw-r--r--   0        0        0      210 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/json_writer.py
--rw-r--r--   0        0        0     3065 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/new_content_yml_output.py
--rw-r--r--   0        0        0     1059 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/svg_output.py
--rw-r--r--   0        0        0      745 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/analyticstories_detections.j2
--rw-r--r--   0        0        0      496 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/analyticstories_investigations.j2
--rw-r--r--   0        0        0      586 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/analyticstories_stories.j2
--rw-r--r--   0        0        0      180 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/collections.j2
--rw-r--r--   0        0        0      670 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/detection_count.j2
--rw-r--r--   0        0        0      671 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/detection_coverage.j2
--rw-r--r--   0        0        0     1002 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_detection_page.j2
--rw-r--r--   0        0        0     6586 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_detections.j2
--rw-r--r--   0        0        0     1471 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_navigation.j2
--rw-r--r--   0        0        0      203 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_navigation_pages.j2
--rw-r--r--   0        0        0     1681 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_playbooks.j2
--rw-r--r--   0        0        0      679 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_playbooks_page.j2
--rw-r--r--   0        0        0     1822 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_stories.j2
--rw-r--r--   0        0        0      874 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_story_page.j2
--rw-r--r--   0        0        0      994 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/es_investigations_investigations.j2
--rw-r--r--   0        0        0      369 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/es_investigations_stories.j2
--rw-r--r--   0        0        0     1432 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/finding_report.j2
--rw-r--r--   0        0        0      190 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/header.j2
--rw-r--r--   0        0        0      424 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/macros.j2
--rw-r--r--   0        0        0      282 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/macros_detections.j2
--rw-r--r--   0        0        0      221 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/panel.j2
--rw-r--r--   0        0        0     1840 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/savedsearches_baselines.j2
--rw-r--r--   0        0        0     5290 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/savedsearches_detections.j2
--rw-r--r--   0        0        0     1380 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/savedsearches_investigations.j2
--rw-r--r--   0        0        0     1416 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/transforms.j2
--rw-r--r--   0        0        0      925 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/workflow_actions.j2
--rw-r--r--   0        0        0      235 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/yml_writer.py
--rw-r--r--   0        0        0     3843 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/templates/app_default.yml
--rw-r--r--   0        0        0      662 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/templates/contentctl_default.yml
--rw-r--r--   0        0        0     9381 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/templates/datamodels_cim.conf
--rw-r--r--   0        0        0      480 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/templates/datamodels_custom.conf
--rw-r--r--   0        0        0     3262 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/templates/detections/anomalous_usage_of_7zip.yml
--rw-r--r--   0        0        0      159 2023-06-12 22:32:39.590106 contentctl-1.0.1/contentctl/templates/macros/security_content_ctime.yml
--rw-r--r--   0        0        0      162 2023-06-12 22:32:39.590106 contentctl-1.0.1/contentctl/templates/macros/security_content_summariesonly.yml
--rw-r--r--   0        0        0       90 2023-06-12 22:32:39.590106 contentctl-1.0.1/contentctl/templates/splunk_app/metadata/default.meta
--rw-r--r--   0        0        0     3086 2023-06-12 22:32:39.590106 contentctl-1.0.1/contentctl/templates/stories/cobalt_strike.yml
--rw-r--r--   0        0        0      501 2023-06-12 22:32:39.590106 contentctl-1.0.1/contentctl/templates/tests/anomalous_usage_of_7zip.test.yml
--rw-r--r--   0        0        0      729 2023-06-12 22:32:39.590106 contentctl-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    18660 1970-01-01 00:00:00.000000 contentctl-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-07-13 00:36:19.774439 contentctl-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0    17554 2023-07-13 00:36:19.774439 contentctl-2.0.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/__init__.py
+-rw-r--r--   0        0        0     2999 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/apav_deploy.py
+-rw-r--r--   0        0        0     6963 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/api_deploy.py
+-rw-r--r--   0        0        0     5580 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/DataManipulation.py
+-rw-r--r--   0        0        0     7180 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/DetectionTestingManager.py
+-rw-r--r--   0        0        0    16208 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/GitHubService.py
+-rw-r--r--   0        0        0     2259 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
+-rw-r--r--   0        0        0    27462 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
+-rw-r--r--   0        0        0     4051 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
+-rw-r--r--   0        0        0      363 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
+-rw-r--r--   0        0        0     3907 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingView.py
+-rw-r--r--   0        0        0     2050 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
+-rw-r--r--   0        0        0     1368 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
+-rw-r--r--   0        0        0     4780 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
+-rw-r--r--   0        0        0      857 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/doc_gen.py
+-rw-r--r--   0        0        0     3348 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/generate.py
+-rw-r--r--   0        0        0     3000 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/initialize.py
+-rw-r--r--   0        0        0     9333 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/initialize_old.py
+-rw-r--r--   0        0        0     1294 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/inspect.py
+-rw-r--r--   0        0        0      920 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/new_content.py
+-rw-r--r--   0        0        0     1022 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/reporting.py
+-rw-r--r--   0        0        0     3014 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/test.py
+-rw-r--r--   0        0        0     2741 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/actions/validate.py
+-rw-r--r--   0        0        0    15135 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/contentctl.py
+-rw-r--r--   0        0        0     4392 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/enrichments/attack_enrichment.py
+-rw-r--r--   0        0        0     3242 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/enrichments/cve_enrichment.py
+-rw-r--r--   0        0        0     3418 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/enrichments/splunk_app_enrichment.py
+-rw-r--r--   0        0        0     1198 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/helper/config_handler.py
+-rw-r--r--   0        0        0     7238 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/helper/link_validator.py
+-rw-r--r--   0        0        0        0 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/helper/logger.py
+-rw-r--r--   0        0        0    15586 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/helper/utils.py
+-rw-r--r--   0        0        0     1906 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/baseline_builder.py
+-rw-r--r--   0        0        0     2291 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/basic_builder.py
+-rw-r--r--   0        0        0    13759 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/detection_builder.py
+-rw-r--r--   0        0        0    11189 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/director.py
+-rw-r--r--   0        0        0     1244 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/investigation_builder.py
+-rw-r--r--   0        0        0     4485 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/new_content_generator.py
+-rw-r--r--   0        0        0     4576 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/new_content_questions.py
+-rw-r--r--   0        0        0     2100 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/playbook_builder.py
+-rw-r--r--   0        0        0     4755 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/story_builder.py
+-rw-r--r--   0        0        0     1016 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/input/yml_reader.py
+-rw-r--r--   0        0        0     7699 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/app.py
+-rw-r--r--   0        0        0     1930 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/baseline.py
+-rw-r--r--   0        0        0      711 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/baseline_tags.py
+-rw-r--r--   0        0        0     5658 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/config.py
+-rw-r--r--   0        0        0     3519 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/constants.py
+-rw-r--r--   0        0        0     1136 2023-07-13 00:36:19.774439 contentctl-2.0.0/contentctl/objects/deployment.py
+-rw-r--r--   0        0        0      141 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_email.py
+-rw-r--r--   0        0        0      164 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_notable.py
+-rw-r--r--   0        0        0      201 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_phantom.py
+-rw-r--r--   0        0        0      111 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_rba.py
+-rw-r--r--   0        0        0      193 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_scheduling.py
+-rw-r--r--   0        0        0      129 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/deployment_slack.py
+-rw-r--r--   0        0        0     5630 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/detection.py
+-rw-r--r--   0        0        0     5921 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/detection_tags.py
+-rw-r--r--   0        0        0     2882 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/enums.py
+-rw-r--r--   0        0        0     2150 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/investigation.py
+-rw-r--r--   0        0        0      191 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/investigation_tags.py
+-rw-r--r--   0        0        0     1002 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/lookup.py
+-rw-r--r--   0        0        0      845 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/macro.py
+-rw-r--r--   0        0        0      219 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/mitre_attack_enrichment.py
+-rw-r--r--   0        0        0      920 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/playbook.py
+-rw-r--r--   0        0        0      315 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/playbook_tags.py
+-rw-r--r--   0        0        0     6522 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/repo_config.py
+-rw-r--r--   0        0        0     1875 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/security_content_object.py
+-rw-r--r--   0        0        0     1531 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/story.py
+-rw-r--r--   0        0        0     1213 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/story_tags.py
+-rw-r--r--   0        0        0    22343 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/test_config.py
+-rw-r--r--   0        0        0      805 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/unit_test.py
+-rw-r--r--   0        0        0      580 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/unit_test_attack_data.py
+-rw-r--r--   0        0        0      255 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/unit_test_baseline.py
+-rw-r--r--   0        0        0     8186 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/unit_test_result.py
+-rw-r--r--   0        0        0      602 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/objects/unit_test_test.py
+-rw-r--r--   0        0        0     3089 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/api_json_output.py
+-rw-r--r--   0        0        0     1701 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/attack_nav_output.py
+-rw-r--r--   0        0        0     2130 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/attack_nav_writer.py
+-rw-r--r--   0        0        0     3946 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/ba_yml_output.py
+-rw-r--r--   0        0        0    11388 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/conf_output.py
+-rw-r--r--   0        0        0     2958 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/conf_writer.py
+-rw-r--r--   0        0        0     3238 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/doc_md_output.py
+-rw-r--r--   0        0        0     3050 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/finding_report_writer.py
+-rw-r--r--   0        0        0     1089 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/jinja_writer.py
+-rw-r--r--   0        0        0      210 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/json_writer.py
+-rw-r--r--   0        0        0     3065 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/new_content_yml_output.py
+-rw-r--r--   0        0        0     1059 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/svg_output.py
+-rw-r--r--   0        0        0      745 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/analyticstories_detections.j2
+-rw-r--r--   0        0        0      496 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/analyticstories_investigations.j2
+-rw-r--r--   0        0        0      586 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/analyticstories_stories.j2
+-rw-r--r--   0        0        0     1011 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/app.conf.j2
+-rw-r--r--   0        0        0      180 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/collections.j2
+-rw-r--r--   0        0        0      670 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/detection_count.j2
+-rw-r--r--   0        0        0      671 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/detection_coverage.j2
+-rw-r--r--   0        0        0     1002 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_detection_page.j2
+-rw-r--r--   0        0        0     6586 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_detections.j2
+-rw-r--r--   0        0        0     1471 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_navigation.j2
+-rw-r--r--   0        0        0      203 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_navigation_pages.j2
+-rw-r--r--   0        0        0     1681 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_playbooks.j2
+-rw-r--r--   0        0        0      679 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_playbooks_page.j2
+-rw-r--r--   0        0        0     1822 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_stories.j2
+-rw-r--r--   0        0        0      874 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/doc_story_page.j2
+-rw-r--r--   0        0        0      994 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/es_investigations_investigations.j2
+-rw-r--r--   0        0        0      369 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/es_investigations_stories.j2
+-rw-r--r--   0        0        0     1432 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/finding_report.j2
+-rw-r--r--   0        0        0      177 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/header.j2
+-rw-r--r--   0        0        0      424 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/macros.j2
+-rw-r--r--   0        0        0      282 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/macros_detections.j2
+-rw-r--r--   0        0        0      221 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/panel.j2
+-rw-r--r--   0        0        0     1474 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/savedsearches_baselines.j2
+-rw-r--r--   0        0        0     5566 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/savedsearches_detections.j2
+-rw-r--r--   0        0        0     1390 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/savedsearches_investigations.j2
+-rw-r--r--   0        0        0       90 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/splunk_app/metadata/default.meta
+-rw-r--r--   0        0        0     1003 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/splunk_app/static/appIcon.png
+-rw-r--r--   0        0        0     2222 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/splunk_app/static/appIcon_2x.png
+-rw-r--r--   0        0        0     1416 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/transforms.j2
+-rw-r--r--   0        0        0      925 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/templates/workflow_actions.j2
+-rw-r--r--   0        0        0      235 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/output/yml_writer.py
+-rw-r--r--   0        0        0      133 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/README
+-rw-r--r--   0        0        0     1293 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/app_default.yml
+-rw-r--r--   0        0        0     9381 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/datamodels_cim.conf
+-rw-r--r--   0        0        0      480 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/datamodels_custom.conf
+-rw-r--r--   0        0        0     3312 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml
+-rw-r--r--   0        0        0     3508 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/detections/anomalous_usage_of_7zip_test_fail.yml
+-rw-r--r--   0        0        0     3391 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/detections/anomalous_usage_of_7zip_validation_fail.yml
+-rw-r--r--   0        0        0      159 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/macros/security_content_ctime.yml
+-rw-r--r--   0        0        0      162 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/macros/security_content_summariesonly.yml
+-rw-r--r--   0        0        0     3095 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/stories/cobalt_strike.yml
+-rw-r--r--   0        0        0      949 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/stories/splunk_app/metadata/app.conf.j2
+-rw-r--r--   0        0        0       90 2023-07-13 00:36:19.778439 contentctl-2.0.0/contentctl/templates/stories/splunk_app/metadata/default.meta
+-rw-r--r--   0        0        0      796 2023-07-13 00:36:19.778439 contentctl-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    18763 1970-01-01 00:00:00.000000 contentctl-2.0.0/PKG-INFO
```

### Comparing `contentctl-1.0.1/LICENSE.md` & `contentctl-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/README.md` & `contentctl-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/deploy.py` & `contentctl-2.0.0/contentctl/actions/api_deploy.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,125 +5,129 @@
 from requests.auth import HTTPBasicAuth
 
 from dataclasses import dataclass
 from configparser import RawConfigParser
 import splunklib.client as client
 
 from contentctl.objects.config import Config
-
+import pathlib
 
 @dataclass(frozen=True)
-class DeployInputDto:
-    path: str
+class API_DeployInputDto:
+    path: pathlib.Path
     config: Config
 
 
-class Deploy:
-    def fix_newlines_in_conf_files(self, conf_path: str) -> RawConfigParser:
+class API_Deploy:
+    def fix_newlines_in_conf_files(self, conf_path: pathlib.Path) -> RawConfigParser:
         parser = RawConfigParser()
         with open(conf_path, "r") as conf_data_file:
             conf_data = conf_data_file.read()
 
         # ConfigParser cannot read multipleline strings that simply escape the newline character with \
         # To include a newline, you need to include a space at the beginning of the newline.
         # We will simply replace all \NEWLINE with NEWLINESPACE (removing the leading literal \).
         # We will discuss whether we intend to make these changes to the underlying conf files
         # or just apply the changes here
         conf_data = conf_data.replace("\\\n", "\n ")
 
         parser.read_string(conf_data)
         return parser
 
-    def execute(self, input_dto: DeployInputDto) -> None:
-
-        splunk_args = {
-            "host": input_dto.config.deploy.server,
-            "port": 8089,
-            "username": input_dto.config.deploy.username,
-            "password": input_dto.config.deploy.password,
-            "owner": "nobody",
-            "app": input_dto.config.deploy.app,
-        }
-        service = client.connect(**splunk_args)
-
-        macros_parser = self.fix_newlines_in_conf_files(
-            os.path.join(
-                input_dto.path,
-                input_dto.config.build.splunk_app.path,
-                "default",
-                "macros.conf",
+    def execute(self, input_dto: API_DeployInputDto) -> None:
+        if len(input_dto.config.deployments.rest_api_deployments) == 0:
+            raise Exception("No rest_api_deployments defined in 'contentctl.yml'")
+        app_path =  pathlib.Path(input_dto.config.build.path_root)/input_dto.config.build.name
+        if not app_path.is_dir():
+            raise Exception(f"The unpackaged app does not exist at the path {app_path}. Please run 'contentctl build' to generate the app.")
+        for target in input_dto.config.deployments.rest_api_deployments:
+            print(f"Deploying '{input_dto.config.build.name}' to target '{target.server}' [{target.description}]")
+            splunk_args = {
+                "host": target.server,
+                "port": target.port,
+                "username": target.username,
+                "password": target.password,
+                "owner": "nobody",
+                "app": "search",
+            }
+            print("Warning - we are currently deploying all content into the 'search' app. "
+                  "At this time, this means the user does not have to install the app "
+                  "manually, but this will change")
+            service = client.connect(**splunk_args)
+
+                
+            macros_parser = self.fix_newlines_in_conf_files(
+                app_path/"default"/"macros.conf"
             )
-        )
-        import tqdm
+            import tqdm
 
-        bar_format_macros = (
-            f"Deploying macros        "
-            + "{percentage:3.0f}%[{bar:20}]"
-            + "[{n_fmt}/{total_fmt} | ETA: {remaining}]"
-        )
-        bar_format_detections = (
-            f"Deploying saved searches"
-            + "{percentage:3.0f}%[{bar:20}]"
-            + "[{n_fmt}/{total_fmt} | ETA: {remaining}]"
-        )
-        for section in tqdm.tqdm(
-            macros_parser.sections(), bar_format=bar_format_macros
-        ):
-            try:
-                service.post("properties/macros", __stanza=section)
-                service.post("properties/macros/" + section, **macros_parser[section])
-                # print("Deployed macro: " + section)
-            except Exception as e:
-                tqdm.tqdm.write(f"Error deploying macro {section}: {str(e)}")
-
-        detection_parser = RawConfigParser()
-        detection_parser = self.fix_newlines_in_conf_files(
-            os.path.join(
-                input_dto.path,
-                input_dto.config.build.splunk_app.path,
-                "default",
-                "savedsearches.conf",
+            bar_format_macros = (
+                f"Deploying macros        "
+                + "{percentage:3.0f}%[{bar:20}]"
+                + "[{n_fmt}/{total_fmt} | ETA: {remaining}]"
+            )
+            bar_format_detections = (
+                f"Deploying saved searches"
+                + "{percentage:3.0f}%[{bar:20}]"
+                + "[{n_fmt}/{total_fmt} | ETA: {remaining}]"
             )
-        )
-        try:
-            service.delete("saved/searches/MSCA - Anomalous usage of 7zip - Rule")
-        except Exception as e:
-            pass
-
-        for section in tqdm.tqdm(
-            detection_parser.sections(), bar_format=bar_format_detections
-        ):
-            try:
-                if section.startswith(input_dto.config.build.splunk_app.prefix):
-                    params = detection_parser[section]
-                    params["name"] = section
-                    response_actions = []
-                    if (
-                        input_dto.config.detection_configuration.notable
-                        and input_dto.config.detection_configuration.notable.rule_description
-                    ):
-                        response_actions.append("notable")
-                    if (
-                        input_dto.config.detection_configuration.rba
-                        and input_dto.config.detection_configuration.rba.enabled
-                    ):
-                        response_actions.append("risk")
-                    params["actions"] = ",".join(response_actions)
-                    params["request.ui_dispatch_app"] = "ES Content Updates"
-                    params["request.ui_dispatch_view"] = "ES Content Updates"
-                    params["alert_type"] = params.pop("counttype")
-                    params["alert_comparator"] = params.pop("relation")
-                    params["alert_threshold"] = params.pop("quantity")
-                    params.pop("enablesched")
-
-                    service.post("saved/searches", **params)
-
-                    # print("Deployed detection: " + params["name"])
-            except Exception as e:
-                tqdm.tqdm.write(f"Error deploying saved search {section}: {str(e)}")
+            for section in tqdm.tqdm(
+                macros_parser.sections(), bar_format=bar_format_macros
+            ):
+                try:
+                    service.post("properties/macros", __stanza=section)
+                    service.post("properties/macros/" + section, **macros_parser[section])
+                    tqdm.tqdm.write(f"Deployed macro [{section}]")
+                except Exception as e:
+                    tqdm.tqdm.write(f"Error deploying macro {section}: {str(e)}")
+
+            detection_parser = RawConfigParser()
+            detection_parser = self.fix_newlines_in_conf_files(
+                app_path/"default"/"savedsearches.conf",
+            )
+            
+
+            for section in tqdm.tqdm(
+                detection_parser.sections(), bar_format=bar_format_detections
+            ):
+                try:
+                    if section.startswith(input_dto.config.build.prefix):
+                        params = detection_parser[section]
+                        params["name"] = section
+                        response_actions = []
+                        if (
+                            input_dto.config.detection_configuration.notable
+                            and input_dto.config.detection_configuration.notable.rule_description
+                        ):
+                            response_actions.append("notable")
+                        if (
+                            input_dto.config.detection_configuration.rba
+                            and input_dto.config.detection_configuration.rba.enabled
+                        ):
+                            response_actions.append("risk")
+                        params["actions"] = ",".join(response_actions)
+                        params["request.ui_dispatch_app"] = "ES Content Updates"
+                        params["request.ui_dispatch_view"] = "ES Content Updates"
+                        params["alert_type"] = params.pop("counttype")
+                        params["alert_comparator"] = params.pop("relation")
+                        params["alert_threshold"] = params.pop("quantity")
+                        params.pop("enablesched")
+                        
+                        try:
+                            service.saved_searches.delete(section)
+                            #tqdm.tqdm.write(f"Deleted old saved search: {section}")
+                        except Exception as e:
+                            #tqdm.tqdm.write(f"Error deleting savedsearch '{section}' :[{str(e)}]")
+                            pass
+                        
+                        service.post("saved/searches", **params)
+                        tqdm.tqdm.write(f"Deployed savedsearch [{section}]")
+                
+                except Exception as e:
+                    tqdm.tqdm.write(f"Error deploying saved search {section}: {str(e)}")
 
         # story_parser = RawConfigParser()
         # story_parser.read(os.path.join(input_dto.path, input_dto.config.build.splunk_app.path, "default", "analyticstories.conf"))
 
         # for section in story_parser.sections():
         #     if section.startswith("analytic_story"):
         #         params = story_parser[section]
```

### Comparing `contentctl-1.0.1/contentctl/actions/detection_testing/DataManipulation.py` & `contentctl-2.0.0/contentctl/actions/detection_testing/DataManipulation.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/detection_testing/DetectionTestingManager.py` & `contentctl-2.0.0/contentctl/actions/detection_testing/DetectionTestingManager.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/detection_testing/GitHubService.py` & `contentctl-2.0.0/contentctl/actions/detection_testing/GitHubService.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/detection_testing/generate_detection_coverage_badge.py` & `contentctl-2.0.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py` & `contentctl-2.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 class DetectionTestingManagerOutputDto:
     inputQueue: list[Detection] = Field(default_factory=list)
     outputQueue: list[Detection] = Field(default_factory=list)
     currentTestingQueue: dict[str, Union[Detection, None]] = Field(default_factory=dict)
     start_time: Union[datetime.datetime, None] = None
     replay_index: str = "CONTENTCTL_TESTING_INDEX"
     replay_host: str = "CONTENTCTL_HOST"
-    timeout_seconds: int = 120
+    timeout_seconds: int = 15
     terminate: bool = False
 
 
 class DetectionTestingInfrastructure(BaseModel, abc.ABC):
     # thread: threading.Thread = threading.Thread()
     config: TestConfig
     sync_obj: DetectionTestingManagerOutputDto
@@ -354,19 +354,19 @@
             except Exception as e:
                 self.pbar.write(f"Error testing detection: {str(e)}")
             finally:
                 self.sync_obj.outputQueue.append(detection)
                 self.sync_obj.currentTestingQueue[self.get_name()] = None
 
     def test_detection(self, detection: Detection):
-        if detection.test is None:
+        if detection.tests is None:
             self.pbar.write(f"No test(s) found for {detection.name}")
             return
 
-        for test in detection.test.tests:
+        for test in detection.tests:
             self.execute_test(detection, test)
 
     def format_pbar_string(
         self,
         test_name: str,
         state: str,
         start_time: Union[float, None],
@@ -392,30 +392,30 @@
         return new_string
 
     def execute_test(
         self, detection: Detection, test: UnitTestTest, FORCE_ALL_TIME: bool = True
     ):
         start_time = time.time()
         self.pbar.reset()
-        self.format_pbar_string(test.name, "Beginning Test", start_time)
+        self.format_pbar_string(f"{detection.name}:{test.name}", "Beginning Test", start_time)
         # https://github.com/WoLpH/python-progressbar/issues/164
         # Use NullBar if there is more than 1 container or we are running
         # in a non-interactive context
 
         try:
             self.replay_attack_data_files(test.attack_data, test, start_time)
         except Exception as e:
 
             test.result = UnitTestResult()
             test.result.set_job_content(
                 e, self.config, duration=time.time() - start_time
             )
             self.pbar.write(
                 self.format_pbar_string(
-                    test.name,
+                    f"{detection.name}:{test.name}",
                     "\x1b[0;30;41m" + "FAIL".ljust(LONGEST_STATE) + "\x1b[0m",
                     start_time=time.time() - start_time,
                     set_pbar=False,
                 )
             )
 
             return
@@ -457,39 +457,39 @@
                 if res:
                     res = "PASS"
                 else:
                     res = "FAIL"
                 link = test.result.get_summary_dict()["sid_link"]
 
             self.format_pbar_string(
-                test.name, f"{res} - {link} (CTRL+D to continue)", start_time
+                f"{detection.name}:{test.name}", f"{res} - {link} (CTRL+D to continue)", start_time
             )
 
             try:
                 _ = input()
             except Exception as e:
                 pass
 
-        self.format_pbar_string(test.name, f"Deleting Data", start_time)
+        self.format_pbar_string(f"{detection.name}:{test.name}", f"Deleting Data", start_time)
         self.delete_attack_data(test.attack_data)
 
         if test.result is not None and test.result.success:
             self.pbar.write(
                 self.format_pbar_string(
-                    test.name,
+                    f"{detection.name}:{test.name}",
                     "\x1b[0;30;42m" + "PASS".ljust(LONGEST_STATE) + "\x1b[0m",
                     start_time,
                     set_pbar=False,
                 )
             )
 
         else:
             self.pbar.write(
                 self.format_pbar_string(
-                    test.name,
+                    f"{detection.name}:{test.name}",
                     "\x1b[0;30;41m" + "FAIL".ljust(LONGEST_STATE) + "\x1b[0m",
                     start_time,
                     set_pbar=False,
                 )
             )
 
         if test.result is not None:
@@ -521,19 +521,19 @@
 
         while time.time() < search_stop_time:
 
             for _ in range(pow(2, tick - 1)):
                 # This loop allows us to capture shutdown events without being
                 # stuck in an extended sleep. Remember that this raises an exception
                 self.check_for_teardown()
-                self.format_pbar_string(test.name, "Waiting for Processing", start_time)
+                self.format_pbar_string(f"{detection.name}:{test.name}", "Waiting for Processing", start_time)
 
                 time.sleep(1)
 
-            self.format_pbar_string(test.name, "Running Search", start_time)
+            self.format_pbar_string(f"{detection.name}:{test.name}", "Running Search", start_time)
 
             job = self.get_conn().search(query=search, **kwargs)
 
             # the following raises an error if there is an exception in the search
             _ = job.results(output_mode="json")
 
             if int(job.content.get("resultCount", "0")) > 0:
```

### Comparing `contentctl-1.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py` & `contentctl-2.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingView.py` & `contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingView.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             raise Exception("Unknown ETA")
         elif num_untested == 0:
             raise Exception("Finishing test")
 
         try:
             runtime = self.getRuntime()
             time_per_detection = runtime / num_tested
-            remaining_time = num_untested * time_per_detection
+            remaining_time = (num_untested+.5) * time_per_detection
             remaining_time -= datetime.timedelta(
                 microseconds=remaining_time.microseconds
             )
         except:
             raise Exception("Unknown ETA")
         return remaining_time
```

### Comparing `contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py` & `contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py` & `contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         folder_path.mkdir(parents=True, exist_ok=True)
 
         result_dict = self.getSummaryObject()
 
         # use the yaml writer class
         with open(output_file, "w") as res:
-            res.write(yaml.dump(result_dict))
+            res.write(yaml.safe_dump(result_dict))
 
     def showStatus(self, interval: int = 60):
         pass
 
     def showResults(self):
         pass
```

### Comparing `contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py` & `contentctl-2.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             <th>Success</th>
         </tr>
     </thead>
     <tbody>
         {% for detection in detections %}
         {% for test in detection.tests %}
         <tr>
-            <td>{{ test.name }}</td>
+            <td>{{ detection.name }}: {{ test.name }}</td>
             <td><a href="{{test.sid_link}}" target="_blank"/>SID</td>
             <td>{{ test.runDuration }}</td>
             <td>{{ test.message }}</td>
             {% if test.success %}
             <td>True</td>
             {% else %}
             <td style="font-weight: bold;background-color: #ff9999"><b>False</b></td>
@@ -88,23 +88,23 @@
                 pass
 
             def log_exception(*args, **kwargs):
                 print(f"Exception in Web View:\n\tARGS:{args}\n\t{kwargs}")
 
         self.options["handler_class"] = DontLog
         self.server = make_server(
-            "localhost", DEFAULT_WEB_UI_PORT, handler, **self.options
+            self.host, DEFAULT_WEB_UI_PORT, handler, **self.options
         )
 
         self.server.serve_forever()
 
 
 class DetectionTestingViewWeb(DetectionTestingView):
     bottleApp: Bottle = Bottle()
-    server: SimpleWebServer = SimpleWebServer()
+    server: SimpleWebServer = SimpleWebServer(host="0.0.0.0", port=DEFAULT_WEB_UI_PORT)
 
     class Config:
         arbitrary_types_allowed = True
 
     def setup(self):
         self.bottleApp.route("/", callback=self.showStatus)
         self.bottleApp.route("/status", callback=self.showStatus)
@@ -113,15 +113,15 @@
 
         t = Thread(
             target=self.bottleApp.run, daemon=True, kwargs=({"server": self.server})
         )
         t.start()
 
         try:
-            webbrowser.open(f"http://localhost:{DEFAULT_WEB_UI_PORT}")
+            webbrowser.open(f"http://{self.server.host}:{DEFAULT_WEB_UI_PORT}")
         except Exception as e:
             print(f"Could not open webbrowser for status page: {str(e)}")
 
     def stop(self):
 
         if self.server.server is None:
             print("Web Server is not running anyway - nothing to shut down")
```

### Comparing `contentctl-1.0.1/contentctl/actions/doc_gen.py` & `contentctl-2.0.0/contentctl/actions/doc_gen.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/generate.py` & `contentctl-2.0.0/contentctl/actions/generate.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,34 +19,36 @@
 class Generate:
 
     def execute(self, input_dto: GenerateInputDto) -> DirectorOutputDto:
         director_output_dto = DirectorOutputDto([],[],[],[],[],[],[],[])
         director = Director(director_output_dto)
         director.execute(input_dto.director_input_dto)
 
-        if input_dto.director_input_dto.product == SecurityContentProduct.splunk_app:
+        if input_dto.director_input_dto.product == SecurityContentProduct.SPLUNK_APP:
             conf_output = ConfOutput(input_dto.director_input_dto.input_path, input_dto.director_input_dto.config)
             conf_output.writeHeaders()
             conf_output.writeObjects(director_output_dto.detections, SecurityContentType.detections)
             conf_output.writeObjects(director_output_dto.stories, SecurityContentType.stories)
             conf_output.writeObjects(director_output_dto.baselines, SecurityContentType.baselines)
             conf_output.writeObjects(director_output_dto.investigations, SecurityContentType.investigations)
             conf_output.writeObjects(director_output_dto.lookups, SecurityContentType.lookups)
             conf_output.writeObjects(director_output_dto.macros, SecurityContentType.macros)
+            conf_output.writeAppConf()
             conf_output.packageApp()
+            conf_output.inspectApp()
 
-        elif input_dto.director_input_dto.product == SecurityContentProduct.ba_objects:
+        elif input_dto.director_input_dto.product == SecurityContentProduct.SSA:
             shutil.rmtree(input_dto.output_path + '/srs/', ignore_errors=True)
             shutil.rmtree(input_dto.output_path + '/complex/', ignore_errors=True)
             os.makedirs(input_dto.output_path + '/complex/')
             os.makedirs(input_dto.output_path + '/srs/')     
             ba_yml_output = BAYmlOutput()
             ba_yml_output.writeObjects(director_output_dto.detections, input_dto.output_path)
 
-        elif input_dto.director_input_dto.product == SecurityContentProduct.json_objects:
+        elif input_dto.director_input_dto.product == SecurityContentProduct.API:
             api_json_output = ApiJsonOutput()
             api_json_output.writeObjects(director_output_dto.detections, input_dto.output_path, SecurityContentType.detections)
             api_json_output.writeObjects(director_output_dto.stories, input_dto.output_path, SecurityContentType.stories)
             api_json_output.writeObjects(director_output_dto.baselines, input_dto.output_path, SecurityContentType.baselines)
             api_json_output.writeObjects(director_output_dto.investigations, input_dto.output_path, SecurityContentType.investigations)
             api_json_output.writeObjects(director_output_dto.lookups, input_dto.output_path, SecurityContentType.lookups)
             api_json_output.writeObjects(director_output_dto.macros, input_dto.output_path, SecurityContentType.macros)
```

### Comparing `contentctl-1.0.1/contentctl/actions/initialize_old.py` & `contentctl-2.0.0/contentctl/actions/initialize_old.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/new_content.py` & `contentctl-2.0.0/contentctl/actions/new_content.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/reporting.py` & `contentctl-2.0.0/contentctl/actions/reporting.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/test.py` & `contentctl-2.0.0/contentctl/actions/test.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/actions/validate.py` & `contentctl-2.0.0/contentctl/actions/validate.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/contentctl.py` & `contentctl-2.0.0/contentctl/contentctl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import sys
 import argparse
 import os
 
 import yaml
-
+import pathlib
 from contentctl.actions.detection_testing.GitHubService import (
     GithubService,
 )
 from contentctl.actions.validate import ValidateInputDto, Validate
 from contentctl.actions.generate import (
     GenerateInputDto,
     DirectorOutputDto,
     Generate,
 )
 from contentctl.actions.reporting import ReportingInputDto, Reporting
 from contentctl.actions.new_content import NewContentInputDto, NewContent
 from contentctl.actions.doc_gen import DocGenInputDto, DocGen
 from contentctl.actions.initialize import Initialize, InitializeInputDto
-from contentctl.actions.deploy import Deploy, DeployInputDto
+from contentctl.actions.inspect import InspectInputDto, Inspect
+from contentctl.actions.api_deploy import API_Deploy, API_DeployInputDto
+
 from contentctl.input.director import DirectorInputDto
 from contentctl.objects.enums import (
     SecurityContentType,
     SecurityContentProduct,
     DetectionTestingMode,
     PostTestBehavior,
 )
@@ -33,14 +35,15 @@
 from contentctl.objects.app import App
 from contentctl.objects.test_config import TestConfig
 from contentctl.actions.test import Test, TestInputDto, TestOutputDto
 
 
 import tqdm
 import functools
+from typing import Union
 
 
 def configure_unattended(args: argparse.Namespace) -> argparse.Namespace:
     # disable all calls to tqdm - this is so that CI/CD contexts don't
     # have a large amount of output due to progress bar updates.
     tqdm.tqdm.__init__ = functools.partialmethod(
         tqdm.tqdm.__init__, disable=args.unattended
@@ -82,130 +85,144 @@
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠉⠻⠶⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
 
     By: Splunk Threat Research Team [STRT] - research@splunk.com
     """
     )
 
 
-def start(args) -> Config:
-    return ConfigHandler.read_config(os.path.join(args.path, "contentctl.yml"))
+def start(args, read_test_file:bool = False) -> Config:
+    base_config = ConfigHandler.read_config(pathlib.Path(args.path)/"contentctl.yml")
+    if read_test_file:
+        base_config.test = ConfigHandler.read_test_config(pathlib.Path(args.path)/"contentctl_test.yml")
+    return base_config
+
 
 
-def initialize(args) -> None:
 
-    Initialize().execute(InitializeInputDto(path=os.path.abspath(args.path)))
+def initialize(args) -> None:
+    Initialize().execute(InitializeInputDto(path=pathlib.Path(args.path), demo=args.demo))
 
 
-def build(args) -> DirectorOutputDto:
-    config = start(args)
-    product_type = SecurityContentProduct.splunk_app
+def build(args, config:Union[Config,None]=None) -> DirectorOutputDto:
+    if config == None:
+        config = start(args)
+    product_type = SecurityContentProduct.SPLUNK_APP
     director_input_dto = DirectorInputDto(
         input_path=os.path.abspath(args.path), product=product_type, config=config
     )
     generate_input_dto = GenerateInputDto(director_input_dto)
 
     generate = Generate()
 
     return generate.execute(generate_input_dto)
 
 
 def inspect(args) -> None:
-    raise (Exception("WARNING - INSPECT NOT YET IMPLEMENTED"))
-    # Inspect(args)
+    config=start(args)
+    app_path = pathlib.Path(config.build.path_root)/f"{config.build.name}.tar.gz"
+    input_dto = InspectInputDto(path=app_path)
+    i = Inspect()
+    i.execute(input_dto=input_dto)
 
 
-def deploy(args) -> None:
+def api_deploy(args) -> None:
     config = start(args)
-    deploy_input_dto = DeployInputDto(path=args.path, config=config)
-    deploy = Deploy()
+    deploy_input_dto = API_DeployInputDto(path=pathlib.Path(args.path), config=config)
+    deploy = API_Deploy()
+    
     deploy.execute(deploy_input_dto)
 
+def acs_deploy(args) -> None:
+    config = start(args)
+    raise NotImplementedError("ACS Deploy is not yet implemented.")
 
 def test(args: argparse.Namespace):
     args = configure_unattended(args)
-    config = start(args)
+    config = start(args, read_test_file=True)
+    
 
     # set some arguments that are not
     # yet exposed/written properly in
     # the config file
-    test_config = TestConfig.parse_obj(
-        {
-            # "repo_path": args.path,
-            "mode": args.mode,
-            "num_containers": 1,
-            "post_test_behavior": args.behavior,
-            "detections_list": args.detections_list,
-        }
-    )
+    config.test.mode=DetectionTestingMode(args.mode) 
+    config.test.num_containers=1 
+    config.test.post_test_behavior=PostTestBehavior(args.behavior)
+    config.test.detections_list=args.detections_list
+    
+    
 
     # We do this before generating the app to save some time if options are incorrect.
     # For example, if the detection(s) we are trying to test do not exist
-    githubService = GithubService(test_config)
+    githubService = GithubService(config.test)
+
+    
+    director_output_dto = build(args, config)
 
-    director_output_dto = build(args)
+    
 
     # All this information will later come from the config, so we will
     # be able to do it in Test().execute. For now, we will do it here
     app = App(
         uid=9999,
-        appid="my_custom_app",
-        title="my_custom_app",
-        release="1.0.0",
+        appid=config.build.name,
+        title=config.build.name,
+        release=config.build.version,
         http_path=None,
-        local_path=os.path.join(
-            os.path.abspath(args.path), f"{config.build.splunk_app.path}.tar.gz"
-        ),
-        description="some description",
+        local_path=str(pathlib.Path(config.build.path_root)/f"{config.build.name}.tar.gz"),
+        description=config.build.description,
         splunkbase_path=None,
     )
 
     # We need to do this instead of appending to retrigger validation.
     # It does not happen the first time since validation does not run for default values
     # unless we use always=True in the validator
     # we always want to keep CIM as the last app installed
 
-    test_config.apps = [app] + test_config.apps
+    config.test.apps = [app] + config.test.apps
 
+    
     test_input_dto = TestInputDto(
         director_output_dto=director_output_dto,
         githubService=githubService,
-        config=test_config,
+        config=config.test,
     )
+    
     test = Test()
 
     try:
+        
         result = test.execute(test_input_dto)
         # This return code is important.  Even if testing
         # fully completes, if everything does not pass then
         # we want to return a nonzero status code
         if result:
             sys.exit(0)
         else:
             sys.exit(1)
 
     except Exception as e:
-        print("Error running contentctl test: {str(e)}")
+        print(f"Error running contentctl test: {str(e)}")
         sys.exit(1)
 
 
 def validate(args) -> None:
     config = start(args)
-    product_type = SecurityContentProduct.splunk_app
+    product_type = SecurityContentProduct.SPLUNK_APP
     director_input_dto = DirectorInputDto(
-        input_path=os.path.abspath(args.path), product=product_type, config=config
+        input_path=pathlib.Path(args.path), product=product_type, config=config
     )
     validate_input_dto = ValidateInputDto(director_input_dto=director_input_dto)
     validate = Validate()
     return validate.execute(validate_input_dto)
 
 
 def doc_gen(args) -> None:
     config = start(args)
     director_input_dto = DirectorInputDto(
-        input_path=args.path, product=SecurityContentProduct.splunk_app, config=config
+        input_path=pathlib.Path(args.path), product=SecurityContentProduct.SPLUNK_APP, config=config
     )
 
     doc_gen_input_dto = DocGenInputDto(director_input_dto=director_input_dto)
 
     doc_gen = DocGen()
     doc_gen.execute(doc_gen_input_dto)
 
@@ -227,30 +244,30 @@
     new_content = NewContent()
     new_content.execute(new_content_input_dto)
 
 
 def reporting(args) -> None:
     config = start(args)
     director_input_dto = DirectorInputDto(
-        input_path=args.path, product=SecurityContentProduct.splunk_app, config=config
+        input_path=args.path, product=SecurityContentProduct.SPLUNK_APP, config=config
     )
 
     reporting_input_dto = ReportingInputDto(director_input_dto=director_input_dto)
 
     reporting = Reporting()
     reporting.execute(reporting_input_dto)
 
 
 def main():
     """
     main function parses the arguments passed to the script and calls the respctive method.
     :param args: arguments passed by the user on command line while calling the script.
     :return: returns the output of the function called.
     """
-
+    
     # grab arguments
     parser = argparse.ArgumentParser(
         description="Use `contentctl action -h` to get help with any Splunk content action"
     )
     parser.add_argument(
         "-p",
         "--path",
@@ -281,27 +298,32 @@
     reporting_parser = actions_parser.add_parser(
         "report", help="create Splunk content report of the current pack"
     )
     inspect_parser = actions_parser.add_parser(
         "inspect",
         help="runs Splunk appinspect on a build Splunk app to ensure that an app meets Splunkbase requirements.",
     )
-    deploy_parser = actions_parser.add_parser(
-        "deploy", help="install an application on a target Splunk instance."
+    api_deploy_parser = actions_parser.add_parser(
+        "api_deploy", help="Deploy content via API to a target Splunk Instance."
     )
     docs_parser = actions_parser.add_parser(
         "docs", help="create documentation in docs folder"
     )
 
     test_parser = actions_parser.add_parser(
         "test",
         help="Run a test of the detections against a Splunk Server or Splunk Docker Container",
     )
 
     init_parser.set_defaults(func=initialize)
+    init_parser.add_argument("--demo", action=argparse.BooleanOptionalAction, 
+                             help="Use this flag to pre-populate the content pack "
+                             "with one additional detection that will fail 'contentctl validate' "
+                             "and on detection that will fail 'contentctl test'.  This is useful "
+                             "for demonstrating contentctl functionality.")
 
     validate_parser.set_defaults(func=validate)
 
     build_parser.set_defaults(func=build)
 
     docs_parser.set_defaults(func=doc_gen)
 
@@ -322,15 +344,15 @@
         required=False,
         type=str,
         default=None,
         help="path to the Splunk app to be inspected",
     )
     inspect_parser.set_defaults(func=inspect)
 
-    deploy_parser.set_defaults(func=deploy)
+    api_deploy_parser.set_defaults(func=api_deploy)
 
     test_parser.add_argument(
         "--mode",
         required=False,
         default=DetectionTestingMode.all.name,
         type=str,
         choices=DetectionTestingMode._member_names_,
@@ -360,15 +382,22 @@
         nargs="+",
         type=str,
         help="An explicit list "
         "of detections to test. Their paths should be relative to the app path.",
     )
 
     test_parser.add_argument("--unattended", action=argparse.BooleanOptionalAction)
-
+    
     test_parser.set_defaults(func=test)
 
     # parse them
     args = parser.parse_args()
 
     print_ascii_art()
-    args.func(args)
+    try:
+        args.func(args)
+    except Exception as e:
+        print(f"Error during contentctl:\n{str(e)}")
+        import traceback
+        traceback.print_exc()
+        sys.exit(1)
+
```

### Comparing `contentctl-1.0.1/contentctl/enrichments/attack_enrichment.py` & `contentctl-2.0.0/contentctl/enrichments/attack_enrichment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 
 import csv
 import os
 from posixpath import split
 from typing import Optional
 import sys
 from attackcti import attack_client
-from functools import cache
 import logging
 logging.getLogger('taxii2client').setLevel(logging.CRITICAL)
 
 
 class AttackEnrichment():
 
     @classmethod
-
-    def get_attack_lookup(self, input_path: str) -> dict:
+    def get_attack_lookup(self, input_path: str, store_csv = False, force_cached_or_offline: bool = False, skip_enrichment:bool = False) -> dict:
         print("Getting MITRE Attack Enrichment Data. This may take some time...")
         attack_lookup = dict()
         file_path = os.path.join(input_path, "lookups", "mitre_enrichment.csv")
 
+        if skip_enrichment is True:
+            print("Skipping enrichment")
+            return attack_lookup
         try:
 
+            if force_cached_or_offline is True:
+                raise(Exception("WARNING - Using cached MITRE Attack Enrichment.  Attack Enrichment may be out of date. Only use this setting for offline environments and development purposes."))
             print(f"\r{'Client'.rjust(23)}: [{0:3.0f}%]...", end="", flush=True)
             lift = attack_client()
             print(f"\r{'Client'.rjust(23)}: [{100:3.0f}%]...Done!", end="\n", flush=True)
             
             print(f"\r{'Enterprise'.rjust(23)}: [{0.0:3.0f}%]...", end="", flush=True)
             all_enterprise = lift.get_enterprise(stix_format=False)
             print(f"\r{'Enterprise'.rjust(23)}: [{100:3.0f}%]...Done!", end="\n", flush=True)
@@ -52,31 +55,32 @@
                 if ('tactic' in technique):
                     for tactic in technique['tactic']:
                         tactics.append(tactic.replace('-',' ').title())
 
                 if not ('revoked' in technique):
                     attack_lookup[technique['technique_id']] = {'technique': technique['technique'], 'tactics': tactics, 'groups': apt_groups}
 
-            f = open(file_path, 'w')
-            writer = csv.writer(f)
-            writer.writerow(['mitre_id', 'technique', 'tactics' ,'groups'])
-            for key in attack_lookup.keys():
-                if len(attack_lookup[key]['groups']) == 0:
-                    groups = 'no'
-                else:
-                    groups = '|'.join(attack_lookup[key]['groups'])
+            if store_csv:
+                f = open(file_path, 'w')
+                writer = csv.writer(f)
+                writer.writerow(['mitre_id', 'technique', 'tactics' ,'groups'])
+                for key in attack_lookup.keys():
+                    if len(attack_lookup[key]['groups']) == 0:
+                        groups = 'no'
+                    else:
+                        groups = '|'.join(attack_lookup[key]['groups'])
+                    
+                    writer.writerow([
+                        key,
+                        attack_lookup[key]['technique'],
+                        '|'.join(attack_lookup[key]['tactics']),
+                        groups
+                    ])
                 
-                writer.writerow([
-                    key,
-                    attack_lookup[key]['technique'],
-                    '|'.join(attack_lookup[key]['tactics']),
-                    groups
-                ])
-            
-            f.close()
+                f.close()
 
         except Exception as err:
             print('Warning: ' + str(err))
             print('Use local copy lookups/mitre_enrichment.csv')
             dict_from_csv = {}
             with open(file_path, mode='r') as inp:
                 reader = csv.reader(inp)
```

### Comparing `contentctl-1.0.1/contentctl/helper/config_handler.py` & `contentctl-2.0.0/contentctl/helper/config_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,48 @@
 import os
 import collections
 import sys
-
+import pathlib
 
 from contentctl.input.yml_reader import YmlReader
-from contentctl.objects.config import Config
+from contentctl.objects.config import Config, TestConfig
 
 
 class ConfigHandler:
 
     @classmethod
-    def read_config(cls, config_path: str) -> Config:
+    def read_config(cls, config_path: pathlib.Path) -> Config:
         try:
-            yml_dict = YmlReader.load_file(config_path)
+            yml_dict = YmlReader.load_file(config_path, add_fields=False)
+
         except:
             print("ERROR: no contentctl.yml found in given path")
             sys.exit(1)
 
         try: 
             config = Config.parse_obj(yml_dict)
         except Exception as e:
-            print(e)
-            sys.exit(1)
+            raise Exception(f"Error reading config file: {str(e)}")
+            
 
         return config
+    
+    @classmethod
+    def read_test_config(cls, test_config_path: pathlib.Path) -> TestConfig:
+        try:
+            yml_dict = YmlReader.load_file(test_config_path, add_fields=False)
+        except:
+            print("ERROR: no contentctl_test.yml found in given path")
+            sys.exit(1)
+
+        try: 
+            test_config = TestConfig.parse_obj(yml_dict)
+        except Exception as e:
+            raise Exception(f"Error reading test config file: {str(e)}")
+            
+
+        return test_config
+
```

### Comparing `contentctl-1.0.1/contentctl/helper/utils.py` & `contentctl-2.0.0/contentctl/helper/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,58 +3,58 @@
 import shutil
 import requests
 import random
 import string
 from timeit import default_timer
 import pathlib
 import datetime
-from typing import Union
+from typing import Union, Tuple
+from pydantic import ValidationError
 import tqdm
 from contentctl.objects.security_content_object import SecurityContentObject
 from math import ceil
 
 TOTAL_BYTES = 0
 ALWAYS_PULL = True
 
 
 class Utils:
     @staticmethod
-    def get_all_yml_files_from_directory(path: str) -> list:
-        listOfFiles = list()
+    def get_all_yml_files_from_directory(path: str) -> list[pathlib.Path]:
+        listOfFiles:list[pathlib.Path] = []
         for (dirpath, dirnames, filenames) in os.walk(path):
             for file in filenames:
                 if file.endswith(".yml"):
-                    listOfFiles.append(os.path.join(dirpath, file))
-
+                    listOfFiles.append(pathlib.Path(os.path.join(dirpath, file)))
+    
         return sorted(listOfFiles)
 
+
     @staticmethod
-    def add_id(
-        id_dict: dict[str, list[str]], obj: SecurityContentObject, path: str
-    ) -> None:
+    def add_id(id_dict:dict[str, list[pathlib.Path]], obj:SecurityContentObject, path:pathlib.Path) -> None:     
         if hasattr(obj, "id"):
             obj_id = obj.id
             if obj_id in id_dict:
                 id_dict[obj_id].append(path)
             else:
                 id_dict[obj_id] = [path]
-
     # Otherwise, no ID so nothing to add....
 
     @staticmethod
-    def check_ids_for_duplicates(id_dict: dict[str, list[str]]) -> bool:
-        validation_error = False
+    def check_ids_for_duplicates(id_dict:dict[str, list[pathlib.Path]])->list[Tuple[pathlib.Path,  ValueError]]:
+        validation_errors:list[Tuple[pathlib.Path,  ValueError]] = []
+        
         for key, values in id_dict.items():
             if len(values) > 1:
-                validation_error = True
-                id_conflicts_string = "\n\t* ".join(values)
-                print(
-                    f"\nError validating id [{key}] - duplicate ID is used for the following content: \n\t* {id_conflicts_string}"
-                )
-        return validation_error
+                error_file_path = pathlib.Path("MULTIPLE")
+                all_files = '\n\t'.join(str(pathlib.Path(p)) for p in values)
+                exception = ValueError(f"Error validating id [{key}] - duplicate ID was used in the following files: \n\t{all_files}")
+                validation_errors.append((error_file_path, exception))
+                
+        return validation_errors
 
     @staticmethod
     def validate_git_hash(
         repo_path: str, repo_url: str, commit_hash: str, branch_name: Union[str, None]
     ) -> bool:
 
         # Get a list of all branches
```

### Comparing `contentctl-1.0.1/contentctl/input/baseline_builder.py` & `contentctl-2.0.0/contentctl/input/baseline_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import sys
-
+import pathlib
 from pydantic import ValidationError
 
 from contentctl.input.yml_reader import YmlReader
 from contentctl.objects.baseline import Baseline
 from contentctl.objects.enums import SecurityContentType
 from contentctl.objects.enums import SecurityContentProduct
 
 
 class BaselineBuilder():
     baseline : Baseline
 
-    def setObject(self, path: str) -> None:
+    def setObject(self, path: pathlib.Path) -> None:
         yml_dict = YmlReader.load_file(path)
         yml_dict["tags"]["name"] = yml_dict["name"]
-
+        
         try:
             self.baseline = Baseline.parse_obj(yml_dict)
+            
         
         except ValidationError as e:
-            print('Validation Error for file ' + path)
+            print('Validation Error for file ' + str(path))
             print(e)
             sys.exit(1)
 
     def addDeployment(self, deployments: list) -> None:
         matched_deployments = []
 
         for d in deployments:
```

### Comparing `contentctl-1.0.1/contentctl/input/basic_builder.py` & `contentctl-2.0.0/contentctl/input/basic_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-
+import pathlib
 from pydantic import ValidationError
 
 from contentctl.objects.security_content_object import SecurityContentObject
 from contentctl.input.yml_reader import YmlReader
 from contentctl.objects.enums import SecurityContentType
 from contentctl.objects.deployment import Deployment
 from contentctl.objects.macro import Macro
@@ -12,46 +12,47 @@
 from contentctl.objects.unit_test import UnitTest
 
 
 class BasicBuilder():
     security_content_obj : SecurityContentObject
 
 
-    def setObject(self, path: str, type: SecurityContentType) -> None:
+    def setObject(self, path: pathlib.Path, type: SecurityContentType) -> None:
+        #print(path)
         yml_dict = YmlReader.load_file(path)
         if type == SecurityContentType.deployments:
             if "alert_action" in yml_dict:
                 alert_action_dict = yml_dict["alert_action"]
                 for key in alert_action_dict.keys():
                     yml_dict[key] = yml_dict["alert_action"][key]
             try:
                 self.security_content_obj = Deployment.parse_obj(yml_dict)
             except ValidationError as e:
-                print('Validation Error for file ' + path)
+                print('Validation Error for file ' + str(path))
                 print(e)
                 sys.exit(1)
         elif type == SecurityContentType.macros:
             try:
                 self.security_content_obj = Macro.parse_obj(yml_dict)
             except ValidationError as e:
-                print('Validation Error for file ' + path)
+                print('Validation Error for file ' + str(path))
                 print(e)
                 sys.exit(1)
         elif type == SecurityContentType.lookups:
             try:
                 self.security_content_obj = Lookup.parse_obj(yml_dict)
             except ValidationError as e:
-                print('Validation Error for file ' + path)
+                print('Validation Error for file ' + str(path))
                 print(e)
                 sys.exit(1)
         elif type == SecurityContentType.unit_tests:
             try:
                 self.security_content_obj = UnitTest.parse_obj(yml_dict)
             except ValidationError as e:
-                print('Validation Error for file ' + path)
+                print('Validation Error for file ' + str(path))
                 print(e)
                 sys.exit(1)
     
     def reset(self) -> None:
         self.security_content_obj = None
 
     def getObject(self) -> SecurityContentObject:
```

### Comparing `contentctl-1.0.1/contentctl/input/detection_builder.py` & `contentctl-2.0.0/contentctl/input/detection_builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,39 +28,43 @@
     def addDeployment(self, detection_configuration: ConfigDetectionConfiguration) -> None:
         if self.security_content_obj:
             self.security_content_obj.deployment = detection_configuration
 
 
     def addRBA(self) -> None:
         if self.security_content_obj:
+
             risk_objects = []
             risk_object_user_types = {'user', 'username', 'email address'}
             risk_object_system_types = {'device', 'endpoint', 'hostname', 'ip address'}
 
             if hasattr(self.security_content_obj.tags, 'observable') and hasattr(self.security_content_obj.tags, 'risk_score'):
                 for entity in self.security_content_obj.tags.observable:
+
                     risk_object = dict()
                     if entity['type'].lower() in risk_object_user_types:
-                        for r in entity['role']:
-                            if 'attacker' == r.lower() or 'victim' ==r.lower():
-                                risk_object['risk_object_type'] = 'user'
-                                risk_object['risk_object_field'] = entity['name']
-                                risk_object['risk_score'] = self.security_content_obj.tags.risk_score
-                                risk_objects.append(risk_object)
+                        risk_object['risk_object_type'] = 'user'
+                        risk_object['risk_object_field'] = entity['name']
+                        risk_object['risk_score'] = self.security_content_obj.tags.risk_score
+                        risk_objects.append(risk_object)
 
                     elif entity['type'].lower() in risk_object_system_types:
-                        for r in entity['role']:
-                            if 'attacker' == r.lower() or 'victim' ==r.lower():
-                                risk_object['risk_object_type'] = 'system'
-                                risk_object['risk_object_field'] = entity['name']
-                                risk_object['risk_score'] = self.security_content_obj.tags.risk_score
-                                risk_objects.append(risk_object)
-                    else:
+                        risk_object['risk_object_type'] = 'system'
+                        risk_object['risk_object_field'] = entity['name']
+                        risk_object['risk_score'] = self.security_content_obj.tags.risk_score
+                        risk_objects.append(risk_object)
+
+                    elif 'role' in entity and 'Attacker' in entity['role']:
                         risk_object['threat_object_field'] = entity['name']
                         risk_object['threat_object_type'] = entity['type'].lower()
+                        risk_objects.append(risk_object) 
+                    else:
+                        risk_object['risk_object_type'] = 'other'
+                        risk_object['risk_object_field'] = entity['name']
+                        risk_object['risk_score'] = self.security_content_obj.tags.risk_score
                         risk_objects.append(risk_object)
                         continue
 
             if self.security_content_obj.tags.risk_score >= 80:
                 self.security_content_obj.tags.risk_severity = 'high'
             elif (self.security_content_obj.tags.risk_score >= 50 and self.security_content_obj.tags.risk_score <= 79):
                 self.security_content_obj.tags.risk_severity = 'medium'
@@ -68,21 +72,20 @@
                 self.security_content_obj.tags.risk_severity = 'low'
 
             self.security_content_obj.risk = risk_objects
 
 
     def addProvidingTechnologies(self) -> None:
         if self.security_content_obj:
-            # if self.security_content_obj.tags.supported_tas:
-                if 'Endpoint' in self.security_content_obj.datamodel:
-                    self.security_content_obj.providing_technologies = ["Sysmon", "Microsoft Windows","Carbon Black Response","CrowdStrike Falcon", "Symantec Endpoint Protection"]
-                if "`cloudtrail`" in str(self.security_content_obj.search):
-                    self.security_content_obj.providing_technologies = ["Amazon Web Services - Cloudtrail"]
-                if '`wineventlog_security`' in self.security_content_obj.search or '`powershell`' in self.security_content_obj.search:
-                    self.security_content_obj.providing_technologies = ["Microsoft Windows"]
+            if 'Endpoint' in str(self.security_content_obj.search):
+                self.security_content_obj.providing_technologies = ["Sysmon", "Microsoft Windows","Carbon Black Response","CrowdStrike Falcon", "Symantec Endpoint Protection"]
+            if "`cloudtrail`" in str(self.security_content_obj.search):
+                self.security_content_obj.providing_technologies = ["Amazon Web Services - Cloudtrail"]
+            if '`wineventlog_security`' in self.security_content_obj.search or '`powershell`' in self.security_content_obj.search:
+                self.security_content_obj.providing_technologies = ["Microsoft Windows"]
 
     
     def addNesFields(self) -> None:
         if self.security_content_obj:
             if self.security_content_obj.deployment:
                 if self.security_content_obj.deployment.notable:
                     nes_fields = ",".join(list(self.security_content_obj.deployment.notable.nes_fields))
@@ -102,15 +105,15 @@
             self.security_content_obj.mappings = mappings
 
 
     def addAnnotations(self) -> None:
         if self.security_content_obj:
             annotations = {}
             annotation_keys = ['mitre_attack', 'kill_chain_phases', 'cis20', 'nist', 
-                'analytic_story', 'observable', 'context', 'impact', 'confidence', 'cve']
+                'analytic_story', 'context', 'impact', 'confidence', 'cve']
             for key in annotation_keys:
                 if key == 'mitre_attack':
                     if getattr(self.security_content_obj.tags, 'mitre_attack_id'):
                         annotations[key] = getattr(self.security_content_obj.tags, 'mitre_attack_id')
                 try:
                     if getattr(self.security_content_obj.tags, key):
                         annotations[key] = getattr(self.security_content_obj.tags, key)
@@ -140,32 +143,32 @@
                         matched_baselines.append(baseline)
 
             self.security_content_obj.baselines = matched_baselines
 
 
     def addUnitTest(self, tests: list) -> None:
         if self.security_content_obj:
-            for test in tests:
-                if test.name == f"{self.security_content_obj.name} Unit Test":
-                    self.security_content_obj.test = test
-                    return
-            if self.security_content_obj.type not in ["Correlation"] and \
+            if self.security_content_obj.tests and len(self.security_content_obj.tests) > 0: 
+                return
+            elif self.security_content_obj.type not in ["Correlation"] and \
                self.security_content_obj.deprecated == False and \
-               self.security_content_obj.experimental == False:
-                #raise(Exception(f"No tests found found {self.security_content_obj.file_path}"))
-                print(f"No tests found found {self.security_content_obj.file_path}")
+               self.security_content_obj.experimental == False and \
+               self.security_content_obj.tags.manual_test == None:
+                raise(Exception(f"No tests found found {self.security_content_obj.file_path}"))
+                #print(f"No tests found found {self.security_content_obj.file_path}")
             return None
 
 
 
     def addMitreAttackEnrichment(self, attack_enrichment: dict) -> None:
         if self.security_content_obj:
             if attack_enrichment:
                 if self.security_content_obj.tags.mitre_attack_id:
                     self.security_content_obj.tags.mitre_attack_enrichments = []
+                    
                     for mitre_attack_id in self.security_content_obj.tags.mitre_attack_id:
                         if mitre_attack_id in attack_enrichment:
                             mitre_attack_enrichment = MitreAttackEnrichment(
                                 mitre_attack_id = mitre_attack_id, 
                                 mitre_attack_technique = attack_enrichment[mitre_attack_id]["technique"], 
                                 mitre_attack_tactics = sorted(attack_enrichment[mitre_attack_id]["tactics"]), 
                                 mitre_attack_groups = sorted(attack_enrichment[mitre_attack_id]["groups"])
@@ -221,13 +224,62 @@
     def addSplunkApp(self) -> None:
         if self.security_content_obj:
             self.security_content_obj.splunk_app_enrichment = []
             if self.security_content_obj.tags.supported_tas:
                 for splunk_app in self.security_content_obj.tags.supported_tas:
                     self.security_content_obj.splunk_app_enrichment.append(SplunkAppEnrichment.enrich_splunk_app(splunk_app))
 
+    def addCIS(self) -> None:
+        if self.security_content_obj:
+            if self.security_content_obj.tags.security_domain == "network":
+                self.security_content_obj.tags.cis20 = ["CIS 13"]
+            else:
+                self.security_content_obj.tags.cis20 = ["CIS 10"]
+
+
+    def addKillChainPhase(self) -> None:
+        if self.security_content_obj:
+            if not self.security_content_obj.tags.kill_chain_phases:
+                kill_chain_phases = list()
+                if self.security_content_obj.tags.mitre_attack_enrichments:
+                    for mitre_attack_enrichment in self.security_content_obj.tags.mitre_attack_enrichments:
+                        for mitre_attack_tactic in mitre_attack_enrichment.mitre_attack_tactics:
+                            kill_chain_phases.append(ATTACK_TACTICS_KILLCHAIN_MAPPING[mitre_attack_tactic])
+                self.security_content_obj.tags.kill_chain_phases = list(dict.fromkeys(kill_chain_phases))
+
+    def addNist(self) -> None:
+        if self.security_content_obj:
+            if self.security_content_obj.type == "TTP":
+                self.security_content_obj.tags.nist = ["DE.CM"]
+            else:
+                self.security_content_obj.tags.nist = ["DE.AE"]
+
+    def addDatamodel(self) -> None:
+        if self.security_content_obj:
+            self.security_content_obj.datamodel = []
+            data_models = [
+                "Authentication", 
+                "Change", 
+                "Change_Analysis", 
+                "Email", 
+                "Endpoint", 
+                "Network_Resolution", 
+                "Network_Sessions", 
+                "Network_Traffic", 
+                "Risk", 
+                "Splunk_Audit", 
+                "UEBA", 
+                "Updates", 
+                "Vulnerabilities", 
+                "Web"
+            ]
+            for data_model in data_models:
+                if data_model in self.security_content_obj.search:
+                    self.security_content_obj.datamodel.append(data_model)
+
+
     def reset(self) -> None:
         self.security_content_obj = None
 
 
     def getObject(self) -> SecurityContentObject:
         return self.security_content_obj
```

### Comparing `contentctl-1.0.1/contentctl/input/director.py` & `contentctl-2.0.0/contentctl/input/director.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import sys
-
+import pathlib
 from dataclasses import dataclass
 from pydantic import ValidationError
 
 
 
 from contentctl.objects.detection import Detection
 from contentctl.objects.story import Story
@@ -30,15 +30,15 @@
 
 from contentctl.objects.config import Config
 
 
 
 @dataclass(frozen=True)
 class DirectorInputDto:
-    input_path: str
+    input_path: pathlib.Path
     product: SecurityContentProduct
     config: Config
 
 
 @dataclass()
 class DirectorOutputDto:
      detections: list[Detection]
@@ -68,64 +68,61 @@
         self.output_dto = output_dto
         self.attack_enrichment = dict()
 
 
     def execute(self, input_dto: DirectorInputDto) -> None:
         self.input_dto = input_dto
         
-        
         if self.input_dto.config.enrichments.attack_enrichment:
             self.attack_enrichment = AttackEnrichment.get_attack_lookup(self.input_dto.input_path)
         
         self.basic_builder = BasicBuilder()
         self.playbook_builder = PlaybookBuilder(self.input_dto.input_path)
         self.baseline_builder = BaselineBuilder()
         self.investigation_builder = InvestigationBuilder()
         self.story_builder = StoryBuilder()
         self.detection_builder = DetectionBuilder()
-
-        if self.input_dto.product == SecurityContentProduct.splunk_app or self.input_dto.product == SecurityContentProduct.json_objects:
+        if self.input_dto.product == SecurityContentProduct.SPLUNK_APP or self.input_dto.product == SecurityContentProduct.API:
             self.createSecurityContent(SecurityContentType.unit_tests)
             self.createSecurityContent(SecurityContentType.lookups)
             self.createSecurityContent(SecurityContentType.macros)
             self.createSecurityContent(SecurityContentType.baselines)
             self.createSecurityContent(SecurityContentType.investigations)
             self.createSecurityContent(SecurityContentType.playbooks)
             self.createSecurityContent(SecurityContentType.detections)
             self.createSecurityContent(SecurityContentType.stories)
-
-        elif self.input_dto.product == SecurityContentProduct.ba_objects:
+        elif self.input_dto.product == SecurityContentProduct.SSA:
             self.createSecurityContent(SecurityContentType.unit_tests)
             self.createSecurityContent(SecurityContentType.detections)
-            
+        
 
     def createSecurityContent(self, type: SecurityContentType) -> None:
         objects = []
         if type == SecurityContentType.unit_tests:
             files = Utils.get_all_yml_files_from_directory(os.path.join(self.input_dto.input_path, 'tests'))
         else:
             files = Utils.get_all_yml_files_from_directory(os.path.join(self.input_dto.input_path, str(type.name)))
 
         validation_error_found = False
                 
         already_ran = False
         progress_percent = 0
 
-        if self.input_dto.product == SecurityContentProduct.splunk_app or self.input_dto.product == SecurityContentProduct.json_objects:
-            security_content_files = [f for f in files if 'ssa___' not in f]
-        elif self.input_dto.product == SecurityContentProduct.ba_objects:
-            security_content_files = [f for f in files if 'ssa___' in f]
+        if self.input_dto.product == SecurityContentProduct.SPLUNK_APP or self.input_dto.product == SecurityContentProduct.API:
+            security_content_files = [f for f in files if not f.name.startswith('ssa___')]
+        elif self.input_dto.product == SecurityContentProduct.SSA:
+            security_content_files = [f for f in files if f.name.startswith('ssa___')]
         else:
             raise(Exception(f"Cannot createSecurityContent for unknown product '{self.input_dto.product}'"))
 
 
         for index,file in enumerate(security_content_files):
             progress_percent = ((index+1)/len(security_content_files)) * 100
             try:
-                type_string = "UNKNOWN TYPE"
+                type_string = type.name.upper()
                 if type == SecurityContentType.lookups:
                         self.constructLookup(self.basic_builder, file)
                         lookup = self.basic_builder.getObject()
                         self.output_dto.lookups.append(lookup)
                 
                 elif type == SecurityContentType.macros:
                         self.constructMacro(self.basic_builder, file)
@@ -139,32 +136,29 @@
                 
                 elif type == SecurityContentType.playbooks:
                         self.constructPlaybook(self.playbook_builder, file)
                         playbook = self.playbook_builder.getObject()
                         self.output_dto.playbooks.append(playbook)                    
                 
                 elif type == SecurityContentType.baselines:
-                        type_string = "Baselines"
                         self.constructBaseline(self.baseline_builder, file)
                         baseline = self.baseline_builder.getObject()
                         self.output_dto.baselines.append(baseline)
                 
                 elif type == SecurityContentType.investigations:
                         self.constructInvestigation(self.investigation_builder, file)
                         investigation = self.investigation_builder.getObject()
                         self.output_dto.investigations.append(investigation)
 
                 elif type == SecurityContentType.stories:
-                        type_string = "Stories"
                         self.constructStory(self.story_builder, file)
                         story = self.story_builder.getObject()
                         self.output_dto.stories.append(story)
             
                 elif type == SecurityContentType.detections:
-                        type_string = "Detections"
                         self.constructDetection(self.detection_builder, file)
                         detection = self.detection_builder.getObject()
                         self.output_dto.detections.append(detection)
             
                 elif type == SecurityContentType.unit_tests:
                         self.constructTest(self.basic_builder, file)
                         test = self.basic_builder.getObject()
@@ -174,29 +168,33 @@
                         raise Exception(f"Unsupported type: [{type}]")
                 
                 if (sys.stdout.isatty() and sys.stdin.isatty() and sys.stderr.isatty()) or not already_ran:
                         already_ran = True
                         print(f"\r{f'{type_string} Progress'.rjust(23)}: [{progress_percent:3.0f}%]...", end="", flush=True)
             
             except ValidationError as e:
-                print('\nValidation Error for file ' + file)
+                print(f"\nValidation Error for file '{file}'")
                 print(e)
                 validation_error_found = True
 
-        print(f"\r{f'{type.name} Progress'.rjust(23)}: [{progress_percent:3.0f}%]...", end="", flush=True)
+        print(f"\r{f'{type.name.upper()} Progress'.rjust(23)}: [{progress_percent:3.0f}%]...", end="", flush=True)
         print("Done!")
 
         if validation_error_found:
             sys.exit(1)
 
 
     def constructDetection(self, builder: DetectionBuilder, file_path: str) -> None:
         builder.reset()
         builder.setObject(file_path)
         builder.addDeployment(self.input_dto.config.detection_configuration)
+        builder.addKillChainPhase()
+        builder.addCIS()
+        builder.addNist()
+        builder.addDatamodel()
         builder.addRBA()
         builder.addProvidingTechnologies()
         builder.addNesFields()
         builder.addAnnotations()
         builder.addMappings()
         builder.addBaseline(self.output_dto.baselines)
         builder.addPlaybook(self.output_dto.playbooks)
@@ -222,14 +220,16 @@
         builder.addBaselines(self.output_dto.baselines)
         builder.addAuthorCompanyName()
 
 
     def constructBaseline(self, builder: BaselineBuilder, file_path: str) -> None:
         builder.reset()
         builder.setObject(file_path)
+        print("skipping deployment for baseline for now...")
+        return
         builder.addDeployment(self.output_dto.deployments)
 
 
     def constructDeployment(self, builder: BasicBuilder, file_path: str) -> None:
         builder.reset()
         builder.setObject(file_path, SecurityContentType.deployments)
```

### Comparing `contentctl-1.0.1/contentctl/input/investigation_builder.py` & `contentctl-2.0.0/contentctl/input/investigation_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/input/new_content_generator.py` & `contentctl-2.0.0/contentctl/input/new_content_generator.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/input/new_content_questions.py` & `contentctl-2.0.0/contentctl/input/new_content_questions.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/input/playbook_builder.py` & `contentctl-2.0.0/contentctl/input/playbook_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 
 import sys
 import os
-
+import pathlib
 from pydantic import ValidationError
 from pathlib import Path
 
 from contentctl.objects.playbook import Playbook
 from contentctl.input.yml_reader import YmlReader
 
 
 class PlaybookBuilder():
     playbook: Playbook
-    input_path: str
+    input_path: pathlib.Path
     
     
-    def __init__(self, input_path: str):
+    def __init__(self, input_path: pathlib.Path):
         self.input_path = input_path
 
-    def setObject(self, path: str) -> None:
+    def setObject(self, path: pathlib.Path) -> None:
         yml_dict = YmlReader.load_file(path)
 
         try:
             self.playbook = Playbook.parse_obj(yml_dict)
 
         except ValidationError as e:
-            print('Validation Error for file ' + path)
+            print('Validation Error for file ' + str(path))
             print(e)
             sys.exit(1)
 
 
     def addDetections(self) -> None:
         if self.playbook.tags.detections:
             self.playbook.tags.detection_objects = []
@@ -60,8 +60,9 @@
 
 
     def findDetectionPath(self, detection_name: str) -> str:
         for path in Path(os.path.join(self.input_path, 'detections')).rglob(self.convertNameToFileName(detection_name) + '.yml'):
             normalized_path = os.path.normpath(path)
             path_components = normalized_path.split(os.sep)
             value_index = path_components.index('detections')
-            return "/".join(path_components[value_index:])
+            return "/".join(path_components[value_index:])
+        raise Exception(f"Failed to find detection path for playbook with name '{detection_name}'")
```

### Comparing `contentctl-1.0.1/contentctl/input/story_builder.py` & `contentctl-2.0.0/contentctl/input/story_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import re
 import sys
-
+import pathlib
 from pydantic import ValidationError
 
 from contentctl.objects.story import Story
 from contentctl.objects.enums import SecurityContentType
 from contentctl.objects.config import Config
 from contentctl.input.yml_reader import YmlReader
 
 
 class StoryBuilder():
     story: Story
 
-    def setObject(self, path: str) -> None:
+    def setObject(self, path: pathlib.Path) -> None:
         yml_dict = YmlReader.load_file(path)
         yml_dict["tags"]["name"] = yml_dict["name"]
 
         try:
             self.story = Story.parse_obj(yml_dict)
         except ValidationError as e:
-            print('Validation Error for file ' + path)
+            print('Validation Error for file ' + str(path))
             print(e)
             sys.exit(1)
 
     def reset(self) -> None:
         self.story = None
 
     def getObject(self) -> Story:
@@ -37,15 +37,15 @@
         datamodels = set()
         kill_chain_phases = set()
 
         for detection in detections:
             if detection:
                 for detection_analytic_story in detection.tags.analytic_story:
                     if detection_analytic_story == self.story.name:
-                        matched_detection_names.append(str(f'{config.build.splunk_app.prefix} - ' + detection.name + ' - Rule'))
+                        matched_detection_names.append(str(f'{config.build.prefix} - ' + detection.name + ' - Rule'))
                         mitre_attack_enrichments_list = []
                         if (detection.tags.mitre_attack_enrichments):
                             for attack in detection.tags.mitre_attack_enrichments:
                                 mitre_attack_enrichments_list.append({"mitre_attack_technique": attack.mitre_attack_technique})
                         tags_obj = {"mitre_attack_enrichments": mitre_attack_enrichments_list}
                         matched_detections.append({
                             "name": detection.name,
```

### Comparing `contentctl-1.0.1/contentctl/input/yml_reader.py` & `contentctl-2.0.0/contentctl/input/yml_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from typing import Dict
 
 import yaml
 import sys
+import pathlib
 
 class YmlReader():
 
     @staticmethod
-    def load_file(file_path: str) -> Dict:
+    def load_file(file_path: pathlib.Path, add_fields=True) -> Dict:
         try:
             file_handler = open(file_path, 'r', encoding="utf-8")
             try:
                 yml_obj = list(yaml.safe_load_all(file_handler))[0]
             except yaml.YAMLError as exc:
                 print(exc)
                 sys.exit(1)
 
         except OSError as exc:
             print(exc)
             sys.exit(1)
-
-        yml_obj['file_path'] = file_path
-
-        if 'deprecated' in file_path:
+        
+        if add_fields == False:
+            return yml_obj
+        
+        yml_obj['file_path'] = str(file_path)
+        
+        if 'deprecated' in [parent.name for parent in file_path.parents]:
             yml_obj['deprecated'] = True
         else:
             yml_obj['deprecated'] = False
 
-        if 'experimental' in file_path:
+        if 'experimental' in [parent.name for parent in file_path.parents]:
             yml_obj['experimental'] = True
         else:
             yml_obj['experimental'] = False
 
         return yml_obj
```

### Comparing `contentctl-1.0.1/contentctl/objects/app.py` & `contentctl-2.0.0/contentctl/objects/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 import validators
 from contentctl.objects.security_content_object import SecurityContentObject
 from contentctl.objects.enums import DataModel
 from contentctl.helper.utils import Utils
 import yaml
 
 SPLUNKBASE_URL = "https://splunkbase.splunk.com/app/{uid}/release/{release}/download"
-
+ENVIRONMENT_PATH_NOT_SET = "ENVIRONMENT_PATH_NOT_SET"
 
 class App(BaseModel, extra=Extra.forbid):
 
     # uid is a numeric identifier assigned by splunkbase, so
     # homemade applications will not have this
     uid: Union[int, None]
 
-    # appid is basically the internal name of you app
+    # appid is basically the internal name of your app
     appid: str
 
     # Title is the human readable name for your application
     title: str
 
     # Self explanatory
     description: Union[str, None]
@@ -39,15 +39,15 @@
     http_path: Union[str, None]
     # Splunkbase path is made of the combination of uid and release fields
     splunkbase_path: Union[str, None]
 
     # Ultimate source of the app. Can be a local path or a Splunkbase Path.
     # This will be set via a function call and should not be provided in the YML
     # Note that this is the path relative to the container mount
-    environment_path: str = "ENVIRONMENT_PATH_NOT_SET"
+    environment_path: str = ENVIRONMENT_PATH_NOT_SET
 
     def configure_app_source_for_container(
         self,
         splunkbase_username: Union[str, None],
         splunkbase_password: Union[str, None],
         apps_directory: pathlib.Path,
         container_mount_path: pathlib.Path,
@@ -152,19 +152,18 @@
     def validate_splunkbase_path(cls, v, values):
         Utils.check_required_fields(
             "splunkbase_path", values, ["local_path", "http_path", "uid", "title"]
         )
 
         if v is not None:
             try:
-                res = bool(validator.url(v))
-                if res is False:
-                    raise Exception
+                if bool(validators.url(v)) == False:
+                    raise ValueError(f"splunkbase_url {v} is not a valid URL")
             except Exception as e:
-                raise (ValueError(f"splunkbase_url {v} is not a valid URL"))
+                raise (ValueError(f"Error validating the splunkbase_url: {str(e)}"))
 
             if (
                 bool(
                     re.match(
                         "^https://splunkbase\.splunk\.com/app/\d+/release/.+/download$",
                         v,
                     )
```

### Comparing `contentctl-1.0.1/contentctl/objects/baseline.py` & `contentctl-2.0.0/contentctl/objects/investigation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,67 @@
-import string
+import enum
 import uuid
+import string
+import re
 import requests
 
 from pydantic import BaseModel, validator, ValidationError
 from dataclasses import dataclass
 from datetime import datetime
 
 from contentctl.objects.security_content_object import SecurityContentObject
+from contentctl.objects.enums import AnalyticsType
 from contentctl.objects.enums import DataModel
-from contentctl.objects.baseline_tags import BaselineTags
-from contentctl.objects.deployment import Deployment
+from contentctl.objects.enums import SecurityContentType
+from contentctl.objects.investigation_tags import InvestigationTags
+from contentctl.helper.link_validator import LinkValidator
 
 
-class Baseline(BaseModel, SecurityContentObject):
-    # baseline spec
-    name: str
-    id: str
-    version: int
-    date: str
-    author: str
+class Investigation(SecurityContentObject):
+    # investigation spec
+    contentType: SecurityContentType = SecurityContentType.investigations
+    #name: str
+    #id: str
+    #version: int
+    #date: str
+    #author: str
     type: str
     datamodel: list
-    description: str
+    #description: str
     search: str
     how_to_implement: str
     known_false_positives: str
     check_references: bool = False #Validation is done in order, this field must be defined first
     references: list
-    tags: BaselineTags
+    inputs: list = None
+    tags: InvestigationTags
 
     # enrichment
-    deployment: Deployment = None
+    lowercase_name: str = None
 
-
-    @validator('name')
+    # check_fields=False because we want to override the 
+    # name validator in SecurityContentObject 
+    # (since we allow longer than the default length)
+    @validator('name',check_fields=False)
     def name_max_length(cls, v):
-        if len(v) > 67:
-            raise ValueError('name is longer then 67 chars: ' + v)
-        return v
-
-    @validator('name')
-    def name_invalid_chars(cls, v):
-        invalidChars = set(string.punctuation.replace("-", ""))
-        if any(char in invalidChars for char in v):
-            raise ValueError('invalid chars used in name: ' + v)
-        return v
-
-    @validator('id')
-    def id_check(cls, v, values):
-        try:
-            uuid.UUID(str(v))
-        except:
-            raise ValueError('uuid is not valid: ' + values["name"])
-        return v
-
-    @validator('date')
-    def date_valid(cls, v, values):
-        try:
-            datetime.strptime(v, "%Y-%m-%d")
-        except:
-            raise ValueError('date is not in format YYYY-MM-DD: ' + values["name"])
-        return v
-
-    @validator('type')
-    def type_valid(cls, v, values):
-        if v != "Baseline":
-            raise ValueError('not valid analytics type: ' + values["name"])
+        if len(v) > 75:
+            raise ValueError('name is longer then 75 chars: ' + v)
         return v
 
     @validator('datamodel')
     def datamodel_valid(cls, v, values):
         for datamodel in v:
             if datamodel not in [el.name for el in DataModel]:
                 raise ValueError('not valid data model: ' + values["name"])
         return v
 
-    @validator('description', 'how_to_implement')
+    @validator('how_to_implement')
     def encode_error(cls, v, values, field):
-        try:
-            v.encode('ascii')
-        except UnicodeEncodeError:
-            raise ValueError('encoding error in ' + field.name + ': ' + values["name"])
-        return v
-
+        return SecurityContentObject.free_text_field_valid(cls,v,values,field)
+    
+    @validator('references')
+    def references_check(cls, v, values):
+        return LinkValidator.SecurityContentObject_validate_references(v, values)
     @validator('search')
     def search_validate(cls, v, values):
         # write search validator
-        return v
+        return v
```

### Comparing `contentctl-1.0.1/contentctl/objects/baseline_tags.py` & `contentctl-2.0.0/contentctl/objects/baseline_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/objects/constants.py` & `contentctl-2.0.0/contentctl/objects/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,25 @@
 
+ATTACK_TACTICS_KILLCHAIN_MAPPING = {
+    "Reconnaissance": "Reconnaissance",
+    "Resource Development": "Weaponization",
+    "Initial Access": "Delivery",
+    "Execution": "Installation",
+    "Persistence": "Installation",
+    "Privilege Escalation": "Exploitation",
+    "Defense Evasion": "Exploitation",
+    "Credential Access": "Exploitation",
+    "Discovery": "Exploitation", 
+    "Lateral Movement": "Exploitation",
+    "Collection": "Exploitation",
+    "Command And Control": "Command And Control",
+    "Command And Control": "Command And Control",
+    "Exfiltration": "Actions on Objectives",
+    "Impact": "Actions on Objectives"
+}
 
 SES_CONTEXT_MAPPING = {
     "Unknown": 0,
     "Source:Endpoint": 10,
     "Source:AD": 11,
     "Source:Firewall": 12,
     "Source:Application Log": 13,
@@ -53,15 +70,15 @@
 SES_KILL_CHAIN_MAPPINGS = {
     "Unknown": 0,
     "Reconnaissance": 1,
     "Weaponization": 2,
     "Delivery": 3,
     "Exploitation": 4,
     "Installation": 5,
-    "Command & Control": 6,
+    "Command And Control": 6,
     "Actions on Objectives": 7
 }
 
 SES_OBSERVABLE_ROLE_MAPPING = {
     "Other": -1,
     "Unknown": 0,
     "Actor": 1,
@@ -72,27 +89,47 @@
     "Child Process": 6,
     "Known Bad": 7,
     "Data Loss": 8,
     "Observer": 9
 }
 
 SES_OBSERVABLE_TYPE_MAPPING = {
-    "Other": -1,
     "Unknown": 0,
-    "Device": 1,
-    "Container": 2,
-    "Endpoint": 3,
-    "Hostname": 4,
-    "IP Address": 5,
-    "User": 6,
-    "Username": 7,
-    "Email": 8,
-    "Email Address": 9,
-    "URL": 10,
-    "URL Domain": 11,
-    "File": 12,
-    "File Name": 13,
-    "File Hash": 14,
-    "Process": 15,
-    "Process Name": 16,
-    "Location": 17
+    "Hostname": 1,
+    "IP Address": 2,
+    "MAC Address": 3,
+    "User Name": 4,
+    "Email Address": 5,
+    "URL String": 6,
+    "File Name": 7,
+    "File Hash": 8,
+    "Process Name": 9,
+    "Ressource UID": 10,
+    "Endpoint": 20,
+    "User": 21,
+    "Email": 22,
+    "Uniform Resource Locator": 23,
+    "File": 24,
+    "Process": 25,
+    "Geo Location": 26,
+    "Container": 27,
+    "Registry Key": 28,
+    "Registry Value": 29,
+    "Other": 99
+}
+
+SES_ATTACK_TACTICS_ID_MAPPING = {
+    "Reconnaissance": "TA0043",
+    "Resource_Development": "TA0042",
+    "Initial_Access": "TA0001",
+    "Execution": "TA0002",
+    "Persistence": "TA0003",
+    "Privilege_Escalation": "TA0004",
+    "Defense_Evasion": "TA0005",
+    "Credential_Access": "TA0006",
+    "Discovery": "TA0007",
+    "Lateral_Movement": "TA0008",
+    "Collection": "TA0009",
+    "Command_and_Control": "TA0011",
+    "Exfiltration": "TA0010",
+    "Impact": "TA0040"
 }
```

### Comparing `contentctl-1.0.1/contentctl/objects/deployment.py` & `contentctl-2.0.0/contentctl/objects/deployment.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,53 +8,23 @@
 from contentctl.objects.security_content_object import SecurityContentObject
 from contentctl.objects.deployment_scheduling import DeploymentScheduling
 from contentctl.objects.deployment_email import DeploymentEmail
 from contentctl.objects.deployment_notable import DeploymentNotable
 from contentctl.objects.deployment_rba import DeploymentRBA
 from contentctl.objects.deployment_slack import DeploymentSlack
 from contentctl.objects.deployment_phantom import DeploymentPhantom
-
-class Deployment(BaseModel, SecurityContentObject):
-    name: str
-    id: str
-    date: str
-    author: str
-    description: str
+from contentctl.objects.enums import SecurityContentType
+class Deployment(SecurityContentObject):
+    name: str = "PLACEHOLDER_NAME"
+    #id: str = None
+    #date: str = None
+    #author: str = None
+    #description: str = None
+    contentType: SecurityContentType = SecurityContentType.deployments
     scheduling: DeploymentScheduling = None
     email: DeploymentEmail = None
     notable: DeploymentNotable = None
     rba: DeploymentRBA = None
     slack: DeploymentSlack = None
     phantom: DeploymentPhantom = None
-    tags: dict
-    
-
-    @validator('name')
-    def name_invalid_chars(cls, v):
-        invalidChars = set(string.punctuation.replace("-", ""))
-        if any(char in invalidChars for char in v):
-            raise ValueError('invalid chars used in name: ' + v)
-        return v
-
-    @validator('id')
-    def id_check(cls, v, values):
-        try:
-            uuid.UUID(str(v))
-        except:
-            raise ValueError('uuid is not valid: ' + values["name"])
-        return v
-
-    @validator('date')
-    def date_valid(cls, v, values):
-        try:
-            datetime.strptime(v, "%Y-%m-%d")
-        except:
-            raise ValueError('date is not in format YYYY-MM-DD: ' + values["name"])
-        return v
-
-    @validator('description')
-    def encode_error(cls, v, values, field):
-        try:
-            v.encode('ascii')
-        except UnicodeEncodeError:
-            raise ValueError('encoding error in ' + field.name + ': ' + values["name"])
-        return v
+    tags: dict = None
+
```

### Comparing `contentctl-1.0.1/contentctl/objects/detection.py` & `contentctl-2.0.0/contentctl/objects/detection.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,160 +2,139 @@
 import string
 import requests
 import time
 import sys
 
 from pydantic import BaseModel, validator, root_validator, Extra
 from dataclasses import dataclass
+from typing import Union
 from datetime import datetime, timedelta
 
 
 from contentctl.objects.security_content_object import SecurityContentObject
 from contentctl.objects.enums import AnalyticsType
 from contentctl.objects.enums import DataModel
+from contentctl.objects.enums import DetectionStatus
 from contentctl.objects.detection_tags import DetectionTags
 from contentctl.objects.config import ConfigDetectionConfiguration
 from contentctl.objects.unit_test import UnitTest
 from contentctl.objects.macro import Macro
 from contentctl.objects.lookup import Lookup
 from contentctl.objects.baseline import Baseline
 from contentctl.objects.playbook import Playbook
 from contentctl.helper.link_validator import LinkValidator
+from contentctl.objects.enums import SecurityContentType
 
 
-from typing import Union
-
-
-class Detection(BaseModel, SecurityContentObject):
+class Detection(SecurityContentObject):
     # detection spec
-    name: str
-    id: str
-    version: int
-    date: str
-    author: str
+    #name: str
+    #id: str
+    #version: int
+    #date: str
+    #author: str
+    contentType: SecurityContentType = SecurityContentType.detections
     type: str
-    datamodel: list
-    description: str
-    search: str
+    status: DetectionStatus
+    #description: str
+    data_source: list[str]
+    search: Union[str, dict]
     how_to_implement: str
     known_false_positives: str
-    check_references: bool = (
-        False  # Validation is done in order, this field must be defined first
-    )
+    check_references: bool = False  
     references: list
     tags: DetectionTags
+    tests: list[UnitTest] = []
 
     # enrichments
+    datamodel: list = None
     deprecated: bool = None
     experimental: bool = None
     deployment: ConfigDetectionConfiguration = None
     annotations: dict = None
     risk: list = None
     playbooks: list[Playbook] = None
     baselines: list[Baseline] = None
     mappings: dict = None
-    test: UnitTest = None
     macros: list[Macro] = None
     lookups: list[Lookup] = None
     cve_enrichment: list = None
     splunk_app_enrichment: list = None
     file_path: str = None
     source: str = None
     nes_fields: str = None
     providing_technologies: list = None
+    runtime: str = None
 
-    # @validator('name')
-    # def name_max_length(cls, v, values):
-    #     if len(v) > 67:
-    #         raise ValueError('name is longer then 67 chars: ' + v)
-    #     return v
-
-    @validator("name")
-    def name_invalid_chars(cls, v):
-        invalidChars = set(string.punctuation.replace("-", ""))
-        if any(char in invalidChars for char in v):
-            raise ValueError("invalid chars used in name: " + v)
-        return v
-
-    @validator("id")
-    def id_check(cls, v, values):
-        try:
-            uuid.UUID(str(v))
-        except:
-            raise ValueError("uuid is not valid: " + values["name"])
-        return v
-
-    @validator("date")
-    def date_valid(cls, v, values):
-        try:
-            datetime.strptime(v, "%Y-%m-%d")
-        except:
-            raise ValueError("date is not in format YYYY-MM-DD: " + values["name"])
-        return v
+    class Config:
+        use_enum_values = True
 
     @validator("type")
     def type_valid(cls, v, values):
         if v.lower() not in [el.name.lower() for el in AnalyticsType]:
             raise ValueError("not valid analytics type: " + values["name"])
         return v
 
-    @validator("datamodel")
-    def datamodel_valid(cls, v, values):
-        for datamodel in v:
-            if datamodel not in [el.name for el in DataModel]:
-                raise ValueError("not valid data model: " + values["name"])
-        return v
-
-    @validator("description", "how_to_implement")
+    @validator('how_to_implement')
     def encode_error(cls, v, values, field):
-        try:
-            v.encode("ascii")
-        except UnicodeEncodeError:
-            raise ValueError("encoding error in " + field.name + ": " + values["name"])
-        return v
-
-    @root_validator
-    def search_validation(cls, values):
-        if "ssa_" not in values["file_path"]:
-            if not "_filter" in values["search"]:
-                raise ValueError("filter macro missing in: " + values["name"])
-            if any(
-                x in values["search"]
-                for x in ["eventtype=", "sourcetype=", " source=", "index="]
-            ):
-                if not "index=_internal" in values["search"]:
-                    raise ValueError(
-                        "Use source macro instead of eventtype, sourcetype, source or index in detection: "
-                        + values["name"]
-                    )
-        return values
+        return SecurityContentObject.free_text_field_valid(cls,v,values,field)
 
-    @root_validator
-    def name_max_length(cls, values):
-        # Check max length only for ESCU searches, SSA does not have that constraint
-        if "ssa_" not in values["file_path"]:
-            if len(values["name"]) > 67:
-                raise ValueError("name is longer then 67 chars: " + values["name"])
-        return values
+    # @root_validator
+    # def search_validation(cls, values):
+    #     if 'ssa_' not in values['file_path']:
+    #         if not '_filter' in values['search']:
+    #             raise ValueError('filter macro missing in: ' + values["name"])
+    #         if any(x in values['search'] for x in ['eventtype=', 'sourcetype=', ' source=', 'index=']):
+    #             if not 'index=_internal' in values['search']:
+    #                 raise ValueError('Use source macro instead of eventtype, sourcetype, source or index in detection: ' + values["name"])
+    #     return values
 
     # disable it because of performance reasons
     # @validator('references')
     # def references_check(cls, v, values):
-    #     LinkValidator.check_references(v, values["name"])
+    #     return LinkValidator.check_references(v, values["name"])
     #     return v
+    
 
     @validator("search")
     def search_validate(cls, v, values):
         # write search validator
         return v
 
+    @validator("tests")
+    def tests_validate(cls, v, values):
+        if values.get("status","") != DetectionStatus.production and not v:
+            raise ValueError(
+                "tests value is needed for production detection: " + values["name"]
+            )
+        return v
+
+    @validator("experimental", always=True)
+    def experimental_validate(cls, v, values):
+        if DetectionStatus(values.get("status","")) == DetectionStatus.experimental:
+            return True
+        return False
+
+    @validator("deprecated", always=True)
+    def deprecated_validate(cls, v, values):
+        if DetectionStatus(values.get("status","")) == DetectionStatus.deprecated:
+            return True
+        return False
+    
+    @validator("datamodel")
+    def datamodel_valid(cls, v, values):
+        for datamodel in v:
+            if datamodel not in [el.name for el in DataModel]:
+                raise ValueError("not valid data model: " + values["name"])
+        return v
+    
     def all_tests_successful(self) -> bool:
-        if self.test is None or len(self.test.tests) == 0:
+        if len(self.tests) == 0:
             return False
-        for test in self.test.tests:
+        for test in self.tests:
             if test.result is None or test.result.success == False:
                 return False
         return True
 
     def get_summary(
         self,
         detection_fields: list[str] = ["name", "search"],
@@ -163,24 +142,23 @@
         test_job_fields: list[str] = ["resultCount", "runDuration"],
     ) -> dict:
         summary_dict = {}
         for field in detection_fields:
             summary_dict[field] = getattr(self, field)
         summary_dict["success"] = self.all_tests_successful()
         summary_dict["tests"] = []
-        if self.test is not None:
-            for test in self.test.tests:
-                result: dict[str, Union[str, bool]] = {"name": test.name}
-                if test.result is not None:
-                    result.update(
-                        test.result.get_summary_dict(
-                            model_fields=test_model_fields,
-                            job_fields=test_job_fields,
-                        )
+        for test in self.tests:
+            result: dict[str, Union[str, bool]] = {"name": test.name}
+            if test.result is not None:
+                result.update(
+                    test.result.get_summary_dict(
+                        model_fields=test_model_fields,
+                        job_fields=test_job_fields,
                     )
-                else:
-                    result["success"] = False
-                    result["message"] = "RESULT WAS NONE"
+                )
+            else:
+                result["success"] = False
+                result["message"] = "RESULT WAS NONE"
 
-                summary_dict["tests"].append(result)
+            summary_dict["tests"].append(result)
 
         return summary_dict
```

### Comparing `contentctl-1.0.1/contentctl/objects/detection_tags.py` & `contentctl-2.0.0/contentctl/objects/detection_tags.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,88 @@
 import re
 
-from pydantic import BaseModel, validator, ValidationError
+from pydantic import BaseModel, validator, ValidationError, root_validator
 from contentctl.objects.mitre_attack_enrichment import MitreAttackEnrichment
 from contentctl.objects.constants import *
 
 class DetectionTags(BaseModel):
     # detection spec
     name: str
     analytic_story: list
     asset_type: str
     automated_detection_testing: str = None
     cis20: list = None
     confidence: str
-    context: list
-    dataset: list = None
     impact: int
-    kill_chain_phases: list
+    kill_chain_phases: list = None
     message: str
     mitre_attack_id: list = None
     nist: list = None
     observable: list
     product: list
     required_fields: list
     risk_score: int
     security_domain: str
     risk_severity: str = None
     cve: list = None
     supported_tas: list = None
+    atomic_guid: list = None
+    drilldown_search: str = None
+    manual_test: str = None
+
 
     # enrichment
     mitre_attack_enrichments: list[MitreAttackEnrichment] = []
     confidence_id: int = None
     impact_id: int = None
     context_ids: list = None
     risk_level_id: int = None
     risk_level: str = None
     observable_str: str = None
+    evidence_str: str = None
     kill_chain_phases_id: list = None
+    research_site_url: str = None
+    event_schema: str = None
+    mappings: list = None
+    annotations: dict = None
 
 
     @validator('cis20')
     def tags_cis20(cls, v, values):
-        pattern = 'CIS [0-9]{1,2}'
+        pattern = '^CIS ([0-9]|1[0-9]|20)$' #DO NOT match leading zeroes and ensure no extra characters before or after the string
         for value in v:
             if not re.match(pattern, value):
-                raise ValueError('CIS controls are not following the pattern CIS xx: ' + values["name"])
+                raise ValueError(f"CIS control '{value}' is not a valid Control ('CIS 1' -> 'CIS 20'):  {values['name']}")
+        return v
+    
+    @validator('nist')
+    def tags_nist(cls, v, values):
+        # Sourced Courtest of NIST: https://www.nist.gov/system/files/documents/cyberframework/cybersecurity-framework-021214.pdf (Page 19)
+        IDENTIFY = [f'ID.{category}' for category in ["AM", "BE", "GV", "RA", "RM"]      ]
+        PROTECT  = [f'PR.{category}' for category in ["AC", "AT", "DS", "IP", "MA", "PT"]]
+        DETECT   = [f'DE.{category}' for category in ["AE", "CM", "DP"]                  ]
+        RESPOND  = [f'RS.{category}' for category in ["RP", "CO", "AN", "MI", "IM"]      ]
+        RECOVER  = [f'RC.{category}' for category in ["RP", "IM", "CO"]                  ]
+        ALL_NIST_CATEGORIES = IDENTIFY + PROTECT + DETECT + RESPOND + RECOVER
+
+        
+        for value in v:
+            if not value in ALL_NIST_CATEGORIES:
+                raise ValueError(f"NIST Category '{value}' is not a valid category")
         return v
 
     @validator('confidence')
     def tags_confidence(cls, v, values):
         v = int(v)
         if not (v > 0 and v <= 100):
              raise ValueError('confidence score is out of range 1-100: ' + values["name"])
         else:
             return v
 
-    @validator('context')
+    @validator('context_ids')
     def tags_context(cls, v, values):
         context_list = SES_CONTEXT_MAPPING.keys()
         for value in v:
             if value not in context_list:
                 raise ValueError('context value not valid for ' + values["name"] + '. valid options are ' + str(context_list) )
         return v
 
@@ -82,40 +105,45 @@
     def tags_mitre_attack_id(cls, v, values):
         pattern = 'T[0-9]{4}'
         for value in v:
             if not re.match(pattern, value):
                 raise ValueError('Mitre Attack ID are not following the pattern Txxxx: ' + values["name"])
         return v
 
-    @validator('observable')
-    def tags_observable(cls,v,values):
-        valid_roles = SES_OBSERVABLE_ROLE_MAPPING.keys()
-        valid_types = SES_OBSERVABLE_TYPE_MAPPING.keys()
-        
-        for value in v:
-            if value['type'] in valid_types:
-                for role in value['role']:
-                    if role not in valid_roles:
-                        raise ValueError('Observable role ' + role + ' not valid for ' + values["name"] + '. valid options are ' + str(valid_roles))
-            else:
-                raise ValueError('Observable type ' + value['type'] + ' not valid for ' + values["name"] + '. valid options are ' + str(valid_types))
-        return v
-
     @validator('product')
     def tags_product(cls, v, values):
         valid_products = [
             "Splunk Enterprise", "Splunk Enterprise Security", "Splunk Cloud",
             "Splunk Security Analytics for AWS", "Splunk Behavioral Analytics"
         ]
 
         for value in v:
             if value not in valid_products:
                 raise ValueError('product is not valid for ' + values['name'] + '. valid products are ' + str(valid_products))
         return v
 
     @validator('risk_score')
     def tags_calculate_risk_score(cls, v, values):
-        calculated_risk_score = (int(values['impact']))*(int(values['confidence']))/100
+        calculated_risk_score = round(values['impact'] * values['confidence'] / 100)
         if calculated_risk_score != int(v):
-            raise ValueError('risk_score is calculated wrong: ' + values["name"])
+            raise ValueError(f"Risk Score must be calculated as round(confidence * impact / 100)"
+                             f"\n  Expected risk_score={calculated_risk_score}, found risk_score={int(v)}: {values['name']}")
         return v
 
+    @root_validator
+    def tags_observable(cls, values):
+        valid_roles = SES_OBSERVABLE_ROLE_MAPPING.keys()
+        valid_types = SES_OBSERVABLE_TYPE_MAPPING.keys()
+        
+        for value in values["observable"]:
+            if value['type'] in valid_types:
+                if 'Splunk Behavioral Analytics' in values["product"]:
+                    continue
+
+                if 'role' not in value:
+                    raise ValueError('Observable role is missing for ' + values["name"])
+                for role in value['role']:
+                    if role not in valid_roles:
+                        raise ValueError('Observable role ' + role + ' not valid for ' + values["name"] + '. valid options are ' + str(valid_roles))
+            else:
+                raise ValueError('Observable type ' + value['type'] + ' not valid for ' + values["name"] + '. valid options are ' + str(valid_types))
+        return values
```

### Comparing `contentctl-1.0.1/contentctl/objects/investigation.py` & `contentctl-2.0.0/contentctl/objects/baseline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,63 @@
-import enum
-import uuid
 import string
-import re
+import uuid
 import requests
 
 from pydantic import BaseModel, validator, ValidationError
 from dataclasses import dataclass
 from datetime import datetime
 
 from contentctl.objects.security_content_object import SecurityContentObject
-from contentctl.objects.enums import AnalyticsType
 from contentctl.objects.enums import DataModel
-from contentctl.objects.investigation_tags import InvestigationTags
-
-
-class Investigation(BaseModel, SecurityContentObject):
-    # investigation spec
-    name: str
-    id: str
-    version: int
-    date: str
-    author: str
+from contentctl.objects.baseline_tags import BaselineTags
+from contentctl.objects.deployment import Deployment
+from contentctl.helper.link_validator import LinkValidator
+from contentctl.objects.enums import SecurityContentType
+
+class Baseline(SecurityContentObject):
+    # baseline spec
+    #name: str
+    #id: str
+    #version: int
+    #date: str
+    #author: str
+    contentType: SecurityContentType = SecurityContentType.baselines
     type: str
     datamodel: list
-    description: str
+    #description: str
     search: str
     how_to_implement: str
     known_false_positives: str
     check_references: bool = False #Validation is done in order, this field must be defined first
     references: list
-    inputs: list = None
-    tags: InvestigationTags
+    tags: BaselineTags
 
     # enrichment
-    lowercase_name: str = None
+    deployment: Deployment = None
 
 
-    @validator('name')
-    def name_max_length(cls, v):
-        if len(v) > 75:
-            raise ValueError('name is longer then 75 chars: ' + v)
-        return v
 
-    @validator('name')
-    def name_invalid_chars(cls, v):
-        invalidChars = set(string.punctuation.replace("-", ""))
-        if any(char in invalidChars for char in v):
-            raise ValueError('invalid chars used in name: ' + v)
-        return v
 
-    @validator('id')
-    def id_check(cls, v, values):
-        try:
-            uuid.UUID(str(v))
-        except:
-            raise ValueError('uuid is not valid: ' + values["name"])
-        return v
-
-    @validator('date')
-    def date_valid(cls, v, values):
-        try:
-            datetime.strptime(v, "%Y-%m-%d")
-        except:
-            raise ValueError('date is not in format YYYY-MM-DD: ' + values["name"])
+    @validator('type')
+    def type_valid(cls, v, values):
+        if v != "Baseline":
+            raise ValueError('not valid analytics type: ' + values["name"])
         return v
 
     @validator('datamodel')
     def datamodel_valid(cls, v, values):
         for datamodel in v:
             if datamodel not in [el.name for el in DataModel]:
                 raise ValueError('not valid data model: ' + values["name"])
         return v
 
-    @validator('description', 'how_to_implement')
+    @validator('how_to_implement')
     def encode_error(cls, v, values, field):
-        try:
-            v.encode('ascii')
-        except UnicodeEncodeError:
-            raise ValueError('encoding error in ' + field.name + ': ' + values["name"])
-        return v
-
+        return SecurityContentObject.free_text_field_valid(cls,v,values,field)
+        
+    # @validator('references')
+    # def references_check(cls, v, values):
+    #     return LinkValidator.SecurityContentObject_validate_references(v, values)
     @validator('search')
     def search_validate(cls, v, values):
         # write search validator
-        return v
+        return v
```

### Comparing `contentctl-1.0.1/contentctl/objects/repo_config.py` & `contentctl-2.0.0/contentctl/objects/repo_config.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/objects/story.py` & `contentctl-2.0.0/contentctl/objects/story.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,60 +3,47 @@
 import requests
 
 from pydantic import BaseModel, validator, ValidationError
 from datetime import datetime
 
 from contentctl.objects.security_content_object import SecurityContentObject
 from contentctl.objects.story_tags import StoryTags
-
-class Story(BaseModel, SecurityContentObject):
+from contentctl.helper.link_validator import LinkValidator
+from contentctl.objects.enums import SecurityContentType
+class Story(SecurityContentObject):
     # story spec
-    name: str
-    id: str
-    version: int
-    date: str
-    author: str
-    description: str
+    #name: str
+    #id: str
+    #version: int
+    #date: str
+    #author: str
+    #description: str
+    contentType: SecurityContentType = SecurityContentType.stories
     narrative: str
+    check_references: bool = False #Validation is done in order, this field must be defined first
     references: list
     tags: StoryTags
 
     # enrichments
     detection_names: list = None
     investigation_names: list = None
     baseline_names: list = None
     author_company: str = None
     author_name: str = None
     detections: list = None
     investigations: list = None
     
-    
-    @validator('name')
-    def name_invalid_chars(cls, v):
-        invalidChars = set(string.punctuation.replace("-", ""))
-        if any(char in invalidChars for char in v):
-            raise ValueError('invalid chars used in name: ' + v)
-        return v
-
-    @validator('id')
-    def id_check(cls, v, values):
-        try:
-            uuid.UUID(str(v))
-        except:
-            raise ValueError('uuid is not valid: ' + values["name"])
-        return v
 
-    @validator('date')
-    def date_valid(cls, v, values):
-        try:
-            datetime.strptime(v, "%Y-%m-%d")
-        except:
-            raise ValueError('date is not in format YYYY-MM-DD: ' + values["name"])
+    # Allow long names for macros
+    @validator('name',check_fields=False)
+    def name_max_length(cls, v):
+        #if len(v) > 67:
+        #    raise ValueError('name is longer then 67 chars: ' + v)
         return v
-
-    @validator('description', 'narrative')
+    
+    @validator('narrative')
     def encode_error(cls, v, values, field):
-        try:
-            v.encode('ascii')
-        except UnicodeEncodeError:
-            raise ValueError('encoding error in ' + field.name + ': ' + values["name"])
-        return v
+        return SecurityContentObject.free_text_field_valid(cls,v,values,field)
+
+    @validator('references')
+    def references_check(cls, v, values):
+        return LinkValidator.SecurityContentObject_validate_references(v, values)
```

### Comparing `contentctl-1.0.1/contentctl/objects/story_tags.py` & `contentctl-2.0.0/contentctl/objects/story_tags.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 
 from pydantic import BaseModel, validator, ValidationError
 from contentctl.objects.mitre_attack_enrichment import MitreAttackEnrichment
-
+from contentctl.objects.enums import StoryCategory
 
 class StoryTags(BaseModel):
     # story spec
     name: str
     analytic_story: str
-    category: list
+    category: list[StoryCategory]
     product: list
     usecase: str
 
     # enrichment
     mitre_attack_enrichments: list[MitreAttackEnrichment] = []
     mitre_attack_tactics: list = []
     datamodels: list = []
@@ -25,8 +25,14 @@
             "Splunk Enterprise", "Splunk Enterprise Security", "Splunk Cloud",
             "Splunk Security Analytics for AWS", "Splunk Behavioral Analytics"
         ]
 
         for value in v:
             if value not in valid_products:
                 raise ValueError('product is not valid for ' + values['name'] + '. valid products are ' + str(valid_products))
+        return v
+
+    @validator('category')
+    def category_validate(cls,v,values):
+        if len(v) == 0:
+            raise ValueError(f"Error for Story '{values['name']}' - at least one 'category' MUST be provided.")
         return v
```

### Comparing `contentctl-1.0.1/contentctl/objects/test_config.py` & `contentctl-2.0.0/contentctl/objects/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from contentctl.objects.enums import (
     PostTestBehavior,
     DetectionTestingMode,
     DetectionTestingTargetInfrastructure,
 )
 
-from contentctl.objects.app import App
+from contentctl.objects.app import App, ENVIRONMENT_PATH_NOT_SET
 from contentctl.helper.utils import Utils
 
 
 ALWAYS_PULL_REPO = False
 PREVIOUSLY_ALLOCATED_PORTS: set[int] = set()
 
 LOCAL_APP_DIR = pathlib.Path("apps")
@@ -42,18 +42,14 @@
 
 class TestConfig(BaseModel, extra=Extra.forbid, validate_assignment=True):
     repo_path: str = Field(default=".", title="Path to the root of your app")
     repo_url: Union[str, None] = Field(
         default=None,
         title="HTTP(s) path to the repo for repo_path.  If this field is blank, it will be inferred from the repo",
     )
-    mock: bool = Field(
-        default=False,
-        title="Whether or not to actually run the test, or just generate the app and test configuration files",
-    )
     # main_branch: Union[str,None] = Field(default=None, title="Main branch of the repo, if applicable.")
     # test_branch: Union[str,None] = Field(default=None, title="Branch of the repo to be tested, if applicable.")
     # commit_hash: Union[str,None] = Field(default=None, title="Commit hash of the repo state to be tested, if applicable")
     target_infrastructure: DetectionTestingTargetInfrastructure = Field(
         default=DetectionTestingTargetInfrastructure.container,
         title=f"Control where testing should be launched.  Choose one of {DetectionTestingTargetInfrastructure._member_names_}",
     )
@@ -103,14 +99,15 @@
         title="Domain name of IP address of Splunk server to be used for testing. Do NOT use a protocol, like http(s):// or 'localhost'",
     )
 
     hec_port: int = Field(default=8088, title="HTTP Event Collector Port")
     web_ui_port: int = Field(default=8000, title="Web UI Port")
     api_port: int = Field(default=8089, title="REST API Port")
 
+
     @validator("hec_port", "web_ui_port", "api_port", each_item=True)
     def validate_ports_range(cls, v):
         if v < 2:
             raise (
                 ValueError(
                     f"Error, invalid Port number. Port must be between 2-65535: {v}"
                 )
@@ -457,15 +454,15 @@
                     "1 of them"
                 )
             )
 
         else:
             return v
 
-    @validator("apps")
+    @validator("apps",)
     def validate_apps(cls, v, values):
         Utils.check_required_fields(
             "repo_url", values, ["splunkbase_username", "splunkbase_password"]
         )
 
         app_errors = []
 
@@ -477,14 +474,18 @@
             os.makedirs(LOCAL_APP_DIR, exist_ok=True)
         except Exception as e:
             raise (
                 Exception(f"Error: When trying to create {CONTAINER_APP_DIR}: {str(e)}")
             )
 
         for app in v:
+            if app.environment_path != ENVIRONMENT_PATH_NOT_SET:
+                #Avoid re-configuring the apps that have already been configured.
+                continue
+
             try:
                 app.configure_app_source_for_container(
                     username, password, app_directory, CONTAINER_APP_DIR
                 )
             except Exception as e:
                 error_string = f"Unable to prepare app '{app.title}': {str(e)}"
                 app_errors.append(error_string)
@@ -493,29 +494,28 @@
             error_string = "\n\t".join(app_errors)
             raise (ValueError(f"Error preparing apps to install:\n\t{error_string}"))
 
         return v
 
     @validator("target_infrastructure", always=True)
     def validate_target_infrastructure(cls, v, values):
-        if v == DetectionTestingTargetInfrastructure.server.value:
+        if v == DetectionTestingTargetInfrastructure.server:
             # No need to validate that the docker client is available
             return v
-        elif v == DetectionTestingTargetInfrastructure.container.value:
-            if values["mock"] is False:
-                # we need to make sure we can actually get the docker client from the environment
-                try:
-                    docker.client.from_env()
-                except Exception as e:
-                    raise (
-                        Exception(
-                            f"Error, failed to get docker client.  Is Docker Installed and running "
-                            f"and are docker environment variables set properly? Error:\n\t{str(e)}"
-                        )
+        elif v == DetectionTestingTargetInfrastructure.container:
+            # we need to make sure we can actually get the docker client from the environment
+            try:
+                docker.client.from_env()
+            except Exception as e:
+                raise (
+                    Exception(
+                        f"Error, failed to get docker client.  Is Docker Installed and running "
+                        f"and are docker environment variables set properly? Error:\n\t{str(e)}"
                     )
+                )
         return v
 
     @validator("test_instance_address", always=True)
     def validate_test_instance_address(cls, v, values):
         try:
             if v.startswith("http"):
                 raise (Exception("should not begin with http"))
```

### Comparing `contentctl-1.0.1/contentctl/objects/unit_test_result.py` & `contentctl-2.0.0/contentctl/objects/unit_test_result.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/objects/unit_test_test.py` & `contentctl-2.0.0/contentctl/objects/unit_test_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/api_json_output.py` & `contentctl-2.0.0/contentctl/output/api_json_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/attack_nav_output.py` & `contentctl-2.0.0/contentctl/output/attack_nav_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/attack_nav_writer.py` & `contentctl-2.0.0/contentctl/output/attack_nav_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/ba_yml_output.py` & `contentctl-2.0.0/contentctl/output/ba_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/doc_md_output.py` & `contentctl-2.0.0/contentctl/output/doc_md_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/finding_report_writer.py` & `contentctl-2.0.0/contentctl/output/finding_report_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/jinja_writer.py` & `contentctl-2.0.0/contentctl/output/jinja_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/new_content_yml_output.py` & `contentctl-2.0.0/contentctl/output/new_content_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/svg_output.py` & `contentctl-2.0.0/contentctl/output/svg_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/analyticstories_detections.j2` & `contentctl-2.0.0/contentctl/output/templates/analyticstories_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/analyticstories_stories.j2` & `contentctl-2.0.0/contentctl/output/templates/analyticstories_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/detection_count.j2` & `contentctl-2.0.0/contentctl/output/templates/detection_count.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/detection_coverage.j2` & `contentctl-2.0.0/contentctl/output/templates/detection_coverage.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/doc_detection_page.j2` & `contentctl-2.0.0/contentctl/output/templates/doc_detection_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/doc_detections.j2` & `contentctl-2.0.0/contentctl/output/templates/doc_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/doc_navigation.j2` & `contentctl-2.0.0/contentctl/output/templates/doc_navigation.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/doc_playbooks.j2` & `contentctl-2.0.0/contentctl/output/templates/doc_playbooks.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/doc_playbooks_page.j2` & `contentctl-2.0.0/contentctl/output/templates/doc_playbooks_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/doc_stories.j2` & `contentctl-2.0.0/contentctl/output/templates/doc_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/doc_story_page.j2` & `contentctl-2.0.0/contentctl/output/templates/doc_story_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/es_investigations_investigations.j2` & `contentctl-2.0.0/contentctl/output/templates/es_investigations_investigations.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/finding_report.j2` & `contentctl-2.0.0/contentctl/output/templates/finding_report.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/savedsearches_baselines.j2` & `contentctl-2.0.0/contentctl/output/templates/savedsearches_baselines.j2`

 * *Files 20% similar despite different names*

```diff
@@ -14,21 +14,19 @@
 action.{{APP_NAME|lower}}.modification_date = {{ detection.date }}
 {% if detection.tags.analytic_story is defined %}
 action.{{APP_NAME|lower}}.analytic_story = {{ detection.tags.analytic_story | tojson }}
 {% else %}
 action.{{APP_NAME|lower}}.analytic_story = []
 {% endif %}
 action.{{APP_NAME|lower}}.data_models = {{ detection.datamodel | tojson }}
-cron_schedule = {{ detection.deployment.scheduling.cron_schedule }}
+
 enableSched = 1
-dispatch.earliest_time = {{ detection.deployment.scheduling.earliest_time }}
-dispatch.latest_time = {{ detection.deployment.scheduling.latest_time }}
-{% if detection.deployment.scheduling.schedule_window is defined %}
-schedule_window = {{ detection.deployment.scheduling.schedule_window }}
-{% endif %}
+
+
+
 {% if detection.providing_technologies is defined %}
 action.{{APP_NAME|lower}}.providing_technologies = {{ detection.providing_technologies | tojson }}
 {% else %}
 action.{{APP_NAME|lower}}.providing_technologies = []
 {% endif %}
 action.{{APP_NAME|lower}}.eli5 = {{ detection.description }}
 {% if detection.how_to_implement is defined %}
```

### Comparing `contentctl-1.0.1/contentctl/output/templates/savedsearches_detections.j2` & `contentctl-2.0.0/contentctl/output/templates/savedsearches_detections.j2`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 ### {{APP_NAME}} DETECTIONS ###
 
 {% for detection in objects %}
 {% if (detection.type == 'TTP' or detection.type == 'Anomaly' or detection.type == 'Hunting' or detection.type == 'Correlation') %}
 [{{APP_NAME}} - {{ detection.name }} - Rule]
-action.escu = 0
-action.escu.enabled = 1
+action.{{APP_NAME|lower}} = 0
+action.{{APP_NAME|lower}}.enabled = 1
 {% if detection.deprecated %}
 description = WARNING, this detection has been marked deprecated by the Splunk Threat Research team, this means that it will no longer be maintained or supported. If you have any questions feel free to email us at: research@splunk.com. {{ detection.description }} 
 {% else %}
 description = {{ detection.description }}
 {% endif %}
-action.escu.mappings = {{ detection.mappings | tojson }}
-action.escu.data_models = {{ detection.datamodel | tojson }}
-action.escu.eli5 = {{ detection.description }}
+action.{{APP_NAME|lower}}.mappings = {{ detection.mappings | tojson }}
+action.{{APP_NAME|lower}}.data_models = {{ detection.datamodel | tojson }}
+action.{{APP_NAME|lower}}.eli5 = {{ detection.description }}
 {% if detection.how_to_implement is defined %}
-action.escu.how_to_implement = {{ detection.how_to_implement }}
+action.{{APP_NAME|lower}}.how_to_implement = {{ detection.how_to_implement }}
 {% else %}
-action.escu.how_to_implement = none
+action.{{APP_NAME|lower}}.how_to_implement = none
 {% endif %}
 {% if detection.known_false_positives is defined %}
-action.escu.known_false_positives = {{ detection.known_false_positives }}
+action.{{APP_NAME|lower}}.known_false_positives = {{ detection.known_false_positives }}
 {% else %}
-action.escu.known_false_positives = None
+action.{{APP_NAME|lower}}.known_false_positives = None
 {% endif %}
-action.escu.creation_date = {{ detection.date }}
-action.escu.modification_date = {{ detection.date }}
-action.escu.confidence = high
-action.escu.full_search_name = {{APP_NAME}} - {{ detection.name }} - Rule
-action.escu.search_type = detection
+action.{{APP_NAME|lower}}.creation_date = {{ detection.date }}
+action.{{APP_NAME|lower}}.modification_date = {{ detection.date }}
+action.{{APP_NAME|lower}}.confidence = high
+action.{{APP_NAME|lower}}.full_search_name = {{APP_NAME}} - {{ detection.name }} - Rule
+action.{{APP_NAME|lower}}.search_type = detection
 {% if detection.tags.product is defined %}
-action.escu.product = {{ detection.tags.product | tojson }}
+action.{{APP_NAME|lower}}.product = {{ detection.tags.product | tojson }}
 {% endif %}
 {% if detection.providing_technologies is defined %}
-action.escu.providing_technologies = {{ detection.providing_technologies | tojson }}
+action.{{APP_NAME|lower}}.providing_technologies = {{ detection.providing_technologies | tojson }}
 {% else %}
-action.escu.providing_technologies = []
+action.{{APP_NAME|lower}}.providing_technologies = []
 {% endif %}
 {% if detection.tags.analytic_story is defined %}
-action.escu.analytic_story = {{ detection.tags.analytic_story | tojson }}
+action.{{APP_NAME|lower}}.analytic_story = {{ detection.tags.analytic_story | tojson }}
 {% if detection.deployment.rba.enabled is defined %}
 action.risk = 1
 action.risk.param._risk_message = {{ detection.tags.message }}
 action.risk.param._risk = {{ detection.risk | tojson }}
 action.risk.param._risk_score = 0
 action.risk.param.verbose = 0
 {% endif %}
 {% else %}
-action.escu.analytic_story = []
+action.{{APP_NAME|lower}}.analytic_story = []
 {% endif %}
 cron_schedule = {{ detection.deployment.scheduling.cron_schedule }}
 dispatch.earliest_time = {{ detection.deployment.scheduling.earliest_time }}
 dispatch.latest_time = {{ detection.deployment.scheduling.latest_time }}
 action.correlationsearch.enabled = 1
 {% if detection.deprecated %}
 action.correlationsearch.label = {{APP_NAME}} - Deprecated - {{ detection.name }} - Rule
@@ -105,8 +105,8 @@
 quantity = 0
 realtime_schedule = 0
 is_visible = false
 search = {{ detection.search }}
 
 {% endif %}
 {% endfor %}
-### END ESCU DETECTIONS ###
+### END {{ APP_NAME }} DETECTIONS ###
```

### Comparing `contentctl-1.0.1/contentctl/output/templates/savedsearches_investigations.j2` & `contentctl-2.0.0/contentctl/output/templates/savedsearches_investigations.j2`

 * *Files 6% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 search = {{ detection.search }}
 
 {% endif %}
 {% endif %}
 {% endfor %}
 
 
-### END ESCU RESPONSE TASKS ###
+### END {{ APP_NAME }} RESPONSE TASKS ###
```

### Comparing `contentctl-1.0.1/contentctl/output/templates/transforms.j2` & `contentctl-2.0.0/contentctl/output/templates/transforms.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/output/templates/workflow_actions.j2` & `contentctl-2.0.0/contentctl/output/templates/workflow_actions.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/templates/datamodels_cim.conf` & `contentctl-2.0.0/contentctl/templates/datamodels_cim.conf`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.1/contentctl/templates/detections/anomalous_usage_of_7zip.yml` & `contentctl-2.0.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 name: Anomalous usage of 7zip
 id: 9364ee8e-a39a-11eb-8f1d-acde48001122
 version: 1
 date: '2021-04-22'
 author: Michael Haag, Teoderick Contreras, Splunk
+status: production
 type: Anomaly
-datamodel:
-- Endpoint
 description: The following detection identifies a 7z.exe spawned from `Rundll32.exe`
   or `Dllhost.exe`. It is assumed that the adversary has brought in `7z.exe` and `7z.dll`.
   It has been observed where an adversary will rename `7z.exe`. Additional coverage
   may be required to identify the behavior of renamed instances of `7z.exe`. During
   triage, identify the source of injection into `Rundll32.exe` or `Dllhost.exe`. Capture
   any files written to disk and analyze as needed. Review parallel processes for additional
   behaviors. Typically, archiving files will result in exfiltration.
+data_source:
+- Sysmon Event ID 1
 search: '| tstats `security_content_summariesonly` count min(_time) as firstTime max(_time)
   as lastTime from datamodel=Endpoint.Processes where Processes.parent_process_name
   IN ("rundll32.exe", "dllhost.exe") Processes.process_name=*7z* by Processes.dest
   Processes.user Processes.parent_process Processes.process_name Processes.process
   Processes.process_id Processes.parent_process_id | `drop_dm_object_name(Processes)`
   | `security_content_ctime(firstTime)` | `security_content_ctime(lastTime)`| `anomalous_usage_of_7zip_filter`'
 how_to_implement: To successfully implement this search you need to be ingesting information
@@ -27,23 +28,18 @@
 references:
 - https://attack.mitre.org/techniques/T1560/001/
 - https://www.microsoft.com/security/blog/2021/01/20/deep-dive-into-the-solorigate-second-stage-activation-from-sunburst-to-teardrop-and-raindrop/
 - https://thedfirreport.com/2021/01/31/bazar-no-ryuk/
 tags:
   analytic_story:
   - Cobalt Strike
+  - NOBELIUM Group
+  asset_type: Endpoint
   confidence: 80
-  context:
-  - Source:Endpoint
-  - Stage:Collection
-  dataset:
-  - https://media.githubusercontent.com/media/splunk/attack_data/master/datasets/attack_techniques/T1560.001/archive_utility/windows-sysmon.log
   impact: 80
-  kill_chain_phases:
-  - Exploitation
   message: An instance of $parent_process_name$ spawning $process_name$ was identified
     on endpoint $dest$ by user $user$. This behavior is indicative of suspicious loading
     of 7zip.
   mitre_attack_id:
   - T1560.001
   - T1560
   observable:
@@ -76,10 +72,13 @@
   - Processes.parent_process_name
   - Processes.process_name
   - Processes.parent_process
   - Processes.process_id
   - Processes.parent_process_id
   risk_score: 64
   security_domain: endpoint
-  supported_tas:
-  - Splunk_TA_microsoft_sysmon
-  asset_type: Endpoint
+tests:
+- name: True Positive Test
+  attack_data:
+  - data: https://media.githubusercontent.com/media/splunk/attack_data/master/datasets/attack_techniques/T1560.001/archive_utility/windows-sysmon.log
+    source: XmlWinEventLog:Microsoft-Windows-Sysmon/Operational
+    sourcetype: xmlwineventlog
```

### Comparing `contentctl-1.0.1/contentctl/templates/stories/cobalt_strike.yml` & `contentctl-2.0.0/contentctl/templates/stories/cobalt_strike.yml`

 * *Files 4% similar despite different names*

```diff
@@ -12,28 +12,37 @@
   scripts, malleable C2 profiles, default attack packages, and much more. For endpoint
   behavior, Cobalt Strike is most commonly identified via named pipes, spawn to processes,
   and DLL function names. Many additional variables are provided for in memory operation
   of the beacon implant. On the network, depending on the malleable C2 profile used,
   it is near infinite in the amount of ways to conceal the C2 traffic with Cobalt
   Strike. Not every query may be specific to Cobalt Strike the tool, but the methodologies
   and techniques used by it.\
+
   Splunk Threat Research reviewed all publicly available instances of Malleabe C2
   Profiles and generated a list of the most commonly used spawnto and pipenames.\
+
   `Spawnto_x86` and `spawnto_x64` is the process that Cobalt Strike will spawn and
   injects shellcode into.\
+
   Pipename sets the named pipe name used in Cobalt Strikes Beacon SMB C2 traffic.\
+
   With that, new detections were generated focused on these spawnto processes spawning
   without command line arguments. Similar, the named pipes most commonly used by Cobalt
   Strike added as a detection. In generating content for Cobalt Strike, the following
   is considered:\
+
   - Is it normal for spawnto_ value to have no command line arguments? No command
   line arguments and a network connection?\
+
   - What is the default, or normal, process lineage for spawnto_ value?\
+
   - Does the spawnto_ value make network connections?\
+
   - Is it normal for spawnto_ value to load jscript, vbscript, Amsi.dll, and clr.dll?\
+
   While investigating a detection related to this Analytic Story, keep in mind the
   parent process, process path, and any file modifications that may occur. Tuning
   may need to occur to remove any false positives.'
 references:
 - https://www.cobaltstrike.com/
 - https://www.infocyte.com/blog/2020/09/02/cobalt-strike-the-new-favorite-among-thieves/
 - https://bluescreenofjeff.com/2017-01-24-how-to-write-malleable-c2-profiles-for-cobalt-strike/
```

### Comparing `contentctl-1.0.1/pyproject.toml` & `contentctl-2.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [tool.poetry]
 name = "contentctl"
-version = "1.0.1"
+version = "2.0.0"
 description = "Splunk Content Control Tool"
 authors = ["STRT <research@splunk.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 contentctl = 'contentctl.contentctl:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = "^1.10.2"
-PyYAML = "^6.0"
+pydantic = "^1.10.11"
+PyYAML = "<6.0"
 requests = "^2.28.1"
 pycvesearch = "^1.2"
 xmltodict = "^0.13.0"
 attackcti = "^0.3.7"
 Jinja2 = "^3.1.2"
 questionary = "^1.10.0"
 gitpython = "^3.1.29"
 docker = "^6.0.1"
 splunk-sdk = "^1.7.2"
 validators = "^0.20.0"
 semantic-version = "^2.10.0"
 bottle = "^0.12.23"
 tqdm = "^4.65.0"
+splunk-appinspect = "^2.36.0"
+splunk-packaging-toolkit = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `contentctl-1.0.1/PKG-INFO` & `contentctl-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: contentctl
-Version: 1.0.1
+Version: 2.0.0
 Summary: Splunk Content Control Tool
 License: Apache 2.0
 Author: STRT
 Author-email: research@splunk.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: PyYAML (<6.0)
 Requires-Dist: attackcti (>=0.3.7,<0.4.0)
 Requires-Dist: bottle (>=0.12.23,<0.13.0)
 Requires-Dist: docker (>=6.0.1,<7.0.0)
 Requires-Dist: gitpython (>=3.1.29,<4.0.0)
 Requires-Dist: pycvesearch (>=1.2,<2.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
+Requires-Dist: splunk-appinspect (>=2.36.0,<3.0.0)
+Requires-Dist: splunk-packaging-toolkit (>=1.0.1,<2.0.0)
 Requires-Dist: splunk-sdk (>=1.7.2,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
```


# Comparing `tmp/seeq-spy-189.0.tar.gz` & `tmp/seeq-spy-189.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeq-spy-189.0.tar", last modified: Tue Jun 27 19:11:18 2023, max compression
+gzip compressed data, was "seeq-spy-189.3.tar", last modified: Thu Jul 13 17:41:44 2023, max compression
```

## Comparing `seeq-spy-189.0.tar` & `seeq-spy-189.3.tar`

### file list

```diff
@@ -1,153 +1,151 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.956932 seeq-spy-189.0/
--rw-rw-rw-   0        0        0    33551 2023-02-10 21:28:23.000000 seeq-spy-189.0/LICENSE
--rw-rw-rw-   0        0        0      207 2023-02-10 21:28:23.000000 seeq-spy-189.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4606 2023-06-27 19:11:18.955929 seeq-spy-189.0/PKG-INFO
--rw-rw-rw-   0        0        0     4091 2023-04-18 17:55:42.000000 seeq-spy-189.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.753929 seeq-spy-189.0/seeq/
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.769930 seeq-spy-189.0/seeq/base/
--rw-rw-rw-   0        0        0       36 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/base/__init__.py
--rw-rw-rw-   0        0        0      875 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/base/proputil.py
--rw-rw-rw-   0        0        0    32794 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/base/seeq_names.py
--rw-rw-rw-   0        0        0      157 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/base/system.py
--rw-rw-rw-   0        0        0     4788 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/base/util.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.771926 seeq-spy-189.0/seeq/scripts/
--rw-rw-rw-   0        0        0    12250 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/scripts/create_monitoring_alerts.py
--rw-rw-rw-   0        0        0    49636 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/scripts/create_monitoring_workbook.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.797934 seeq-spy-189.0/seeq/spy/
--rw-rw-rw-   0        0        0     1953 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/__init__.py
--rw-rw-rw-   0        0        0    32016 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_common.py
--rw-rw-rw-   0        0        0     4687 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_config.py
--rw-rw-rw-   0        0        0     4424 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_datalab.py
--rw-rw-rw-   0        0        0     9914 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_errors.py
--rw-rw-rw-   0        0        0    49041 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_login.py
--rw-rw-rw-   0        0        0    95701 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_metadata.py
--rw-rw-rw-   0        0        0     5822 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_metadata_push_results.py
--rw-rw-rw-   0        0        0     2954 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_plot.py
--rw-rw-rw-   0        0        0    55640 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_pull.py
--rw-rw-rw-   0        0        0    68835 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_push.py
--rw-rw-rw-   0        0        0     5155 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_redaction.py
--rw-rw-rw-   0        0        0    57799 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_search.py
--rw-rw-rw-   0        0        0    20456 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_session.py
--rw-rw-rw-   0        0        0    16874 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_status.py
--rw-rw-rw-   0        0        0    20657 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_swap.py
--rw-rw-rw-   0        0        0     3471 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_upgrade.py
--rw-rw-rw-   0        0        0    10707 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_url.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.802934 seeq-spy-189.0/seeq/spy/acl/
--rw-rw-rw-   0        0        0      104 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/acl/__init__.py
--rw-rw-rw-   0        0        0    12172 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/acl/_pull.py
--rw-rw-rw-   0        0        0    11351 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/acl/_push.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.809928 seeq-spy-189.0/seeq/spy/addons/
--rw-rw-rw-   0        0        0      188 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/addons/__init__.py
--rw-rw-rw-   0        0        0    26376 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/addons/_install.py
--rw-rw-rw-   0        0        0     2408 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/addons/_permissions.py
--rw-rw-rw-   0        0        0    12137 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/addons/_search.py
--rw-rw-rw-   0        0        0     5334 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/addons/_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.819933 seeq-spy-189.0/seeq/spy/assets/
--rw-rw-rw-   0        0        0      336 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/__init__.py
--rw-rw-rw-   0        0        0     3638 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_brochure.py
--rw-rw-rw-   0        0        0    12419 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_build.py
--rw-rw-rw-   0        0        0     3133 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_context.py
--rw-rw-rw-   0        0        0    48189 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_model.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.833929 seeq-spy-189.0/seeq/spy/assets/_trees/
--rw-rw-rw-   0        0        0       69 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/__init__.py
--rw-rw-rw-   0        0        0     1375 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_constants.py
--rw-rw-rw-   0        0        0     7350 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_csv.py
--rw-rw-rw-   0        0        0    22068 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_match.py
--rw-rw-rw-   0        0        0     2629 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_pandas.py
--rw-rw-rw-   0        0        0     6458 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_path.py
--rw-rw-rw-   0        0        0    23208 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_properties.py
--rw-rw-rw-   0        0        0    13479 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_pull.py
--rw-rw-rw-   0        0        0    58791 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_tree.py
--rw-rw-rw-   0        0        0     5897 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_utils.py
--rw-rw-rw-   0        0        0    25525 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_validate.py
--rw-rw-rw-   0        0        0     2538 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/brochure.html
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.835929 seeq-spy-189.0/seeq/spy/docs/
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.868929 seeq-spy-189.0/seeq/spy/docs/Documentation/
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.870927 seeq-spy-189.0/seeq/spy/docs/Documentation/Administration/
--rw-rw-rw-   0        0        0     6577 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.877929 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/
--rw-rw-rw-   0        0        0    17428 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
--rw-rw-rw-   0        0        0    33412 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
--rw-rw-rw-   0        0        0    16700 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
--rw-rw-rw-   0        0        0     8406 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
--rw-rw-rw-   0        0        0    38889 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
--rw-rw-rw-   0        0        0      870 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
--rw-rw-rw-   0        0        0   186560 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
--rw-rw-rw-   0        0        0   239024 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
--rw-rw-rw-   0        0        0   229026 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
--rw-rw-rw-   0        0        0    24627 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.892929 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/
--rw-rw-rw-   0        0        0   135771 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
--rw-rw-rw-   0        0        0   152116 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
--rw-rw-rw-   0        0        0   207271 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
--rw-rw-rw-   0        0        0      325 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/Readme.txt
--rw-rw-rw-   0        0        0   141516 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
--rw-rw-rw-   0        0        0   439966 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
--rw-rw-rw-   0        0        0   189377 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
--rw-rw-rw-   0        0        0    15177 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Command Reference.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.904927 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/
--rw-rw-rw-   0        0        0    94677 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/Example Export.zip
--rw-rw-rw-   0        0        0   111771 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
--rw-rw-rw-   0        0        0   113084 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
--rw-rw-rw-   0        0        0  1083835 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
--rw-rw-rw-   0        0        0      429 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
--rw-rw-rw-   0        0        0   674467 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Tutorial.ipynb
--rw-rw-rw-   0        0        0    11595 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Version Considerations.ipynb
--rw-rw-rw-   0        0        0  1557151 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Workbook Templates.ipynb
--rw-rw-rw-   0        0        0    54071 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.acl.ipynb
--rw-rw-rw-   0        0        0    11195 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.jobs.ipynb
--rw-rw-rw-   0        0        0    13015 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.login.ipynb
--rw-rw-rw-   0        0        0   128103 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.pull.ipynb
--rw-rw-rw-   0        0        0    99541 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.push.ipynb
--rw-rw-rw-   0        0        0    57647 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.search.ipynb
--rw-rw-rw-   0        0        0    95777 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.swap.ipynb
--rw-rw-rw-   0        0        0    10829 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.widgets.ipynb
--rw-rw-rw-   0        0        0    69828 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.workbooks.ipynb
--rw-rw-rw-   0        0        0       60 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/_copy.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.910928 seeq-spy-189.0/seeq/spy/jobs/
--rw-rw-rw-   0        0        0      491 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/jobs/__init__.py
--rw-rw-rw-   0        0        0     9869 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/jobs/_execute.py
--rw-rw-rw-   0        0        0     6111 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/jobs/_pull.py
--rw-rw-rw-   0        0        0     9398 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/jobs/_push.py
--rw-rw-rw-   0        0        0    25737 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/jobs/_schedule.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.912929 seeq-spy-189.0/seeq/spy/notifications/
--rw-rw-rw-   0        0        0      153 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/notifications/__init__.py
--rw-rw-rw-   0        0        0    11927 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/notifications/_emails.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.914936 seeq-spy-189.0/seeq/spy/utils/
--rw-rw-rw-   0        0        0     1569 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.919931 seeq-spy-189.0/seeq/spy/widgets/
--rw-rw-rw-   0        0        0      200 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/widgets/__init__.py
--rw-rw-rw-   0        0        0     4158 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/widgets/_ipy_utils.py
--rw-rw-rw-   0        0        0    30480 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/widgets/_widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.945936 seeq-spy-189.0/seeq/spy/workbooks/
--rw-rw-rw-   0        0        0     3012 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/__init__.py
--rw-rw-rw-   0        0        0    43729 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_annotation.py
--rw-rw-rw-   0        0        0    34087 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_content.py
--rw-rw-rw-   0        0        0    40974 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_data.py
--rw-rw-rw-   0        0        0     6639 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_folder.py
--rw-rw-rw-   0        0        0    14611 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_item.py
--rw-rw-rw-   0        0        0     5448 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_item_map.py
--rw-rw-rw-   0        0        0     3033 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_load.py
--rw-rw-rw-   0        0        0     3456 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_mustache.py
--rw-rw-rw-   0        0        0    14175 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_pull.py
--rw-rw-rw-   0        0        0    23095 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_push.py
--rw-rw-rw-   0        0        0     6316 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_render.py
--rw-rw-rw-   0        0        0    27127 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_report_content_utilities.py
--rw-rw-rw-   0        0        0     4729 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_save.py
--rw-rw-rw-   0        0        0    15545 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_search.py
--rw-rw-rw-   0        0        0    37445 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_template.py
--rw-rw-rw-   0        0        0    11995 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_user.py
--rw-rw-rw-   0        0        0    52462 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_workbook.py
--rw-rw-rw-   0        0        0    48819 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_worksheet.py
--rw-rw-rw-   0        0        0    51518 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_workstep.py
--rw-rw-rw-   0        0        0   427362 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/app.css
-drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.954930 seeq-spy-189.0/seeq_spy.egg-info/
--rw-rw-rw-   0        0        0     4606 2023-06-27 19:11:18.000000 seeq-spy-189.0/seeq_spy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4785 2023-06-27 19:11:18.000000 seeq-spy-189.0/seeq_spy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 19:11:18.000000 seeq-spy-189.0/seeq_spy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-26 16:53:37.000000 seeq-spy-189.0/seeq_spy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      311 2023-06-27 19:11:18.000000 seeq-spy-189.0/seeq_spy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-27 19:11:18.000000 seeq-spy-189.0/seeq_spy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 19:11:18.956932 seeq-spy-189.0/setup.cfg
--rw-rw-rw-   0        0        0     1677 2023-06-21 20:54:31.000000 seeq-spy-189.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.116257 seeq-spy-189.3/
+-rw-rw-rw-   0        0        0    33551 2023-03-28 23:18:24.000000 seeq-spy-189.3/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-03-28 23:18:24.000000 seeq-spy-189.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4606 2023-07-13 17:41:44.115257 seeq-spy-189.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4091 2023-06-21 15:08:28.000000 seeq-spy-189.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:43.961258 seeq-spy-189.3/seeq/
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:43.977256 seeq-spy-189.3/seeq/base/
+-rw-rw-rw-   0        0        0       36 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/base/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/base/proputil.py
+-rw-rw-rw-   0        0        0    33155 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/base/seeq_names.py
+-rw-rw-rw-   0        0        0      157 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/base/system.py
+-rw-rw-rw-   0        0        0     4788 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/base/util.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:43.997258 seeq-spy-189.3/seeq/spy/
+-rw-rw-rw-   0        0        0     1953 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/__init__.py
+-rw-rw-rw-   0        0        0    32021 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_common.py
+-rw-rw-rw-   0        0        0     4687 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_config.py
+-rw-rw-rw-   0        0        0     4424 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_datalab.py
+-rw-rw-rw-   0        0        0     9914 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_errors.py
+-rw-rw-rw-   0        0        0    49041 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_login.py
+-rw-rw-rw-   0        0        0    95701 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_metadata.py
+-rw-rw-rw-   0        0        0     5822 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_metadata_push_results.py
+-rw-rw-rw-   0        0        0     2954 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_plot.py
+-rw-rw-rw-   0        0        0    55646 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_pull.py
+-rw-rw-rw-   0        0        0    68835 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_push.py
+-rw-rw-rw-   0        0        0     5155 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_redaction.py
+-rw-rw-rw-   0        0        0    57799 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_search.py
+-rw-rw-rw-   0        0        0    20456 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_session.py
+-rw-rw-rw-   0        0        0    16874 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_status.py
+-rw-rw-rw-   0        0        0    20657 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_swap.py
+-rw-rw-rw-   0        0        0     3471 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_upgrade.py
+-rw-rw-rw-   0        0        0    10707 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_url.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.000257 seeq-spy-189.3/seeq/spy/acl/
+-rw-rw-rw-   0        0        0      104 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/acl/__init__.py
+-rw-rw-rw-   0        0        0    12172 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/acl/_pull.py
+-rw-rw-rw-   0        0        0    11351 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/acl/_push.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.005256 seeq-spy-189.3/seeq/spy/addons/
+-rw-rw-rw-   0        0        0      188 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/addons/__init__.py
+-rw-rw-rw-   0        0        0    26376 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/addons/_install.py
+-rw-rw-rw-   0        0        0     2408 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/addons/_permissions.py
+-rw-rw-rw-   0        0        0    12137 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/addons/_search.py
+-rw-rw-rw-   0        0        0     5334 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/addons/_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.011256 seeq-spy-189.3/seeq/spy/assets/
+-rw-rw-rw-   0        0        0      336 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/__init__.py
+-rw-rw-rw-   0        0        0     3638 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_brochure.py
+-rw-rw-rw-   0        0        0    12419 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_build.py
+-rw-rw-rw-   0        0        0     3133 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_context.py
+-rw-rw-rw-   0        0        0    48189 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_model.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.023257 seeq-spy-189.3/seeq/spy/assets/_trees/
+-rw-rw-rw-   0        0        0       69 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/__init__.py
+-rw-rw-rw-   0        0        0     1375 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_constants.py
+-rw-rw-rw-   0        0        0     7350 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_csv.py
+-rw-rw-rw-   0        0        0    22068 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_match.py
+-rw-rw-rw-   0        0        0     2629 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_pandas.py
+-rw-rw-rw-   0        0        0     6458 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_path.py
+-rw-rw-rw-   0        0        0    23208 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_properties.py
+-rw-rw-rw-   0        0        0    13479 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_pull.py
+-rw-rw-rw-   0        0        0    58791 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_tree.py
+-rw-rw-rw-   0        0        0     5897 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_utils.py
+-rw-rw-rw-   0        0        0    25525 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_validate.py
+-rw-rw-rw-   0        0        0     2538 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/brochure.html
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.025257 seeq-spy-189.3/seeq/spy/docs/
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.048256 seeq-spy-189.3/seeq/spy/docs/Documentation/
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.049259 seeq-spy-189.3/seeq/spy/docs/Documentation/Administration/
+-rw-rw-rw-   0        0        0     8501 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.056256 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/
+-rw-rw-rw-   0        0        0    17428 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
+-rw-rw-rw-   0        0        0    33412 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
+-rw-rw-rw-   0        0        0    16700 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
+-rw-rw-rw-   0        0        0     8406 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
+-rw-rw-rw-   0        0        0    38889 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
+-rw-rw-rw-   0        0        0      870 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
+-rw-rw-rw-   0        0        0   186560 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
+-rw-rw-rw-   0        0        0   239024 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
+-rw-rw-rw-   0        0        0   229026 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
+-rw-rw-rw-   0        0        0    24627 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.065256 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/
+-rw-rw-rw-   0        0        0   135771 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
+-rw-rw-rw-   0        0        0   152116 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
+-rw-rw-rw-   0        0        0   207271 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
+-rw-rw-rw-   0        0        0      325 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/Readme.txt
+-rw-rw-rw-   0        0        0   141516 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
+-rw-rw-rw-   0        0        0   439966 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
+-rw-rw-rw-   0        0        0   189377 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
+-rw-rw-rw-   0        0        0    23874 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Command Reference.ipynb
+-rw-rw-rw-   0        0        0   190416 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Data Lab Visualizations.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.072255 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/
+-rw-rw-rw-   0        0        0   100268 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/Example Export.zip
+-rw-rw-rw-   0        0        0   113732 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
+-rw-rw-rw-   0        0        0   645282 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
+-rw-rw-rw-   0        0        0  1083835 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
+-rw-rw-rw-   0        0        0      429 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
+-rw-rw-rw-   0        0        0   674658 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Tutorial.ipynb
+-rw-rw-rw-   0        0        0    11595 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Version Considerations.ipynb
+-rw-rw-rw-   0        0        0  1559074 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Workbook Templates.ipynb
+-rw-rw-rw-   0        0        0    54071 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.acl.ipynb
+-rw-rw-rw-   0        0        0    11195 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.jobs.ipynb
+-rw-rw-rw-   0        0        0    13015 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.login.ipynb
+-rw-rw-rw-   0        0        0   128103 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.pull.ipynb
+-rw-rw-rw-   0        0        0    99541 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.push.ipynb
+-rw-rw-rw-   0        0        0    57647 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.search.ipynb
+-rw-rw-rw-   0        0        0    95777 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.swap.ipynb
+-rw-rw-rw-   0        0        0    10829 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.widgets.ipynb
+-rw-rw-rw-   0        0        0    69828 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.workbooks.ipynb
+-rw-rw-rw-   0        0        0       60 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/_copy.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.077256 seeq-spy-189.3/seeq/spy/jobs/
+-rw-rw-rw-   0        0        0      491 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/jobs/__init__.py
+-rw-rw-rw-   0        0        0     9869 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/jobs/_execute.py
+-rw-rw-rw-   0        0        0     6111 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/jobs/_pull.py
+-rw-rw-rw-   0        0        0     9398 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/jobs/_push.py
+-rw-rw-rw-   0        0        0    25737 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/jobs/_schedule.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.080258 seeq-spy-189.3/seeq/spy/notifications/
+-rw-rw-rw-   0        0        0      153 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/notifications/__init__.py
+-rw-rw-rw-   0        0        0    11927 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/notifications/_emails.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.081256 seeq-spy-189.3/seeq/spy/utils/
+-rw-rw-rw-   0        0        0     1569 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.084257 seeq-spy-189.3/seeq/spy/widgets/
+-rw-rw-rw-   0        0        0      200 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4158 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/widgets/_ipy_utils.py
+-rw-rw-rw-   0        0        0    30480 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/widgets/_widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.106257 seeq-spy-189.3/seeq/spy/workbooks/
+-rw-rw-rw-   0        0        0     3012 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/__init__.py
+-rw-rw-rw-   0        0        0    43797 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_annotation.py
+-rw-rw-rw-   0        0        0    34087 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_content.py
+-rw-rw-rw-   0        0        0    40974 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_data.py
+-rw-rw-rw-   0        0        0     6639 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_folder.py
+-rw-rw-rw-   0        0        0    14611 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_item.py
+-rw-rw-rw-   0        0        0     5586 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_item_map.py
+-rw-rw-rw-   0        0        0     3033 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_load.py
+-rw-rw-rw-   0        0        0     3790 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_mustache.py
+-rw-rw-rw-   0        0        0    14175 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_pull.py
+-rw-rw-rw-   0        0        0    23108 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_push.py
+-rw-rw-rw-   0        0        0     6316 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_render.py
+-rw-rw-rw-   0        0        0    27127 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_report_content_utilities.py
+-rw-rw-rw-   0        0        0     4729 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_save.py
+-rw-rw-rw-   0        0        0    15545 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_search.py
+-rw-rw-rw-   0        0        0    38578 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_template.py
+-rw-rw-rw-   0        0        0    11995 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_user.py
+-rw-rw-rw-   0        0        0    52454 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_workbook.py
+-rw-rw-rw-   0        0        0    48919 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_worksheet.py
+-rw-rw-rw-   0        0        0    51518 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_workstep.py
+-rw-rw-rw-   0        0        0   427362 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/workbooks/app.css
+drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.114256 seeq-spy-189.3/seeq_spy.egg-info/
+-rw-rw-rw-   0        0        0     4606 2023-07-13 17:41:43.000000 seeq-spy-189.3/seeq_spy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4759 2023-07-13 17:41:43.000000 seeq-spy-189.3/seeq_spy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 17:41:43.000000 seeq-spy-189.3/seeq_spy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-10 16:46:50.000000 seeq-spy-189.3/seeq_spy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      311 2023-07-13 17:41:43.000000 seeq-spy-189.3/seeq_spy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-13 17:41:43.000000 seeq-spy-189.3/seeq_spy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 17:41:44.116257 seeq-spy-189.3/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2023-07-13 17:38:47.000000 seeq-spy-189.3/setup.py
```

### Comparing `seeq-spy-189.0/LICENSE` & `seeq-spy-189.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/PKG-INFO` & `seeq-spy-189.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 189.0
+Version: 189.3
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-189.0/README.md` & `seeq-spy-189.3/README.md`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/base/proputil.py` & `seeq-spy-189.3/seeq/base/proputil.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/base/seeq_names.py` & `seeq-spy-189.3/seeq/base/seeq_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,29 @@
         class Schemas:
             materialized_tables = 'materialized_tables'
         
     
     class MaterializedTables:
         datum_id_column = 'datum id'
         item_id_column = 'item id'
+        event_data_column = 'event data'
         context_table_prefix = 'context_'
         class Rules:
             ancestor = 'ancestor'
             concat_columns = 'concatColumns'
             event_property = 'eventProperty'
             item_property = 'itemProperty'
             path = 'path'
         
     
     class Injection:
         everyone_user_group = 'EveryoneUserGroup'
         system_state = 'SystemState'
         system_user = 'SystemUser'
+        agents_user_group = 'AgentsUserGroup'
     
     class Connectors:
         seeq_developer_name = 'Seeq'
         unknown_third_party_developer_name = 'third-party developer'
         connections_json_key = 'Connections'
         datasource_managed_json_key = 'DatasourceManaged'
         class Connections:
@@ -631,14 +633,15 @@
         sync_result = 'Sync Result'
         indexing_schedule_supported = 'Indexing Schedule Supported'
         asset_tree_search_index_needs_updating = 'Asset Tree Search Index Needs Updating'
         sync_mode = 'Sync Mode'
         items_archived_count = 'Items Archived Count'
         indexing_duration = 'Indexing Duration'
         provides_everyone_group_identities = 'Provides Everyone Group Identities'
+        datasource_labels = 'Datasource Labels'
         indexing_progress_timestamp = 'Indexing Progress Timestamp'
         asset_progress = 'Asset Progress'
         asset_count = 'Asset Count'
         previous_asset_count = 'Previous Asset Count'
         signal_progress = 'Signal Progress'
         signal_count = 'Signal Count'
         previous_signal_count = 'Previous Signal Count'
@@ -723,14 +726,17 @@
         last_login_at = 'Last Login At'
         session_duration = 'Session Duration'
         access_key_validity_duration = 'Access Key Validity Duration'
         enabled = 'Enabled'
         admin = 'Admin'
         workbench = 'Workbench'
         user_language = 'userLanguage'
+        agent_provisioning_status = 'Agent Provisioning Status'
+        agent_provisioning_source_address = 'Agent Provisioning Source Address'
+        agent_provisioning_requested_at = 'Agent Provisioning Requested At'
         remote_group_editable = 'Remote Group Editable'
         remove_permissions = 'Remove Permissions'
         data = 'Data'
         created_at = 'Created At'
         updated_at = 'Updated At'
         order = 'Order'
         removed_worksheet_workstep_relationships = 'Removed Worksheet Workstep Relationships'
```

### Comparing `seeq-spy-189.0/seeq/base/util.py` & `seeq-spy-189.3/seeq/base/util.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/__init__.py` & `seeq-spy-189.3/seeq/spy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,8 @@
 """
 
 __all__ = ['acl', 'addons', 'assets', 'docs', 'workbooks', 'widgets', 'login', 'logout', 'plot', 'pull', 'push',
            'search', 'swap', 'PATH_ROOT', 'DEFAULT_WORKBOOK_PATH', 'GLOBALS_ONLY', 'GLOBALS_AND_ALL_WORKBOOKS',
            'INHERIT_FROM_WORKBOOK', 'Session', 'Status', 'options', 'session', 'client', 'user',
            'server_version', 'jobs', 'notifications', 'upgrade', 'utils', 'errors']
 
-__version__ = '%d.%d' % (int('189'), int('0'))
+__version__ = '%d.%d' % (int('189'), int('3'))
```

### Comparing `seeq-spy-189.0/seeq/spy/_common.py` & `seeq-spy-189.3/seeq/spy/_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,18 +386,18 @@
     return datetime.datetime.now() - timer
 
 
 def convert_to_timestamp(value: Union[int, str], tz: Optional[str]) -> pd.Timestamp:
     """
     :param value: A date/time in either nanoseconds from the Unix Epoch or as ISO-8601 string (with time zone).
     :param tz: The time zone identifier to localize the value.
-    :return: The value as a localized pd.Timestamp. pd.NA and None values return as NA.
+    :return: The value as a localized pd.Timestamp. pd.NA and None values return as pd.NaT.
     """
     if pd.isna(value):
-        return pd.NA
+        return pd.NaT
     elif isinstance(value, str):
         value = pd.to_datetime(value)
     elif not isinstance(value, (int, float)):
         raise TypeError(f'Cannot convert {value} to timestamp. Expected either int or str.')
     return convert_timestamp_timezone(none_to_nan(pd.Timestamp(value)), tz)
```

### Comparing `seeq-spy-189.0/seeq/spy/_config.py` & `seeq-spy-189.3/seeq/spy/_config.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_datalab.py` & `seeq-spy-189.3/seeq/spy/_datalab.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_errors.py` & `seeq-spy-189.3/seeq/spy/_errors.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_login.py` & `seeq-spy-189.3/seeq/spy/_login.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_metadata.py` & `seeq-spy-189.3/seeq/spy/_metadata.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_metadata_push_results.py` & `seeq-spy-189.3/seeq/spy/_metadata_push_results.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_plot.py` & `seeq-spy-189.3/seeq/spy/_plot.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_pull.py` & `seeq-spy-189.3/seeq/spy/_pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -901,15 +901,15 @@
 
         check_for_dupes = False
 
         capsule_dict = {
             'Condition': item_name,
             'Capsule Start': pd_capsule_start,
             'Capsule End': pd_capsule_end,
-            'Capsule Is Uncertain': row[column_names_to_indexes['Original Uncertainty']]
+            'Capsule Is Uncertain': bool(row[column_names_to_indexes['Original Uncertainty']])
         }
 
         # capsuleSortKey divides the properties and the stat columns in returned table
         lower_bound = all_column_names.index('Capsule SortKey') + 1
         additional_columns_for_this_row = capsule_properties + all_column_names[lower_bound:]
         for column_name in additional_columns_for_this_row:
             capsule_dict[column_name] = row[column_names_to_indexes[column_name]]
```

### Comparing `seeq-spy-189.0/seeq/spy/_push.py` & `seeq-spy-189.3/seeq/spy/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_redaction.py` & `seeq-spy-189.3/seeq/spy/_redaction.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_search.py` & `seeq-spy-189.3/seeq/spy/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_session.py` & `seeq-spy-189.3/seeq/spy/_session.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_status.py` & `seeq-spy-189.3/seeq/spy/_status.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_swap.py` & `seeq-spy-189.3/seeq/spy/_swap.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_upgrade.py` & `seeq-spy-189.3/seeq/spy/_upgrade.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/_url.py` & `seeq-spy-189.3/seeq/spy/_url.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/acl/_pull.py` & `seeq-spy-189.3/seeq/spy/acl/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/acl/_push.py` & `seeq-spy-189.3/seeq/spy/acl/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/addons/_install.py` & `seeq-spy-189.3/seeq/spy/addons/_install.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/addons/_permissions.py` & `seeq-spy-189.3/seeq/spy/addons/_permissions.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/addons/_search.py` & `seeq-spy-189.3/seeq/spy/addons/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/addons/_uninstall.py` & `seeq-spy-189.3/seeq/spy/addons/_uninstall.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_brochure.py` & `seeq-spy-189.3/seeq/spy/assets/_brochure.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_build.py` & `seeq-spy-189.3/seeq/spy/assets/_build.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_context.py` & `seeq-spy-189.3/seeq/spy/assets/_context.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_model.py` & `seeq-spy-189.3/seeq/spy/assets/_model.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_trees/_constants.py` & `seeq-spy-189.3/seeq/spy/assets/_trees/_constants.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_trees/_csv.py` & `seeq-spy-189.3/seeq/spy/assets/_trees/_csv.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_trees/_match.py` & `seeq-spy-189.3/seeq/spy/assets/_trees/_match.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_trees/_pandas.py` & `seeq-spy-189.3/seeq/spy/assets/_trees/_pandas.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_trees/_path.py` & `seeq-spy-189.3/seeq/spy/assets/_trees/_path.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_trees/_properties.py` & `seeq-spy-189.3/seeq/spy/assets/_trees/_properties.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_trees/_pull.py` & `seeq-spy-189.3/seeq/spy/assets/_trees/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_trees/_tree.py` & `seeq-spy-189.3/seeq/spy/assets/_trees/_tree.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_trees/_utils.py` & `seeq-spy-189.3/seeq/spy/assets/_trees/_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/_trees/_validate.py` & `seeq-spy-189.3/seeq/spy/assets/_trees/_validate.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/assets/brochure.html` & `seeq-spy-189.3/seeq/spy/assets/brochure.html`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Command Reference.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.jobs.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9242284946236559%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '# spy.jobs\\n'), (2, 'Commands to schedule a notebook "*

 * *            "to run in the background.\\n'), (4, '**This feature is only available for scheduling "*

 * *            'notebooks in Seeq Data Lab. You cannot use SPy to schedule content in Anaconda, AWS '*

 * *            "SageMaker, or any other Python environment.**\\n')], delete: [27, 25, 23, 22, 21, 20, "*

 * *            '19, 18, 17, 16, 15, 14, 13, 12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}}, 2: '*

 * *            "{'source' […]*

```diff
@@ -1,276 +1,276 @@
 {
     "cells": [
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 3,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "# Command Reference\n",
-                "\n",
-                "The following sections provide in-depth reference for using the commands in the SPy module.\n",
-                "\n",
-                "[spy.login](spy.login.ipynb) - Logging into a Seeq Server with credentials.\n",
-                "\n",
-                "[spy.search](spy.search.ipynb) - Searching for signals, conditions and other items accessible in Seeq.\n",
-                "\n",
-                "[spy.pull](spy.pull.ipynb) - Retrieving data for a set of signals, conditions or scalars.\n",
+                "from seeq import spy\n",
+                "import pandas as pd\n",
                 "\n",
-                "[spy.push](spy.push.ipynb) - Uploading data for signals, conditions or scalars.\n",
+                "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
+                "spy.options.compatibility = 189"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# spy.jobs\n",
                 "\n",
-                "[spy.jobs](spy.jobs.ipynb) - Scheduling notebooks to run in the background within Seeq Data Lab.\n",
+                "Commands to schedule a notebook to run in the background.\n",
                 "\n",
-                "[spy.acl](spy.acl.ipynb) - Retrieving/modifying Access Control Lists on items.\n",
+                "**This feature is only available for scheduling notebooks in Seeq Data Lab. You cannot use SPy to schedule content in Anaconda, AWS SageMaker, or any other Python environment.**\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Scheduling a notebook to run in the background is achieved by adding the following command near the beginning of your notebook:\n",
                 "\n",
-                "## Asset Trees\n",
+                "```\n",
+                "spy.jobs.schedule('every 6 hours')\n",
+                "```\n",
                 "\n",
-                "Representing your assets and processes in Seeq as Asset Trees is an important task that SPy can help with.\n",
-                "The following sections walk you through the extensive functionality in this area:\n",
+                "This will cause the notebook that contains the command to run every six hours. This background execution is referred to as a _job_.\n",
                 "\n",
-                "[Asset Trees 1 - Introduction](Asset%20Trees%201%20-%20Introduction.ipynb)\n",
+                "The notebook can do anything you want, and the cell output can be inspected by going into the `_Job Results` folder that is created upon the first execution of the job."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Warning!\n",
                 "\n",
-                "[Asset Trees 2 - Templates](Asset%20Trees%202%20-%20Templates.ipynb)\n",
+                "**Scheduling jobs should be done with great care.** Jobs consume CPU, memory, and disk space resources and can easily cause degraded performance on Seeq Server, Seeq Data Lab or an external system that you may be accessing.\n",
                 "\n",
-                "[Asset Trees 3 - Report and Dashboard Templates](Asset%20Trees%203%20-%20Report%20and%20Dashboard%20Templates.ipynb)\n",
+                "If you are scheduling anything to run more frequent than every 15 minutes, you should probably discuss it with your Seeq administrator to make sure it's OK to consume those resources on a continual basis."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Example\n",
                 "\n",
-                "[Asset Trees 4 - Accelerator Templates](Asset%20Trees%204%20-%20Accelerator%20Templates.ipynb)"
+                "To try it out, execute the following cell (this cell only!). Within 15 minutes, you will find that there is a `_Job Results` folder with an HTML file in it corresponding to the output of this notebook."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Scheduled the notebook <strong>SPy Documentation/spy.jobs.ipynb</strong> successfully.<br>Current context is <strong>INTERACTIVE</strong>.</div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE;\">Schedule</td><td style=\"background-color: #EEFFEE;\">Scheduled</td><td style=\"background-color: #EEFFEE;\">Next Run</td></tr><tr style=\"background-color: #EEFFEE;\"><td>0</td><td>every 15 minutes</td><td>Every 15 minutes</td><td>2021-01-30 11:30:00 PST</td></tr></table>"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>Schedule</th>\n",
+                            "      <th>Scheduled</th>\n",
+                            "      <th>Next Run</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>every 15 minutes</td>\n",
+                            "      <td>Every 15 minutes</td>\n",
+                            "      <td>2021-01-30 11:30:00 PST</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "           Schedule         Scheduled                 Next Run\n",
+                            "0  every 15 minutes  Every 15 minutes  2021-01-30 11:30:00 PST"
+                        ]
+                    },
+                    "execution_count": 3,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "spy.jobs.schedule('every 15 minutes')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Properties stored in the output DataFrame\n",
-                "Many SPy functions return a DataFrame, and that DataFrame often has a special `spy` attribute on it that includes\n",
-                "information about the provenance of the DataFrame.\n",
-                "\n",
-                "For example, if you assigned the results of `spy.search()` to a variable you can use the `spy` attribute to\n",
-                "access the following properties of the original search:\n",
-                "\n",
-                "Property         |   Description\n",
-                "-----------------|---------------------------------------------------------------------------------------------------\n",
-                "func             |   A str value of 'spy.search'\n",
-                "kwargs           |   A dict with the values of the input parameters passed to spy.search to get the output DataFrame \n",
-                "status           |   A spy.Status object with the status of the spy.search call\n",
+                "The following line will cause the job to be unscheduled after the first time it runs, which is what we want for the purposes of this tutorial. We don't want to consume resources unnecessarily!\n",
                 "\n",
-                "You can discover which properties are returned for a particular call by printing the detailed help (see below)."
+                "You would omit this line in \"real\" scenarios, since you want the job to run more than once."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "spy.jobs.unschedule()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "If you would like to schedule multiple jobs and parameterize them, check out the [Parameterized Jobs](Advanced%20Scheduling/Parameterized%20Jobs.ipynb) example."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Below the scheduling command, you can add whatever code you would like. In this example, we will perform a trivial computation and push that into a Seeq Workbook Analysis."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pull_df = spy.pull(spy.search({'Name': 'Area A_Temperature', 'Datasource Name': 'Example Data'}))\n",
+                "pull_df['Scheduling Example'] = pull_df['Area A_Temperature'].apply(lambda value: value + 10)\n",
+                "pull_df.drop(columns=['Area A_Temperature'], inplace=True)\n",
+                "spy.push(pull_df)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Detailed Help"
+                "When you're working on debugging or improving your notebook, sometimes it's convenient to prevent jobs for the notebook from executing in the background. You can add the `suspend=True` argument to your `spy.jobs.schedule()` command to achieve that, and then you can remove the flag and execute the cell again to restart the job schedule."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In addition to the documentation notebooks mentioned in **Command Reference** above, all SPy functions \n",
-                "include detailed help that you can access via Python's built-in `help()` function like so:"
+                "## Detailed Help\n",
+                "\n",
+                "All SPy functions have detailed documentation to help you use them. Just execute `help(spy.<func>)` like\n",
+                "you see below.\n",
+                "\n",
+                "**Make sure you re-execute the cell below to see the latest documentation. It otherwise might be from an\n",
+                "earlier version of SPy.**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Help on function search in module seeq.spy._search:\n",
+                        "Help on function schedule in module seeq.spy.jobs._schedule:\n",
                         "\n",
-                        "search(query, *, all_properties=False, workbook='Data Lab >> Data Lab Analysis', recursive=True, ignore_unindexed_properties=True, include_archived=False, estimate_sample_period=None, order_by=None, quiet=False, status=None, session: Union[seeq.spy._session.Session, NoneType] = None)\n",
-                        "    Issues a query to the Seeq Server to retrieve metadata for signals,\n",
-                        "    conditions, scalars and assets. This metadata can be used to retrieve\n",
-                        "    samples, capsules for a particular time range.\n",
+                        "schedule(schedule_spec: str = None, datalab_notebook_url: str = None, user: str = None, suspend: bool = False, quiet: bool = False, status: seeq.spy._common.Status = None)\n",
+                        "    Schedules the automatic execution of a Seeq Data Lab notebook.\n",
                         "    \n",
-                        "    Parameters\n",
-                        "    ----------\n",
-                        "    query : {str, dict, list, pd.DataFrame, pd.Series}\n",
-                        "        A mapping of property / match-criteria pairs or a Seeq Workbench URL\n",
+                        "    The current notebook is scheduled for execution unless datalab_notebook_url\n",
+                        "    is supplied. Scheduling can be done by user with admin privileges on behalf\n",
+                        "    of another user.\n",
                         "    \n",
-                        "        If you supply a dict or list of dicts, then the matching\n",
-                        "        operations are \"contains\" (instead of \"equal to\").\n",
+                        "    Successive calls to 'schedule()' for the same notebook but with different\n",
+                        "    schedules will update the schedule of that notebook.\n",
                         "    \n",
-                        "        If you supply a DataFrame or a Series, then the matching\n",
-                        "        operations are \"equal to\" (instead of \"contains\").\n",
+                        "    Removing the scheduling is accomplished via unschedule().\n",
+                        "    \n",
+                        "    Parameters\n",
+                        "    ----------\n",
+                        "    schedule_spec : str\n",
+                        "        A string that represents the frequency with which the notebook should\n",
+                        "        execute.\n",
+                        "    \n",
+                        "        Examples: 'every 15 minutes'\n",
+                        "                  'every tuesday and friday at 6am'\n",
+                        "                  'every fifth of the month'\n",
+                        "    \n",
+                        "        The timezone used for scheduling is the one specified in the logged-in\n",
+                        "        user's profile.\n",
+                        "    \n",
+                        "        You can also use Quartz Cron syntax. Use the following site to\n",
+                        "        construct it:\n",
+                        "        https://www.freeformatter.com/cron-expression-generator-quartz.html\n",
+                        "    \n",
+                        "    datalab_notebook_url : str, default None\n",
+                        "        A datalab notebook URL. If the value is not specified the currently\n",
+                        "        running notebook URL is used.\n",
+                        "    \n",
+                        "    user : str, default None\n",
+                        "        Determines the user on whose behalf the notebook is executed. If the\n",
+                        "        value is not specified the currently logged in user is used. The can be\n",
+                        "        specified as username or a user's Seeq ID.\n",
+                        "    \n",
+                        "    suspend : bool default False\n",
+                        "        If True, unschedules all jobs for the specified notebook. This is used\n",
+                        "        in scenarios where you wish to work with a notebook interactively and\n",
+                        "        temporarily \"pause\" job execution. Remove the argument (or change it\n",
+                        "        to False) when you are ready to resume job execution.\n",
                         "    \n",
-                        "        If you supply a str, it must be the URL of a Seeq Workbench worksheet.\n",
-                        "        The retrieved metadata will be the signals, conditions and scalars\n",
-                        "        currently present on the Details Panel.\n",
-                        "    \n",
-                        "        'Name' and 'Description' fields support wildcard and regular expression\n",
-                        "        (regex) matching with the same syntax as within the Data tab in Seeq\n",
-                        "        Workbench.\n",
-                        "    \n",
-                        "        The 'Path' field allows you to query within an asset tree, where >>\n",
-                        "        separates each level from the next. E.g.: 'Path': 'Example >> Cooling*'\n",
-                        "        You can use wildcard and regular expression matching at any level but,\n",
-                        "        unlike the Name/Description fields, the match must be a \"full match\",\n",
-                        "        meaning that 'Path': 'Example' will match on a root asset tree node of\n",
-                        "        'Example' but not 'Example (AF)'.\n",
-                        "    \n",
-                        "        Available options are:\n",
-                        "    \n",
-                        "        =================== ===================================================\n",
-                        "        Property            Description\n",
-                        "        =================== ===================================================\n",
-                        "        Name                Name of the item (wildcards/regex supported)\n",
-                        "        Path                Asset tree path of the item (should not include the\n",
-                        "                            \"leaf\" asset), using ' >> ' hierarchy delimiters\n",
-                        "        Asset               Asset name (i.e., the name of the leaf asset) or ID\n",
-                        "        Type                The item type. One of 'Signal', 'Condition',\n",
-                        "                              'Scalar', 'Asset', 'Chart', 'Metric', 'Workbook',\n",
-                        "                              and 'Worksheet'\n",
-                        "        Description         Description of the item (wildcards/regex supported)\n",
-                        "        Datasource Name     Name of the datasource\n",
-                        "        Datasource ID       The datasource ID, which corresponds to the Id\n",
-                        "                            field in the connector configuration\n",
-                        "        Datasource Class    The datasource class (e.g. 'OSIsoft PI')\n",
-                        "        Data ID             The data ID, whose format is managed by the\n",
-                        "                            datasource connector\n",
-                        "        Cache Enabled       True to find items where data caching is enabled\n",
-                        "        Scoped To           The Seeq ID of a workbook such that results are\n",
-                        "                              limited to ONLY items scoped to that workbook.\n",
-                        "        =================== ===================================================\n",
-                        "    \n",
-                        "    \n",
-                        "    all_properties : bool, default False\n",
-                        "        True if all item properties should be retrieved. This currently makes\n",
-                        "        the search operation much slower as retrieval of properties for an item\n",
-                        "        requires a separate call.\n",
-                        "    \n",
-                        "    workbook : {str, None}\n",
-                        "        A path string (with ' >> ' delimiters) or an ID to indicate a workbook\n",
-                        "        such that, in addition to globally-scoped items, the workbook's scoped\n",
-                        "        items will also be returned in the results.\n",
-                        "    \n",
-                        "        If you want all items regardless of scope, use workbook=None.\n",
-                        "    \n",
-                        "        If you don't want globally-scoped items in your results, use the\n",
-                        "        'Scoped To' field in the 'query' argument instead. (See 'query'\n",
-                        "        argument documentation above.)\n",
-                        "    \n",
-                        "        The ID for a workbook is visible in the URL of Seeq Workbench, directly\n",
-                        "        after the \"workbook/\" part.\n",
-                        "    \n",
-                        "    recursive : bool, default True\n",
-                        "        If True, searches that include a Path entry will include items at and\n",
-                        "        below the specified location in an asset tree. If False, then only\n",
-                        "        items at the specified level will be returned. To get only the root\n",
-                        "        assets, supply a Path value of ''.\n",
-                        "    \n",
-                        "    ignore_unindexed_properties : bool, default True\n",
-                        "        If False, a ValueError will be raised if any properties are supplied\n",
-                        "        that cannot be used in the search.\n",
-                        "    \n",
-                        "    include_archived : bool, default False\n",
-                        "        If True, includes trashed/archived items in the output.\n",
-                        "    \n",
-                        "    estimate_sample_period : dict, default None\n",
-                        "        A dict with the keys 'Start' and 'End'. If provided, an estimated\n",
-                        "        sample period for all signals will be included in the output. The\n",
-                        "        values for the 'Start' and 'End' keys must be a string that\n",
-                        "        pandas.to_datetime() can parse, or a pandas.Timestamp. The start\n",
-                        "        and end times are used to bound the calculation of the sample period.\n",
-                        "        If the start and end times encompass a time range that is insufficient\n",
-                        "        to determine the sample period, a pd.NaT will be returned.\n",
-                        "        If the value of 'Start' is set to None, it will default to the value of\n",
-                        "        'End' minus 1 hour. Conversely, if the value of 'End' is set to None,\n",
-                        "        it will default to now.\n",
-                        "    \n",
-                        "    order_by : {str, list}, default None\n",
-                        "        An optional field or list of fields used to sort the search results.\n",
-                        "        Fields on which results can be sorted are 'ID', 'Name', and 'Description'.\n",
-                        "    \n",
-                        "    quiet : bool, default False\n",
-                        "        If True, suppresses progress output. Note that when status is\n",
-                        "        provided, the quiet setting of the Status object that is passed\n",
-                        "        in takes precedence.\n",
+                        "    quiet : bool\n",
+                        "        If True, suppresses progress output.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If specified, the supplied Status object will be updated as the command\n",
                         "        progresses. It gets filled in with the same information you would see\n",
                         "        in Jupyter in the blue/green/red table below your code while the\n",
                         "        command is executed. The table itself is accessible as a DataFrame via\n",
                         "        the status.df property.\n",
                         "    \n",
-                        "    session : spy.Session, optional\n",
-                        "        If supplied, the Session object (and its Options) will be used to\n",
-                        "        store the login session state. This is useful to log in to different\n",
-                        "        Seeq servers at the same time or with different credentials.\n",
-                        "    \n",
                         "    Returns\n",
                         "    -------\n",
-                        "    pandas.DataFrame\n",
-                        "        A DataFrame with rows for each item found and columns for each\n",
-                        "        property.\n",
-                        "    \n",
-                        "        Additionally, the following properties are stored in the\n",
-                        "        output DataFrame:\n",
-                        "    \n",
-                        "        =================== ===================================================\n",
-                        "        Property            Description\n",
-                        "        =================== ===================================================\n",
-                        "        func                A str value of 'spy.search'\n",
-                        "        kwargs              A dict with the values of the input parameters\n",
-                        "                            passed to spy.search to get the output DataFrame\n",
-                        "        status              A spy.Status object with the status of the\n",
-                        "                            spy.search call\n",
-                        "        =================== ===================================================\n",
-                        "    \n",
-                        "    Examples\n",
-                        "    --------\n",
-                        "    Search for signals with the name 'Humid' on the asset tree under\n",
-                        "    'Example >> Cooling Tower 1', retrieving all properties on the results:\n",
-                        "    \n",
-                        "    >>> search_results = spy.search({'Name': 'Humid', 'Path': 'Example >> Cooling Tower 1'}, all_properties=True)\n",
-                        "    \n",
-                        "    To access the stored properties:\n",
-                        "    >>> search_results.kwargs\n",
-                        "    >>> search_results.status\n",
-                        "    \n",
-                        "    Search for signals that have a name that starts with 'Area' in the datasource 'Example Data' and\n",
-                        "    determine the sample period of each signal during the month of January 2018\n",
-                        "    \n",
-                        "    >>> search_results = spy.search({\n",
-                        "    >>>    'Name': 'Area ?_*',\n",
-                        "    >>>    'Datasource Name': 'Example Data'\n",
-                        "    >>> }, estimate_sample_period=dict(Start='2018-01-01', End='2018-02-01'))\n",
-                        "    \n",
-                        "    Using a pandas.DataFrame as the input:\n",
-                        "    \n",
-                        "    >>> my_items = pd.DataFrame(\n",
-                        "    >>>     {'Name': ['Area A_Temperature', 'Area B_Compressor Power', 'Optimize' ],\n",
-                        "    >>>      'Datasource Name': 'Example Data'})\n",
-                        "    >>> spy.search(my_items)\n",
-                        "    \n",
-                        "    Using a URL from a Seeq Workbench worksheet:\n",
-                        "    \n",
-                        "    >>> my_worksheet_items = spy.search(\n",
-                        "    >>> 'https://seeq.com/workbook/17F31703-F0B6-4C8E-B7FD-E20897BD4819/worksheet/CE6A0B92-EE00-45FC-9EB3-D162632DBB48')\n",
+                        "    pd.DataFrame\n",
+                        "        The jobs_df with an appended column containing a description of the\n",
+                        "        schedule\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "from seeq import spy\n",
-                "help(spy.search)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "If you are in the Jupyter user interface (e.g., you are using Seeq Data Lab), you can also access help by\n",
-                "putting your cursor on the name of the function (e.g., the `search` part of `spy.search()`) and pressing\n",
-                "Shift+Tab. (You may also need to click the `+` button to expand the view, since much of the SPy documentation is\n",
-                "lengthy.)"
+                "help(spy.jobs.schedule)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/Example Export.zip` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/Example Export.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,53 +1,60 @@
-Zip file size: 94677 bytes, number of entries: 51
--rw-rw-rw-  2.0 fat      867 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Datasources.json
--rw-rw-rw-  2.0 fat     1023 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Datasource_Map_Auth_Seeq_Seeq.json
--rw-rw-rw-  2.0 fat      694 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Datasource_Map_Seeq Calculations_Seeq Calculations_Seeq Calculations.json
--rw-rw-rw-  2.0 fat      686 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Datasource_Map_Time Series CSV Files_Example Data_Example Data.json
--rw-rw-rw-  2.0 fat    42088 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Items.json
--rw-rw-rw-  2.0 fat      807 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_10198C29-C93C-4055-B313-3388227D0621.html
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6.html
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_44A42737-E20C-4BCE-BB50-4F2468C7419D.html
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_99E1E62B-69F1-4FFB-8649-3225820A7DFB.html
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1.html
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_D978C84E-9435-422F-9C1A-DC4C7E515C0B.html
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_F255BF0D-CCE1-4021-B863-B121FB605913.html
--rw-rw-rw-  2.0 fat     7454 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Workbook.json
--rw-rw-rw-  2.0 fat      589 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621.json
--rw-rw-rw-  2.0 fat    16669 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_1A3522FD-984C-44FF-8928-C466E021DCA4.json
--rw-rw-rw-  2.0 fat     1242 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_1DCFA3AF-77BD-4198-AA0C-C3F549BAA48A.json
--rw-rw-rw-  2.0 fat    18714 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_FD90346A-BF72-4319-9134-3922A012C0DB.json
--rw-rw-rw-  2.0 fat      598 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6.json
--rw-rw-rw-  2.0 fat    22655 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_1945AADF-E4E3-4362-AB6A-DC5C6724E9F4.json
--rw-rw-rw-  2.0 fat    20124 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_221933FE-7956-4888-A3C9-AF1F3971EBA5.json
--rw-rw-rw-  2.0 fat     1242 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_B364236F-3815-4E3F-A4C2-FDF636A2D313.json
--rw-rw-rw-  2.0 fat      592 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_44A42737-E20C-4BCE-BB50-4F2468C7419D.json
--rw-rw-rw-  2.0 fat    17814 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_44A42737-E20C-4BCE-BB50-4F2468C7419D_Workstep_2E03BF34-01A5-4332-A89C-35D73ED1DDC8.json
--rw-rw-rw-  2.0 fat     1242 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_44A42737-E20C-4BCE-BB50-4F2468C7419D_Workstep_5366156C-07CB-4724-9C18-41AA8123B939.json
--rw-rw-rw-  2.0 fat      589 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB.json
--rw-rw-rw-  2.0 fat    20363 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB_Workstep_38151CE5-B36E-4D77-AD00-1995F886CFD2.json
--rw-rw-rw-  2.0 fat     1242 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB_Workstep_8CD6F7D5-8358-4725-A39B-E68B47D9D1BB.json
--rw-rw-rw-  2.0 fat      591 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1.json
--rw-rw-rw-  2.0 fat     1243 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_15B8DB00-1095-4560-BA40-DA7E23A9AFC1.json
--rw-rw-rw-  2.0 fat    17906 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_89535DFA-9A1A-4E75-BF3E-32048EB2B7F5.json
--rw-rw-rw-  2.0 fat    21547 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_C6610DD2-779B-45F8-877A-54A9C3107973.json
--rw-rw-rw-  2.0 fat      588 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B.json
--rw-rw-rw-  2.0 fat    17704 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B_Workstep_962F2F33-DAE6-482F-AD90-2ED4E1577406.json
--rw-rw-rw-  2.0 fat     1242 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B_Workstep_B66A34BE-1B59-4064-9E87-625808FC4146.json
--rw-rw-rw-  2.0 fat      594 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913.json
--rw-rw-rw-  2.0 fat    20087 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_108C566D-6293-4075-BBD5-C22E174F00AE.json
--rw-rw-rw-  2.0 fat     1246 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_6797D860-D3CE-4649-9D4B-F271E600CE45.json
--rw-rw-rw-  2.0 fat    23370 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_79B86A9F-43CE-47BD-9C29-8940BF6B5D6C.json
--rw-rw-rw-  2.0 fat    21368 b- defN 23-Apr-12 10:29 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_BE9F59EB-0151-4B25-BE08-16FFE5D8D85D.json
--rw-rw-rw-  2.0 fat      570 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Datasources.json
--rw-rw-rw-  2.0 fat     1023 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Datasource_Map_Auth_Seeq_Seeq.json
--rw-rw-rw-  2.0 fat      694 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Datasource_Map_Seeq Calculations_Seeq Calculations_Seeq Calculations.json
--rw-rw-rw-  2.0 fat    25001 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Image_CF590E20-AA52-441E-81E3-554C7F893FBA_1596236583342_v1.png
--rw-rw-rw-  2.0 fat     7438 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Items.json
--rw-rw-rw-  2.0 fat     1105 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Report_50A98248-9FBB-4A28-BD3E-CEE434BD359D.html
--rw-rw-rw-  2.0 fat     4724 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Report_50A98248-9FBB-4A28-BD3E-CEE434BD359D.json
--rw-rw-rw-  2.0 fat     1047 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Report_E5B84916-5962-49A7-9987-052CF80CD077.html
--rw-rw-rw-  2.0 fat     2247 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Report_E5B84916-5962-49A7-9987-052CF80CD077.json
--rw-rw-rw-  2.0 fat     5107 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Workbook.json
--rw-rw-rw-  2.0 fat      522 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Worksheet_50A98248-9FBB-4A28-BD3E-CEE434BD359D.json
--rw-rw-rw-  2.0 fat      524 b- defN 23-Apr-12 10:29 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Worksheet_E5B84916-5962-49A7-9987-052CF80CD077.json
-51 files, 354782 bytes uncompressed, 78621 bytes compressed:  77.8%
+Zip file size: 100268 bytes, number of entries: 58
+-rw-rw-rw-  2.0 fat      867 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Datasources.json
+-rw-rw-rw-  2.0 fat     1023 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Datasource_Map_Auth_Seeq_Seeq.json
+-rw-rw-rw-  2.0 fat      694 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Datasource_Map_Seeq Calculations_Seeq Calculations_Seeq Calculations.json
+-rw-rw-rw-  2.0 fat      686 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Datasource_Map_Time Series CSV Files_Example Data_Example Data.json
+-rw-rw-rw-  2.0 fat    40959 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Items.json
+-rw-rw-rw-  2.0 fat      807 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_10198C29-C93C-4055-B313-3388227D0621.html
+-rw-rw-rw-  2.0 fat     2866 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_10198C29-C93C-4055-B313-3388227D0621.json
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6.html
+-rw-rw-rw-  2.0 fat      602 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6.json
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_44A42737-E20C-4BCE-BB50-4F2468C7419D.html
+-rw-rw-rw-  2.0 fat      353 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_44A42737-E20C-4BCE-BB50-4F2468C7419D.json
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_99E1E62B-69F1-4FFB-8649-3225820A7DFB.html
+-rw-rw-rw-  2.0 fat      353 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_99E1E62B-69F1-4FFB-8649-3225820A7DFB.json
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1.html
+-rw-rw-rw-  2.0 fat      353 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1.json
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_D978C84E-9435-422F-9C1A-DC4C7E515C0B.html
+-rw-rw-rw-  2.0 fat      353 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_D978C84E-9435-422F-9C1A-DC4C7E515C0B.json
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_F255BF0D-CCE1-4021-B863-B121FB605913.html
+-rw-rw-rw-  2.0 fat      353 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_F255BF0D-CCE1-4021-B863-B121FB605913.json
+-rw-rw-rw-  2.0 fat     7454 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Workbook.json
+-rw-rw-rw-  2.0 fat      589 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621.json
+-rw-rw-rw-  2.0 fat    16669 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_1A3522FD-984C-44FF-8928-C466E021DCA4.json
+-rw-rw-rw-  2.0 fat     1243 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_7951145D-AA2F-4196-8422-39335A5C5C59.json
+-rw-rw-rw-  2.0 fat    18714 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_FD90346A-BF72-4319-9134-3922A012C0DB.json
+-rw-rw-rw-  2.0 fat      598 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6.json
+-rw-rw-rw-  2.0 fat    22655 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_1945AADF-E4E3-4362-AB6A-DC5C6724E9F4.json
+-rw-rw-rw-  2.0 fat    20124 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_221933FE-7956-4888-A3C9-AF1F3971EBA5.json
+-rw-rw-rw-  2.0 fat     1242 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_D1827683-15C9-4194-A52A-6ADADBB2AF28.json
+-rw-rw-rw-  2.0 fat      592 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_44A42737-E20C-4BCE-BB50-4F2468C7419D.json
+-rw-rw-rw-  2.0 fat    17814 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_44A42737-E20C-4BCE-BB50-4F2468C7419D_Workstep_2E03BF34-01A5-4332-A89C-35D73ED1DDC8.json
+-rw-rw-rw-  2.0 fat     1242 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_44A42737-E20C-4BCE-BB50-4F2468C7419D_Workstep_38BE023E-7380-4160-800B-C615C93B90EF.json
+-rw-rw-rw-  2.0 fat      589 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB.json
+-rw-rw-rw-  2.0 fat    20363 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB_Workstep_38151CE5-B36E-4D77-AD00-1995F886CFD2.json
+-rw-rw-rw-  2.0 fat     1242 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB_Workstep_4D8421AB-A1C0-42FF-B114-3749BC6753D1.json
+-rw-rw-rw-  2.0 fat      591 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1.json
+-rw-rw-rw-  2.0 fat    17906 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_89535DFA-9A1A-4E75-BF3E-32048EB2B7F5.json
+-rw-rw-rw-  2.0 fat    21547 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_C6610DD2-779B-45F8-877A-54A9C3107973.json
+-rw-rw-rw-  2.0 fat     1243 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_E31E275F-8295-43A7-9FC2-E66711C407E8.json
+-rw-rw-rw-  2.0 fat      588 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B.json
+-rw-rw-rw-  2.0 fat     1243 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B_Workstep_1204D33F-257E-4CBD-A6A7-EFAF0D765749.json
+-rw-rw-rw-  2.0 fat    17704 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B_Workstep_962F2F33-DAE6-482F-AD90-2ED4E1577406.json
+-rw-rw-rw-  2.0 fat      594 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913.json
+-rw-rw-rw-  2.0 fat    20087 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_108C566D-6293-4075-BBD5-C22E174F00AE.json
+-rw-rw-rw-  2.0 fat     1246 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_385CF8DA-B5DF-42CE-BA05-BABE20B21F20.json
+-rw-rw-rw-  2.0 fat    23370 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_79B86A9F-43CE-47BD-9C29-8940BF6B5D6C.json
+-rw-rw-rw-  2.0 fat    21368 b- defN 23-Jun-24 21:35 Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_BE9F59EB-0151-4B25-BE08-16FFE5D8D85D.json
+-rw-rw-rw-  2.0 fat      570 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Datasources.json
+-rw-rw-rw-  2.0 fat     1023 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Datasource_Map_Auth_Seeq_Seeq.json
+-rw-rw-rw-  2.0 fat      694 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Datasource_Map_Seeq Calculations_Seeq Calculations_Seeq Calculations.json
+-rw-rw-rw-  2.0 fat    25001 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Image_CF590E20-AA52-441E-81E3-554C7F893FBA_1596236583342_v1.png
+-rw-rw-rw-  2.0 fat     7344 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Items.json
+-rw-rw-rw-  2.0 fat     1105 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Report_50A98248-9FBB-4A28-BD3E-CEE434BD359D.html
+-rw-rw-rw-  2.0 fat    10323 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Report_50A98248-9FBB-4A28-BD3E-CEE434BD359D.json
+-rw-rw-rw-  2.0 fat     1047 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Report_E5B84916-5962-49A7-9987-052CF80CD077.html
+-rw-rw-rw-  2.0 fat     6901 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Report_E5B84916-5962-49A7-9987-052CF80CD077.json
+-rw-rw-rw-  2.0 fat     5107 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Workbook.json
+-rw-rw-rw-  2.0 fat      522 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Worksheet_50A98248-9FBB-4A28-BD3E-CEE434BD359D.json
+-rw-rw-rw-  2.0 fat      524 b- defN 23-Jun-24 21:35 Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Worksheet_E5B84916-5962-49A7-9987-052CF80CD077.json
+58 files, 369047 bytes uncompressed, 82210 bytes compressed:  77.7%
```

#### zipnote {}

```diff
@@ -12,105 +12,126 @@
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Items.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_10198C29-C93C-4055-B313-3388227D0621.html
 Comment: 
 
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_10198C29-C93C-4055-B313-3388227D0621.json
+Comment: 
+
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6.html
 Comment: 
 
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6.json
+Comment: 
+
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_44A42737-E20C-4BCE-BB50-4F2468C7419D.html
 Comment: 
 
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_44A42737-E20C-4BCE-BB50-4F2468C7419D.json
+Comment: 
+
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_99E1E62B-69F1-4FFB-8649-3225820A7DFB.html
 Comment: 
 
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_99E1E62B-69F1-4FFB-8649-3225820A7DFB.json
+Comment: 
+
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1.html
 Comment: 
 
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1.json
+Comment: 
+
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_D978C84E-9435-422F-9C1A-DC4C7E515C0B.html
 Comment: 
 
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_D978C84E-9435-422F-9C1A-DC4C7E515C0B.json
+Comment: 
+
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_F255BF0D-CCE1-4021-B863-B121FB605913.html
 Comment: 
 
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Journal_F255BF0D-CCE1-4021-B863-B121FB605913.json
+Comment: 
+
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Workbook.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_1A3522FD-984C-44FF-8928-C466E021DCA4.json
 Comment: 
 
-Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_1DCFA3AF-77BD-4198-AA0C-C3F549BAA48A.json
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_7951145D-AA2F-4196-8422-39335A5C5C59.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_FD90346A-BF72-4319-9134-3922A012C0DB.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_1945AADF-E4E3-4362-AB6A-DC5C6724E9F4.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_221933FE-7956-4888-A3C9-AF1F3971EBA5.json
 Comment: 
 
-Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_B364236F-3815-4E3F-A4C2-FDF636A2D313.json
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_D1827683-15C9-4194-A52A-6ADADBB2AF28.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_44A42737-E20C-4BCE-BB50-4F2468C7419D.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_44A42737-E20C-4BCE-BB50-4F2468C7419D_Workstep_2E03BF34-01A5-4332-A89C-35D73ED1DDC8.json
 Comment: 
 
-Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_44A42737-E20C-4BCE-BB50-4F2468C7419D_Workstep_5366156C-07CB-4724-9C18-41AA8123B939.json
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_44A42737-E20C-4BCE-BB50-4F2468C7419D_Workstep_38BE023E-7380-4160-800B-C615C93B90EF.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB_Workstep_38151CE5-B36E-4D77-AD00-1995F886CFD2.json
 Comment: 
 
-Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB_Workstep_8CD6F7D5-8358-4725-A39B-E68B47D9D1BB.json
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB_Workstep_4D8421AB-A1C0-42FF-B114-3749BC6753D1.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1.json
 Comment: 
 
-Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_15B8DB00-1095-4560-BA40-DA7E23A9AFC1.json
-Comment: 
-
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_89535DFA-9A1A-4E75-BF3E-32048EB2B7F5.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_C6610DD2-779B-45F8-877A-54A9C3107973.json
 Comment: 
 
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_E31E275F-8295-43A7-9FC2-E66711C407E8.json
+Comment: 
+
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B.json
 Comment: 
 
-Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B_Workstep_962F2F33-DAE6-482F-AD90-2ED4E1577406.json
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B_Workstep_1204D33F-257E-4CBD-A6A7-EFAF0D765749.json
 Comment: 
 
-Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B_Workstep_B66A34BE-1B59-4064-9E87-625808FC4146.json
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B_Workstep_962F2F33-DAE6-482F-AD90-2ED4E1577406.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_108C566D-6293-4075-BBD5-C22E174F00AE.json
 Comment: 
 
-Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_6797D860-D3CE-4649-9D4B-F271E600CE45.json
+Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_385CF8DA-B5DF-42CE-BA05-BABE20B21F20.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_79B86A9F-43CE-47BD-9C29-8940BF6B5D6C.json
 Comment: 
 
 Filename: Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_BE9F59EB-0151-4B25-BE08-16FFE5D8D85D.json
 Comment:
```

#### Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Items.json

##### Pretty-printed

 * *Similarity: 0.9487412389198101%*

 * *Differences: {"'15359EB5-57E9-4A60-A5DA-454885854076'": "{delete: ['Asset', 'Path']}",*

 * * "'2913AEA3-0D61-4271-AF3D-C44CA975B4D7'": "{delete: ['Asset', 'Path']}",*

 * * "'2E09EBCB-1A2B-4BB9-85C6-24AB7B6E01AF'": "{delete: ['Asset', 'Path']}",*

 * * "'32302B01-EE96-4A96-B00B-59DBEA2678EE'": "{delete: ['Asset', 'Path']}",*

 * * "'355DE70E-5478-45D9-B14C-94BF76B81F0C'": "{delete: ['Asset', 'Path']}",*

 * * "'38E66380-26C1-4374-B6F2-C8CC91B4932D'": "{delete: ['Asset', 'Path']}",*

 * * "'47D091C1-1780-4EA0-BD54-AA6E13213EB8'": "{'Sync Token': '2023-06- […]*

```diff
@@ -1,11 +1,10 @@
 {
     "15359EB5-57E9-4A60-A5DA-454885854076": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "f0ddec62-a1fe-4e35-9106-c94829d14d67",
         "Cached By Service": true,
         "Data ID": "15359EB5-57E9-4A60-A5DA-454885854076",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -21,15 +20,14 @@
             "repeatOverCondition": "C1C00D7E-5FFC-43CC-9901-8CB99E7E996E"
         },
         "ID": "15359EB5-57E9-4A60-A5DA-454885854076",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "5",
         "Name": "Temp HiHi",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedSignal",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "griddingPeriod": {
                 "units": "min",
                 "value": 5
@@ -45,28 +43,26 @@
             "windowStart": 1514840921352
         },
         "Unsearchable": false,
         "Value Unit Of Measure": "\u00b0F"
     },
     "2913AEA3-0D61-4271-AF3D-C44CA975B4D7": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "d9783454-07be-4917-ade6-36ef31286454",
         "Data ID": "2913aea3-0d61-4271-af3d-c44ca975b4d7",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
         "Formula": "$b.max(capsule('2018-01-01T00:00:00Z', '2018-02-01T00:00:00Z')).value()",
         "Formula Parameters": {
             "b": "9564A6B8-8A8F-4F6D-AC63-00EA38962B7A"
         },
         "ID": "2913AEA3-0D61-4271-AF3D-C44CA975B4D7",
         "Name": "Temperature Limit",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedScalar",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "maximumDuration": {
                 "units": "day",
                 "value": 1
@@ -74,15 +70,14 @@
             "type": "power-search"
         },
         "Unit Of Measure": "\u00b0F",
         "Unsearchable": false
     },
     "2E09EBCB-1A2B-4BB9-85C6-24AB7B6E01AF": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "82bc675c-1131-47d6-9c9d-42818b23281b",
         "Cached By Service": true,
         "Data ID": "2E09EBCB-1A2B-4BB9-85C6-24AB7B6E01AF",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -98,15 +93,14 @@
             "repeatOverCondition": "C1C00D7E-5FFC-43CC-9901-8CB99E7E996E"
         },
         "ID": "2E09EBCB-1A2B-4BB9-85C6-24AB7B6E01AF",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "5",
         "Name": "Temp LoLo",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedSignal",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "griddingPeriod": {
                 "units": "min",
                 "value": 5
@@ -122,15 +116,14 @@
             "windowStart": 1514840921352
         },
         "Unsearchable": false,
         "Value Unit Of Measure": "\u00b0F"
     },
     "32302B01-EE96-4A96-B00B-59DBEA2678EE": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "be85cdbb-1b19-4eeb-96db-221c2d1d33e0",
         "Cached By Service": true,
         "Data ID": "32302B01-EE96-4A96-B00B-59DBEA2678EE",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -146,15 +139,14 @@
             "repeatOverCondition": "C1C00D7E-5FFC-43CC-9901-8CB99E7E996E"
         },
         "ID": "32302B01-EE96-4A96-B00B-59DBEA2678EE",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "5",
         "Name": "Temperature Warning Upper",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedSignal",
         "UIConfig": {
             "advancedParametersCollapsed": false,
             "griddingPeriod": {
                 "units": "min",
                 "value": 5
@@ -166,15 +158,14 @@
             "windowStart": 1546385007130
         },
         "Unsearchable": false,
         "Value Unit Of Measure": "\u00b0F"
     },
     "355DE70E-5478-45D9-B14C-94BF76B81F0C": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Data ID": "355DE70E-5478-45D9-B14C-94BF76B81F0C",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
         "Formula": "<ThresholdMetric>",
         "Formula Parameters": {
@@ -205,41 +196,38 @@
                         "Name": "LoLo"
                     }
                 }
             ]
         },
         "ID": "355DE70E-5478-45D9-B14C-94BF76B81F0C",
         "Name": "Temperature With Bounds",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "ThresholdMetric",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "type": "threshold-metric"
         },
         "Unsearchable": false
     },
     "38E66380-26C1-4374-B6F2-C8CC91B4932D": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Data ID": "38E66380-26C1-4374-B6F2-C8CC91B4932D",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
         "Formula": "conditionTable($yValueSignal1.toStates(capsule(10%, 85%).partition(5%)).toCondition(\"yValueCol1\").toGroup($viewCapsule, CapsuleBoundary.Intersect), \"yValueCol1\", $condition2.toGroup($viewCapsule), \"Value\").addStatColumn(\"signalToAggregate\", $signalToAggregate, average())",
         "Formula Parameters": {
             "condition2": "88BF5D71-421F-45BE-92C1-C907DF978191",
             "signalToAggregate": "9564A6B8-8A8F-4F6D-AC63-00EA38962B7A",
             "viewCapsule": "capsule(\"2018-11-05T04:59:48.188Z\", \"2018-11-12T04:59:48.188Z\")",
             "yValueSignal1": "D581F7B7-9678-4586-A811-1A1F9F878459"
         },
         "ID": "38E66380-26C1-4374-B6F2-C8CC91B4932D",
         "Name": "Temp vs Avg Humidity",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "Chart",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "aggregationConfigs": [
                 {
                     "binSize": "5",
@@ -271,47 +259,46 @@
             "type": "aggregation-bins-table",
             "yValueSignal": ""
         },
         "Unsearchable": false
     },
     "47D091C1-1780-4EA0-BD54-AA6E13213EB8": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Cache ID": "20b2ae1c-e62d-4b9d-bb6e-f5d5d5bf6a39",
         "Cached By Service": true,
         "Data ID": "[Tag] Area A_Optimizer.sim.ts.csv",
         "Datasource Class": "Time Series CSV Files",
         "Datasource ID": "Example Data",
         "Enabled": true,
         "ID": "47D091C1-1780-4EA0-BD54-AA6E13213EB8",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2min",
         "Name": "Area A_Optimizer",
-        "Path": null,
         "Source Maximum Interpolation": "2min",
         "Source Value Unit Of Measure": "",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "StoredSignal",
         "Unsearchable": false,
         "Value Unit Of Measure": ""
     },
     "4B40EAFC-91ED-4AB0-8199-F21AF40A8350": {
         "Archived": false,
-        "Asset": "Cooling Tower 1",
+        "Asset": "Area A",
         "Cache Enabled": false,
         "Data ID": "root/Cooling Tower 1/Area A",
         "Datasource Class": "Time Series CSV Files",
         "Datasource ID": "Example Data",
         "Enabled": true,
         "ID": "4B40EAFC-91ED-4AB0-8199-F21AF40A8350",
         "Name": "Area A",
-        "Path": "Example",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Old Asset Format": false,
+        "Path": "Example >> Cooling Tower 1",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "Asset",
         "Unsearchable": false
     },
     "51297B6C-9E44-4815-9C17-297ABC4A5D46": {
         "Access Control": [
             {
                 "ID": "2f29a19e-6c9e-49ac-b394-1f75864fd569",
@@ -428,15 +415,14 @@
         },
         "Type": "Folder",
         "Unsearchable": false,
         "Updated At": "1571753347497016700"
     },
     "553DFA1F-BF27-4679-83FB-B6415B1FECB3": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "a63993ab-98b2-4db4-a152-5c23f5ec9302",
         "Cached By Service": true,
         "Data ID": "553dfa1f-bf27-4679-83fb-b6415b1fecb3",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -445,15 +431,14 @@
             "a": "9564A6B8-8A8F-4F6D-AC63-00EA38962B7A"
         },
         "ID": "553DFA1F-BF27-4679-83FB-B6415B1FECB3",
         "Key Unit Of Measure": "ns",
         "Maximum Duration": "1",
         "Metadata Properties": "",
         "Name": "High Temperature",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedCondition",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "limitsParams": {
                 "entryCondition": {
                     "duration": {
@@ -480,15 +465,14 @@
             },
             "type": "limits"
         },
         "Unsearchable": false
     },
     "5C09B1E4-8E3C-44FC-AFFA-0060D3557D0C": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "f21f8da3-6d66-4638-9d11-a9113b2c58db",
         "Cached By Service": true,
         "Data ID": "5C09B1E4-8E3C-44FC-AFFA-0060D3557D0C",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -497,15 +481,14 @@
             "b": "9564A6B8-8A8F-4F6D-AC63-00EA38962B7A"
         },
         "ID": "5C09B1E4-8E3C-44FC-AFFA-0060D3557D0C",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2",
         "Name": "Delayed Smooth Temperature",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedSignal",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "maximumDuration": {
                 "units": "day",
                 "value": 1
@@ -513,15 +496,14 @@
             "type": "power-search"
         },
         "Unsearchable": false,
         "Value Unit Of Measure": "\u00b0F"
     },
     "6ABEEA79-1D4A-4EE8-A237-6C1B8B40B065": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "dfb701c1-aa34-45d0-8c0c-02eb6ca4bb9c",
         "Cached By Service": true,
         "Data ID": "6abeea79-1d4a-4ee8-a237-6c1b8b40b065",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -538,15 +520,14 @@
             "input": "8A4F0E26-8A0C-4127-9E11-B67E031C6049"
         },
         "ID": "6ABEEA79-1D4A-4EE8-A237-6C1B8B40B065",
         "Key Unit Of Measure": "ns",
         "Maximum Duration": "40",
         "Metadata Properties": "",
         "Name": "Temperature Deviation",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedCondition",
         "UIConfig": {
             "advancedParametersCollapsed": false,
             "condition": "OUTSIDE",
             "endDuration": {
                 "units": "min",
@@ -560,15 +541,14 @@
             "startLocation": true,
             "type": "deviation"
         },
         "Unsearchable": false
     },
     "88BF5D71-421F-45BE-92C1-C907DF978191": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "7cb9f574-8b86-49cd-9ab9-30d30507fcf5",
         "Cached By Service": true,
         "Data ID": "88bf5d71-421f-45be-92c1-c907df978191",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -577,15 +557,14 @@
             "b": "D2C089B6-CE85-46FC-8392-E11CC0C08336"
         },
         "ID": "88BF5D71-421F-45BE-92C1-C907DF978191",
         "Key Unit Of Measure": "ns",
         "Maximum Duration": "2",
         "Metadata Properties": "Value=string",
         "Name": "Optimizer Condition",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedCondition",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "maximumDuration": {
                 "units": "day",
                 "value": 1
@@ -608,22 +587,21 @@
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2min",
         "Name": "Temperature",
         "Path": "Example >> Cooling Tower 1",
         "Source Maximum Interpolation": "2min",
         "Source Value Unit Of Measure": "\u00b0F",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "StoredSignal",
         "Unsearchable": false,
         "Value Unit Of Measure": "\u00b0F"
     },
     "8C048548-8E83-4380-8B24-9DAD56B5C2CF": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "9a26fedc-c2c0-45b8-a9da-7b89fda01de1",
         "Cached By Service": true,
         "Data ID": "8c048548-8e83-4380-8b24-9dad56b5c2cf",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -632,15 +610,14 @@
             "a": "DCED9C36-A4BE-4783-9216-DC06B3F57D8C"
         },
         "ID": "8C048548-8E83-4380-8B24-9DAD56B5C2CF",
         "Key Unit Of Measure": "ns",
         "Maximum Duration": "1",
         "Metadata Properties": "",
         "Name": "High Power",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedCondition",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "limitsParams": {
                 "entryCondition": {
                     "duration": {
@@ -667,61 +644,56 @@
             },
             "type": "limits"
         },
         "Unsearchable": false
     },
     "9564A6B8-8A8F-4F6D-AC63-00EA38962B7A": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Cache ID": "3b4ebcda-de18-47fb-ac65-99321c8f2b66",
         "Cached By Service": true,
         "Data ID": "[Tag] Area A_Temperature.sim.ts.csv",
         "Datasource Class": "Time Series CSV Files",
         "Datasource ID": "Example Data",
         "Enabled": true,
         "ID": "9564A6B8-8A8F-4F6D-AC63-00EA38962B7A",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2min",
         "Name": "Area A_Temperature",
-        "Path": null,
         "Source Maximum Interpolation": "2min",
         "Source Value Unit Of Measure": "\u00b0F",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "StoredSignal",
         "Unsearchable": false,
         "Value Unit Of Measure": "\u00b0F"
     },
     "B396F2A6-CD3C-4AC6-9649-EA5E56379578": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Cache ID": "02aaa79c-38ac-440b-bec5-61ab2231266a",
         "Cached By Service": true,
         "Data ID": "[Tag] Area A_Wet Bulb.sim.ts.csv",
         "Datasource Class": "Time Series CSV Files",
         "Datasource ID": "Example Data",
         "Enabled": true,
         "ID": "B396F2A6-CD3C-4AC6-9649-EA5E56379578",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2min",
         "Name": "Area A_Wet Bulb",
-        "Path": null,
         "Source Maximum Interpolation": "2min",
         "Source Value Unit Of Measure": "\u00b0F",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "StoredSignal",
         "Unsearchable": false,
         "Value Unit Of Measure": "\u00b0F"
     },
     "C1C00D7E-5FFC-43CC-9901-8CB99E7E996E": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "eaaaac2a-6d7e-42a4-9052-a39c7a6c18a3",
         "Cached By Service": true,
         "Data ID": "c1c00d7e-5ffc-43cc-9901-8cb99e7e996e",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -729,15 +701,14 @@
         "Formula Parameters": {},
         "ID": "C1C00D7E-5FFC-43CC-9901-8CB99E7E996E",
         "Key Unit Of Measure": "ns",
         "Maximum Duration": "1.0416666666666667",
         "Maximum Interpolation": "1.0416666666666667",
         "Metadata Properties": "Day+of+Year=&Day+of+Week=&Day+of+Month=",
         "Name": "Daily",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedCondition",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "duration": "days",
             "frequencies": [],
             "maximumDuration": {
@@ -756,15 +727,14 @@
             "type": "periodic-condition",
             "weekStart": "Day.Sunday"
         },
         "Unsearchable": false
     },
     "C93E74CA-0FB5-4CBF-9634-4031CD11B3B5": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Data ID": "C93E74CA-0FB5-4CBF-9634-4031CD11B3B5",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
         "Formula": "<ThresholdMetric>",
         "Formula Parameters": {
@@ -788,22 +758,20 @@
                     }
                 }
             ]
         },
         "ID": "C93E74CA-0FB5-4CBF-9634-4031CD11B3B5",
         "Name": "Warning Boundary",
         "NeutralColor": "#0070c0",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "ThresholdMetric",
         "Unsearchable": false
     },
     "CCD70C84-F21E-4983-822F-5480BC50191D": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "22a7523c-c578-4edb-93ba-26cd8aa4ccb6",
         "Cached By Service": true,
         "Data ID": "CCD70C84-F21E-4983-822F-5480BC50191D",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -812,30 +780,28 @@
             "a": "B396F2A6-CD3C-4AC6-9649-EA5E56379578"
         },
         "ID": "CCD70C84-F21E-4983-822F-5480BC50191D",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "15.0",
         "Name": "Rate of Change of Wet Bulb",
-        "Path": null,
         "Type": "CalculatedSignal",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "maximumDuration": {
                 "units": "day",
                 "value": 1
             },
             "type": "power-search"
         },
         "Unsearchable": false,
         "Value Unit Of Measure": "\u00b0F/h"
     },
     "CE98C80E-838D-46E6-8250-2F5D887E86C6": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Data ID": "CE98C80E-838D-46E6-8250-2F5D887E86C6",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
         "Formula": "<ThresholdMetric>",
         "Formula Parameters": {
@@ -866,49 +832,45 @@
                         "Value": 30
                     }
                 }
             ]
         },
         "ID": "CE98C80E-838D-46E6-8250-2F5D887E86C6",
         "Name": "Average Daily Temperature",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "ThresholdMetric",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "type": "threshold-metric"
         },
         "Unsearchable": false
     },
     "D2C089B6-CE85-46FC-8392-E11CC0C08336": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Cache ID": "ce50ccae-6884-418a-9472-46400e4e5fe5",
         "Cached By Service": true,
         "Data ID": "[Tag] Area A_Compressor Stage.sim.ts.csv",
         "Datasource Class": "Time Series CSV Files",
         "Datasource ID": "Example Data",
         "Enabled": true,
         "ID": "D2C089B6-CE85-46FC-8392-E11CC0C08336",
         "Interpolation Method": "Step",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2min",
         "Name": "Area A_Compressor Stage",
-        "Path": null,
         "Source Maximum Interpolation": "2min",
         "Source Value Unit Of Measure": "string",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "StoredSignal",
         "Unsearchable": false,
         "Value Unit Of Measure": "string"
     },
     "D5586EDF-FF35-4C8B-85AC-50764C8A806F": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "eb387b62-1ce6-4f3a-bd49-0c04b2db8ae2",
         "Cached By Service": true,
         "Data ID": "D5586EDF-FF35-4C8B-85AC-50764C8A806F",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -924,15 +886,14 @@
             "repeatOverCondition": "C1C00D7E-5FFC-43CC-9901-8CB99E7E996E"
         },
         "ID": "D5586EDF-FF35-4C8B-85AC-50764C8A806F",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "5",
         "Name": "Temperature Warning Lower",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedSignal",
         "UIConfig": {
             "advancedParametersCollapsed": false,
             "griddingPeriod": {
                 "units": "min",
                 "value": 5
@@ -944,84 +905,77 @@
             "windowStart": 1546385007130
         },
         "Unsearchable": false,
         "Value Unit Of Measure": "\u00b0F"
     },
     "D581F7B7-9678-4586-A811-1A1F9F878459": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Cache ID": "2d8646d4-4f44-401e-a230-bc2ed1c5077f",
         "Cached By Service": true,
         "Data ID": "[Tag] Area A_Relative Humidity.sim.ts.csv",
         "Datasource Class": "Time Series CSV Files",
         "Datasource ID": "Example Data",
         "Enabled": true,
         "ID": "D581F7B7-9678-4586-A811-1A1F9F878459",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2min",
         "Name": "Area A_Relative Humidity",
-        "Path": null,
         "Source Maximum Interpolation": "2min",
         "Source Value Unit Of Measure": "%",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "StoredSignal",
         "Unsearchable": false,
         "Value Unit Of Measure": "%"
     },
     "DCED9C36-A4BE-4783-9216-DC06B3F57D8C": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Cache ID": "e8a5b813-6756-4588-a0a6-028b3150b587",
         "Cached By Service": true,
         "Data ID": "[Tag] Area A_Compressor Power.sim.ts.csv",
         "Datasource Class": "Time Series CSV Files",
         "Datasource ID": "Example Data",
         "Enabled": true,
         "ID": "DCED9C36-A4BE-4783-9216-DC06B3F57D8C",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2min",
         "Name": "Area A_Compressor Power",
-        "Path": null,
         "Source Maximum Interpolation": "2min",
         "Source Value Unit Of Measure": "kW",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "StoredSignal",
         "Unsearchable": false,
         "Value Unit Of Measure": "kW"
     },
     "DF3E0953-12D6-444C-8F9C-3DEDB2999D5A": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Cache ID": "b8652a20-9ce1-439a-bb04-252efe5f6dc2",
         "Cached By Service": true,
         "Data ID": "[Tag] Area C_Temperature.sim.ts.csv",
         "Datasource Class": "Time Series CSV Files",
         "Datasource ID": "Example Data",
         "Enabled": true,
         "ID": "DF3E0953-12D6-444C-8F9C-3DEDB2999D5A",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2min",
         "Name": "Area C_Temperature",
-        "Path": null,
         "Source Maximum Interpolation": "2min",
         "Source Value Unit Of Measure": "F",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "StoredSignal",
         "Unsearchable": false,
         "Value Unit Of Measure": "\u00b0F"
     },
     "DFC5A100-8C92-4809-8044-102AAAB62EEA": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": false,
         "Data ID": "DFC5A100-8C92-4809-8044-102AAAB62EEA",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Duration": "12",
         "Enabled": true,
         "Formula": "<ThresholdMetric>",
@@ -1036,27 +990,25 @@
                 "Unit Of Measure": "min",
                 "Value": 30
             },
             "Process Type": "Continuous"
         },
         "ID": "DFC5A100-8C92-4809-8044-102AAAB62EEA",
         "Name": "Rolling Temperature 12-hour Maximum",
-        "Path": null,
         "Period": "30",
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "ThresholdMetric",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "type": "threshold-metric"
         },
         "Unsearchable": false
     },
     "FBBCD4E0-CE26-4A33-BE59-3E215553FB1F": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "2f103966-3dc2-416d-bc01-f3f5290e8afd",
         "Cached By Service": true,
         "Data ID": "FBBCD4E0-CE26-4A33-BE59-3E215553FB1F",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -1065,15 +1017,14 @@
             "series": "9564A6B8-8A8F-4F6D-AC63-00EA38962B7A"
         },
         "ID": "FBBCD4E0-CE26-4A33-BE59-3E215553FB1F",
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "120.0",
         "Name": "Smooth Temperature",
-        "Path": null,
         "Scoped To": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
         "Type": "CalculatedSignal",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "autoPeriod": true,
             "autoTaps": true,
             "cutoff": {
```

#### Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Items.json

##### Pretty-printed

 * *Similarity: 0.9696969696969697%*

 * *Differences: {"'13830E96-9EAF-4F98-A303-6F05E23E95B3'": "{delete: ['Asset', 'Path']}",*

 * * "'C505586B-9AFE-430E-94E0-B03145AF8EFC'": "{delete: ['Asset', 'Path']}"}*

```diff
@@ -1,11 +1,10 @@
 {
     "13830E96-9EAF-4F98-A303-6F05E23E95B3": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "070c1c80-0245-4de3-a290-d702584829eb",
         "Cached By Service": true,
         "Data ID": "13830e96-9eaf-4f98-a303-6f05e23e95b3",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -13,15 +12,14 @@
         "Formula Parameters": {},
         "ID": "13830E96-9EAF-4F98-A303-6F05E23E95B3",
         "Key Unit Of Measure": "ns",
         "Maximum Duration": "1.0416666666666667",
         "Maximum Interpolation": "1.0416666666666667",
         "Metadata Properties": "Day+of+Year=&Day+of+Week=&Day+of+Month=",
         "Name": "Daily",
-        "Path": null,
         "Scoped To": "811B1488-297A-4FD2-AE7C-A1FE0E3B3641",
         "Type": "CalculatedCondition",
         "UIConfig": {
             "advancedParametersCollapsed": false,
             "duration": "days",
             "frequencies": [],
             "offset": {},
@@ -155,15 +153,14 @@
         },
         "Type": "Folder",
         "Unsearchable": false,
         "Updated At": "1571753347497016700"
     },
     "C505586B-9AFE-430E-94E0-B03145AF8EFC": {
         "Archived": false,
-        "Asset": null,
         "Cache Enabled": true,
         "Cache ID": "0ed8820a-e4a0-48a9-83f5-38839f2443db",
         "Cached By Service": true,
         "Data ID": "c505586b-9afe-430e-94e0-b03145af8efc",
         "Datasource Class": "Seeq Calculations",
         "Datasource ID": "Seeq Calculations",
         "Enabled": true,
@@ -171,15 +168,14 @@
         "Formula Parameters": {},
         "ID": "C505586B-9AFE-430E-94E0-B03145AF8EFC",
         "Key Unit Of Measure": "ns",
         "Maximum Duration": "1.0416666666666667",
         "Maximum Interpolation": "1.0416666666666667",
         "Metadata Properties": "Day+of+Year=&Day+of+Week=&Day+of+Month=",
         "Name": "Daily 2",
-        "Path": null,
         "Scoped To": "811B1488-297A-4FD2-AE7C-A1FE0E3B3641",
         "Type": "CalculatedCondition",
         "UIConfig": {
             "advancedParametersCollapsed": true,
             "duration": "days",
             "frequencies": [],
             "offset": {},
```

#### Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Report_50A98248-9FBB-4A28-BD3E-CEE434BD359D.json

##### Pretty-printed

 * *Similarity: 0.7904545454545454%*

 * *Differences: {"'Date Ranges'": "{0: {'Capsule Picker': OrderedDict([('Offset', 1), ('Reference', 'end'), "*

 * *                  "('Strategy', 'offsetBy')])}, 1: {'Capsule Picker': OrderedDict([('Offset', 1), "*

 * *                  "('Reference', 'end'), ('Strategy', 'closestTo')])}, 2: {'Capsule Picker': "*

 * *                  "OrderedDict([('Offset', 1), ('Reference', 'end'), ('Strategy', 'closestTo')])}, "*

 * *                  "3: {'Capsule Picker': OrderedDict([('Offset', 1), ('Reference', 'end'), "*

 * *                  "('Strategy […]*

```diff
@@ -81,50 +81,92 @@
     "Date Ranges": [
         {
             "Archived": false,
             "Auto Duration": "259200.0s",
             "Auto Enabled": true,
             "Auto Offset": "0min",
             "Auto Offset Direction": "Past",
+            "Capsule Picker": {
+                "Offset": 1,
+                "Reference": "end",
+                "Strategy": "offsetBy"
+            },
             "Condition ID": "13830E96-9EAF-4F98-A303-6F05E23E95B3",
             "Enabled": true,
             "ID": "9C76D056-4EB6-40ED-AF8E-44F5B4753277",
             "Name": "Yesterday",
             "Type": "DateRange"
         },
         {
             "Archived": false,
             "Auto Duration": "259200.0s",
             "Auto Enabled": true,
             "Auto Offset": "0min",
             "Auto Offset Direction": "Past",
+            "Capsule Picker": {
+                "Offset": 1,
+                "Reference": "end",
+                "Strategy": "closestTo"
+            },
             "Condition ID": "13830E96-9EAF-4F98-A303-6F05E23E95B3",
             "Enabled": true,
             "ID": "179D0B7D-BCD4-4221-A7CE-5F22526CB333",
             "Name": "Today",
             "Type": "DateRange"
         },
         {
             "Archived": false,
             "Auto Duration": "3600.0s",
             "Auto Enabled": true,
             "Auto Offset": "0min",
             "Auto Offset Direction": "Past",
+            "Capsule Picker": {
+                "Offset": 1,
+                "Reference": "end",
+                "Strategy": "closestTo"
+            },
             "Enabled": true,
             "ID": "41682646-A6E7-4ABB-B580-0ED45EC6D10D",
             "Name": "Last Hour",
             "Type": "DateRange"
         },
         {
             "Archived": false,
             "Auto Duration": "3600.0s",
             "Auto Enabled": true,
             "Auto Offset": "2h",
             "Auto Offset Direction": "Past",
+            "Capsule Picker": {
+                "Offset": 1,
+                "Reference": "end",
+                "Strategy": "closestTo"
+            },
             "Enabled": true,
             "ID": "82FF19E1-36A7-4A0D-A3E2-44141D8B4145",
             "Name": "Two Hours Ago",
             "Type": "DateRange"
         }
     ],
+    "Definition": {
+        "Archived": false,
+        "Average Run Time": "1883",
+        "Background": false,
+        "Cache Enabled": false,
+        "Condition Formula Now": "1654567505580100000",
+        "Created At": "1542832966647000000",
+        "Description": "Two Hours Ago: Today: Yesterday:",
+        "Document": "\n  <h1>Last Hour:</h1>\n  <p><img id=\"adae6720-8792-44d0-9ca5-5d769d306946\" data-seeq-content=\"3FADF54E-F8E5-43DB-A15B-611734A1D80E\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/3FADF54E-F8E5-43DB-A15B-611734A1D80E/image\" data-seeq-content-border=\"true\"></p>\n  <h1>Two Hours Ago:</h1>\n  <p><img id=\"18487ea1-c06e-5e05-f1e6-ea53b3c9c904\" data-seeq-content=\"3D2E5212-0CEB-4AB2-B2FD-605F402C8226\" class=\"report-image-border fr-dii\" src=\"/api/content/3D2E5212-0CEB-4AB2-B2FD-605F402C8226/image\" data-seeq-content-border=\"true\"><br></p>\n  <h1>Today:</h1>\n  <p><img id=\"3328a7c7-ad75-b405-6cf8-01e520c7f81f\" data-seeq-content=\"79F91706-A9DC-4B56-BA4E-461CC5339EF8\" class=\"report-image-border fr-dii\" src=\"/api/content/79F91706-A9DC-4B56-BA4E-461CC5339EF8/image\" data-seeq-content-border=\"true\"><br></p>\n  <h1>Yesterday:</h1>\n  <p><img id=\"f578a093-8a8e-69be-2d00-d0a5ca59c2db\" data-seeq-content=\"89399BEA-95F9-468C-8A8A-A0F89899C38B\" class=\"report-image-border fr-dii\" src=\"/api/content/89399BEA-95F9-468C-8A8A-A0F89899C38B/image\" data-seeq-content-border=\"true\"><br></p>\n ",
+        "DocumentBackup\u02c9mark.derbecker@seeq.com\u02c92020-07-31T23:03:00Z": "\n  <h1>Last Hour:</h1>\n  <p><a href=\"/api/content/3FADF54E-F8E5-43DB-A15B-611734A1D80E/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"adae6720-8792-44d0-9ca5-5d769d306946\" data-seeq-content=\"3FADF54E-F8E5-43DB-A15B-611734A1D80E\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/3FADF54E-F8E5-43DB-A15B-611734A1D80E/image\"></a></p>\n  <h1>Two Hours Ago:</h1>\n  <p><a href=\"/api/content/3D2E5212-0CEB-4AB2-B2FD-605F402C8226/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"18487ea1-c06e-5e05-f1e6-ea53b3c9c904\" data-seeq-content=\"3D2E5212-0CEB-4AB2-B2FD-605F402C8226\" class=\"report-image-border fr-dii\" src=\"/api/content/3D2E5212-0CEB-4AB2-B2FD-605F402C8226/image\"></a><br></p>\n  <h1>Today:</h1>\n  <p><a href=\"/api/content/79F91706-A9DC-4B56-BA4E-461CC5339EF8/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"3328a7c7-ad75-b405-6cf8-01e520c7f81f\" data-seeq-content=\"79F91706-A9DC-4B56-BA4E-461CC5339EF8\" class=\"report-image-border fr-dii\" src=\"/api/content/79F91706-A9DC-4B56-BA4E-461CC5339EF8/image\"></a><br></p>\n  <h1>Yesterday:</h1>\n  <p><a href=\"/api/content/89399BEA-95F9-468C-8A8A-A0F89899C38B/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"f578a093-8a8e-69be-2d00-d0a5ca59c2db\" data-seeq-content=\"89399BEA-95F9-468C-8A8A-A0F89899C38B\" class=\"report-image-border fr-dii\" src=\"/api/content/89399BEA-95F9-468C-8A8A-A0F89899C38B/image\"></a><br></p>\n ",
+        "Enabled": true,
+        "Froala Backup": "\n  <h1>Last Hour:</h1>\n  <p><a href=\"/api/content/3FADF54E-F8E5-43DB-A15B-611734A1D80E/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"adae6720-8792-44d0-9ca5-5d769d306946\" data-seeq-content=\"3FADF54E-F8E5-43DB-A15B-611734A1D80E\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/3FADF54E-F8E5-43DB-A15B-611734A1D80E/image\"></a></p>\n  <h1>Two Hours Ago:</h1>\n  <p><a href=\"/api/content/3D2E5212-0CEB-4AB2-B2FD-605F402C8226/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"18487ea1-c06e-5e05-f1e6-ea53b3c9c904\" data-seeq-content=\"3D2E5212-0CEB-4AB2-B2FD-605F402C8226\" class=\"report-image-border fr-dii\" src=\"/api/content/3D2E5212-0CEB-4AB2-B2FD-605F402C8226/image\"></a><br></p>\n  <h1>Today:</h1>\n  <p><a href=\"/api/content/79F91706-A9DC-4B56-BA4E-461CC5339EF8/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"3328a7c7-ad75-b405-6cf8-01e520c7f81f\" data-seeq-content=\"79F91706-A9DC-4B56-BA4E-461CC5339EF8\" class=\"report-image-border fr-dii\" src=\"/api/content/79F91706-A9DC-4B56-BA4E-461CC5339EF8/image\"></a><br></p>\n  <h1>Yesterday:</h1>\n  <p><a href=\"/api/content/89399BEA-95F9-468C-8A8A-A0F89899C38B/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"f578a093-8a8e-69be-2d00-d0a5ca59c2db\" data-seeq-content=\"89399BEA-95F9-468C-8A8A-A0F89899C38B\" class=\"report-image-border fr-dii\" src=\"/api/content/89399BEA-95F9-468C-8A8A-A0F89899C38B/image\"></a><br></p>\n ",
+        "ID": "39393625-5DC4-4626-A83B-2DD9A252830D",
+        "Is CK Enabled": true,
+        "Last Viewed At": "1674090780498000000",
+        "Name": "Last Hour:",
+        "Plain Text Document": "\n  Last Hour:\n  \n  Two Hours Ago:\n  \n  Today:\n  \n  Yesterday:\n  \n ",
+        "Total Run Time": "7535",
+        "Type": "Report",
+        "Unsearchable": false,
+        "Updated At": "1674090780000613200"
+    },
     "Schedule": null
 }
```

#### Example Topic (811B1488-297A-4FD2-AE7C-A1FE0E3B3641)/Report_E5B84916-5962-49A7-9987-052CF80CD077.json

##### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'Definition'": "OrderedDict([('Archived', False), ('Average Run Time', '1030'), ('Background', "*

 * *                 "False), ('Cache Enabled', False), ('Condition Formula Now', "*

 * *                 "'1654567505580100000'), ('Created At', '1541999834178000000'), ('Description', "*

 * *                 "'Worksheet Two: Worksheet Three: A Picture:'), ('Document', '\\n  <p>Worksheet "*

 * *                 'One:</p>\\n  <p><img id="43dbf173-16b9-267b-9727-c9d7b48ab07f" '*

 * *                 'data-seeq-content="EF9F18FC-FF98-4 […]*

```diff
@@ -56,9 +56,31 @@
             "Workbook ID": "D833DC83-9A38-48DE-BF45-EB787E9E8375",
             "Worksheet ID": "F255BF0D-CCE1-4021-B863-B121FB605913",
             "Workstep ID": "79B86A9F-43CE-47BD-9C29-8940BF6B5D6C",
             "selector": ""
         }
     ],
     "Date Ranges": [],
+    "Definition": {
+        "Archived": false,
+        "Average Run Time": "1030",
+        "Background": false,
+        "Cache Enabled": false,
+        "Condition Formula Now": "1654567505580100000",
+        "Created At": "1541999834178000000",
+        "Description": "Worksheet Two: Worksheet Three: A Picture:",
+        "Document": "\n  <p>Worksheet One:</p>\n  <p><img id=\"43dbf173-16b9-267b-9727-c9d7b48ab07f\" data-seeq-content=\"EF9F18FC-FF98-4B38-AE89-01D24EE208E6\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/EF9F18FC-FF98-4B38-AE89-01D24EE208E6/image\" data-seeq-content-border=\"true\"></p>\n  <p>Worksheet Two:</p>\n  <p><img id=\"52b8a26a-9de9-508e-d746-835ce5b868a4\" data-seeq-content=\"623F12D3-5A33-48A3-96F6-DE99F5914101\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/623F12D3-5A33-48A3-96F6-DE99F5914101/image\" data-seeq-content-border=\"true\"></p>\n  <p>Worksheet Three:</p>\n  <p><img id=\"ee0e57a0-f1dd-3ab1-9411-2d1c435e9745\" data-seeq-content=\"2DF4FC9C-3813-4D84-BFE5-53A9255D2015\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/2DF4FC9C-3813-4D84-BFE5-53A9255D2015/image\" data-seeq-content-border=\"true\"></p>\n  <p>A Picture:</p>\n  <p><img src=\"/api/annotations/CF590E20-AA52-441E-81E3-554C7F893FBA/images/1596236583342_v1.png\" class=\"fr-fic fr-fin fr-dii\"></p>\n  <p><br></p>\n ",
+        "DocumentBackup\u02c9mark.derbecker@seeq.com\u02c92020-07-31T23:03:00Z": "\n  <p>Worksheet One:</p>\n  <p><a href=\"/api/content/EF9F18FC-FF98-4B38-AE89-01D24EE208E6/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"43dbf173-16b9-267b-9727-c9d7b48ab07f\" data-seeq-content=\"EF9F18FC-FF98-4B38-AE89-01D24EE208E6\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/EF9F18FC-FF98-4B38-AE89-01D24EE208E6/image\"></a></p>\n  <p>Worksheet Two:</p>\n  <p><a href=\"/api/content/623F12D3-5A33-48A3-96F6-DE99F5914101/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"52b8a26a-9de9-508e-d746-835ce5b868a4\" data-seeq-content=\"623F12D3-5A33-48A3-96F6-DE99F5914101\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/623F12D3-5A33-48A3-96F6-DE99F5914101/image\"></a></p>\n  <p>Worksheet Three:</p>\n  <p><a href=\"/api/content/2DF4FC9C-3813-4D84-BFE5-53A9255D2015/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"ee0e57a0-f1dd-3ab1-9411-2d1c435e9745\" data-seeq-content=\"2DF4FC9C-3813-4D84-BFE5-53A9255D2015\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/2DF4FC9C-3813-4D84-BFE5-53A9255D2015/image\"></a></p>\n  <p>A Picture:</p>\n  <p><img src=\"/api/annotations/CF590E20-AA52-441E-81E3-554C7F893FBA/images/1596236583342_v1.png\" class=\"fr-fic fr-fin fr-dii\"></p>\n  <p><br></p>\n ",
+        "Enabled": true,
+        "Froala Backup": "\n  <p>Worksheet One:</p>\n  <p><a href=\"/api/content/EF9F18FC-FF98-4B38-AE89-01D24EE208E6/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"43dbf173-16b9-267b-9727-c9d7b48ab07f\" data-seeq-content=\"EF9F18FC-FF98-4B38-AE89-01D24EE208E6\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/EF9F18FC-FF98-4B38-AE89-01D24EE208E6/image\"></a></p>\n  <p>Worksheet Two:</p>\n  <p><a href=\"/api/content/623F12D3-5A33-48A3-96F6-DE99F5914101/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"52b8a26a-9de9-508e-d746-835ce5b868a4\" data-seeq-content=\"623F12D3-5A33-48A3-96F6-DE99F5914101\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/623F12D3-5A33-48A3-96F6-DE99F5914101/image\"></a></p>\n  <p>Worksheet Three:</p>\n  <p><a href=\"/api/content/2DF4FC9C-3813-4D84-BFE5-53A9255D2015/sourceUrl\" rel=\"nofollow noopener noreferrer\"><img id=\"ee0e57a0-f1dd-3ab1-9411-2d1c435e9745\" data-seeq-content=\"2DF4FC9C-3813-4D84-BFE5-53A9255D2015\" class=\"report-image-border fr-dii specReportSeeqContent\" src=\"/api/content/2DF4FC9C-3813-4D84-BFE5-53A9255D2015/image\"></a></p>\n  <p>A Picture:</p>\n  <p><img src=\"/api/annotations/CF590E20-AA52-441E-81E3-554C7F893FBA/images/1596236583342_v1.png\" class=\"fr-fic fr-fin fr-dii\"></p>\n  <p><br></p>\n ",
+        "ID": "CF590E20-AA52-441E-81E3-554C7F893FBA",
+        "Is CK Enabled": true,
+        "Last Viewed At": "1674090789643000000",
+        "Name": "Worksheet One:",
+        "Plain Text Document": "\n  Worksheet One:\n  \n  Worksheet Two:\n  \n  Worksheet Three:\n  \n  A Picture:\n  \n  \n ",
+        "Total Run Time": "3092",
+        "Type": "Report",
+        "Unsearchable": false,
+        "Updated At": "1674090765833123800"
+    },
     "Schedule": null
 }
```

#### Comparing `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_1DCFA3AF-77BD-4198-AA0C-C3F549BAA48A.json` & `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B_Workstep_1204D33F-257E-4CBD-A6A7-EFAF0D765749.json`

 * *Files 7% similar despite different names*

##### Pretty-printed

 * *Similarity: 0.8329613095238096%*

 * *Differences: {"'Data'": "{'state': {'stores': {'sqDurationStore': {'autoUpdate': {'offset': -1}, "*

 * *           "'displayRange': {'start': 1687581356319, 'end': 1687667756319}, 'investigateRange': "*

 * *           "{'start': 1687062956320, 'end': 1687667756320}}}}}",*

 * * "'ID'": "'1204D33F-257E-4CBD-A6A7-EFAF0D765749'"}*

```diff
@@ -1,22 +1,22 @@
 {
     "Data": {
         "state": {
             "stores": {
                 "sqDurationStore": {
                     "autoUpdate": {
-                        "offset": 0
+                        "offset": -1
                     },
                     "displayRange": {
-                        "end": 1681320554179,
-                        "start": 1681234154178
+                        "end": 1687667756319,
+                        "start": 1687581356319
                     },
                     "investigateRange": {
-                        "end": 1681320554179,
-                        "start": 1680715754179
+                        "end": 1687667756320,
+                        "start": 1687062956320
                     }
                 },
                 "sqTrendCapsuleSetStore": {
                     "items": []
                 },
                 "sqTrendMetricStore": {
                     "items": []
@@ -33,10 +33,10 @@
                 "sqWorksheetStore": {
                     "viewKey": "TREND"
                 }
             }
         },
         "version": 1
     },
-    "ID": "1DCFA3AF-77BD-4198-AA0C-C3F549BAA48A",
+    "ID": "1204D33F-257E-4CBD-A6A7-EFAF0D765749",
     "Type": "Workstep"
 }
```

#### Comparing `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_B364236F-3815-4E3F-A4C2-FDF636A2D313.json` & `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_F255BF0D-CCE1-4021-B863-B121FB605913_Workstep_385CF8DA-B5DF-42CE-BA05-BABE20B21F20.json`

 * *Files 9% similar despite different names*

##### Pretty-printed

 * *Similarity: 0.8329613095238096%*

 * *Differences: {"'Data'": "{'state': {'stores': {'sqDurationStore': {'autoUpdate': {'offset': -1976}, "*

 * *           "'displayRange': {'start': 1687581354071, 'end': 1687667754071}, 'investigateRange': "*

 * *           "{'start': 1687062956047, 'end': 1687667756047}}}}}",*

 * * "'ID'": "'385CF8DA-B5DF-42CE-BA05-BABE20B21F20'"}*

```diff
@@ -1,22 +1,22 @@
 {
     "Data": {
         "state": {
             "stores": {
                 "sqDurationStore": {
                     "autoUpdate": {
-                        "offset": 0
+                        "offset": -1976
                     },
                     "displayRange": {
-                        "end": 1681320554067,
-                        "start": 1681234154067
+                        "end": 1687667754071,
+                        "start": 1687581354071
                     },
                     "investigateRange": {
-                        "end": 1681320554067,
-                        "start": 1680715754067
+                        "end": 1687667756047,
+                        "start": 1687062956047
                     }
                 },
                 "sqTrendCapsuleSetStore": {
                     "items": []
                 },
                 "sqTrendMetricStore": {
                     "items": []
@@ -33,10 +33,10 @@
                 "sqWorksheetStore": {
                     "viewKey": "TREND"
                 }
             }
         },
         "version": 1
     },
-    "ID": "B364236F-3815-4E3F-A4C2-FDF636A2D313",
+    "ID": "385CF8DA-B5DF-42CE-BA05-BABE20B21F20",
     "Type": "Workstep"
 }
```

#### Comparing `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_44A42737-E20C-4BCE-BB50-4F2468C7419D_Workstep_5366156C-07CB-4724-9C18-41AA8123B939.json` & `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_10198C29-C93C-4055-B313-3388227D0621_Workstep_7951145D-AA2F-4196-8422-39335A5C5C59.json`

 * *Files 7% similar despite different names*

##### Pretty-printed

 * *Similarity: 0.8329613095238096%*

 * *Differences: {"'Data'": "{'state': {'stores': {'sqDurationStore': {'autoUpdate': {'offset': -1}, "*

 * *           "'displayRange': {'start': 1687581356264, 'end': 1687667756264}, 'investigateRange': "*

 * *           "{'start': 1687062956265, 'end': 1687667756265}}}}}",*

 * * "'ID'": "'7951145D-AA2F-4196-8422-39335A5C5C59'"}*

```diff
@@ -1,22 +1,22 @@
 {
     "Data": {
         "state": {
             "stores": {
                 "sqDurationStore": {
                     "autoUpdate": {
-                        "offset": 0
+                        "offset": -1
                     },
                     "displayRange": {
-                        "end": 1681320554251,
-                        "start": 1681234154251
+                        "end": 1687667756264,
+                        "start": 1687581356264
                     },
                     "investigateRange": {
-                        "end": 1681320554251,
-                        "start": 1680715754251
+                        "end": 1687667756265,
+                        "start": 1687062956265
                     }
                 },
                 "sqTrendCapsuleSetStore": {
                     "items": []
                 },
                 "sqTrendMetricStore": {
                     "items": []
@@ -33,10 +33,10 @@
                 "sqWorksheetStore": {
                     "viewKey": "TREND"
                 }
             }
         },
         "version": 1
     },
-    "ID": "5366156C-07CB-4724-9C18-41AA8123B939",
+    "ID": "7951145D-AA2F-4196-8422-39335A5C5C59",
     "Type": "Workstep"
 }
```

#### Comparing `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB_Workstep_8CD6F7D5-8358-4725-A39B-E68B47D9D1BB.json` & `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_99E1E62B-69F1-4FFB-8649-3225820A7DFB_Workstep_4D8421AB-A1C0-42FF-B114-3749BC6753D1.json`

 * *Files 16% similar despite different names*

##### Pretty-printed

 * *Similarity: 0.8330853174603176%*

 * *Differences: {"'Data'": "{'state': {'stores': {'sqDurationStore': {'displayRange': {'start': 1687581356221, "*

 * *           "'end': 1687667756221}, 'investigateRange': {'start': 1687062956221, 'end': "*

 * *           '1687667756221}}}}}',*

 * * "'ID'": "'4D8421AB-A1C0-42FF-B114-3749BC6753D1'"}*

```diff
@@ -3,20 +3,20 @@
         "state": {
             "stores": {
                 "sqDurationStore": {
                     "autoUpdate": {
                         "offset": 0
                     },
                     "displayRange": {
-                        "end": 1681320554147,
-                        "start": 1681234154147
+                        "end": 1687667756221,
+                        "start": 1687581356221
                     },
                     "investigateRange": {
-                        "end": 1681320554147,
-                        "start": 1680715754147
+                        "end": 1687667756221,
+                        "start": 1687062956221
                     }
                 },
                 "sqTrendCapsuleSetStore": {
                     "items": []
                 },
                 "sqTrendMetricStore": {
                     "items": []
@@ -33,10 +33,10 @@
                 "sqWorksheetStore": {
                     "viewKey": "TREND"
                 }
             }
         },
         "version": 1
     },
-    "ID": "8CD6F7D5-8358-4725-A39B-E68B47D9D1BB",
+    "ID": "4D8421AB-A1C0-42FF-B114-3749BC6753D1",
     "Type": "Workstep"
 }
```

#### Comparing `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_15B8DB00-1095-4560-BA40-DA7E23A9AFC1.json` & `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_BFB529B8-F127-49FC-81B3-55BCCE4CC2B1_Workstep_E31E275F-8295-43A7-9FC2-E66711C407E8.json`

 * *Files 16% similar despite different names*

##### Pretty-printed

 * *Similarity: 0.8330853174603176%*

 * *Differences: {"'Data'": "{'state': {'stores': {'sqDurationStore': {'displayRange': {'start': 1687581356172, "*

 * *           "'end': 1687667756172}, 'investigateRange': {'start': 1687062956173, 'end': "*

 * *           '1687667756173}}}}}',*

 * * "'ID'": "'E31E275F-8295-43A7-9FC2-E66711C407E8'"}*

```diff
@@ -3,20 +3,20 @@
         "state": {
             "stores": {
                 "sqDurationStore": {
                     "autoUpdate": {
                         "offset": -1
                     },
                     "displayRange": {
-                        "end": 1681320554107,
-                        "start": 1681234154107
+                        "end": 1687667756172,
+                        "start": 1687581356172
                     },
                     "investigateRange": {
-                        "end": 1681320554108,
-                        "start": 1680715754108
+                        "end": 1687667756173,
+                        "start": 1687062956173
                     }
                 },
                 "sqTrendCapsuleSetStore": {
                     "items": []
                 },
                 "sqTrendMetricStore": {
                     "items": []
@@ -33,10 +33,10 @@
                 "sqWorksheetStore": {
                     "viewKey": "TREND"
                 }
             }
         },
         "version": 1
     },
-    "ID": "15B8DB00-1095-4560-BA40-DA7E23A9AFC1",
+    "ID": "E31E275F-8295-43A7-9FC2-E66711C407E8",
     "Type": "Workstep"
 }
```

#### Comparing `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_D978C84E-9435-422F-9C1A-DC4C7E515C0B_Workstep_B66A34BE-1B59-4064-9E87-625808FC4146.json` & `Example Analysis (D833DC83-9A38-48DE-BF45-EB787E9E8375)/Worksheet_1F02C6C7-5009-4A13-9343-CDDEBB6AF7E6_Workstep_D1827683-15C9-4194-A52A-6ADADBB2AF28.json`

 * *Files 16% similar despite different names*

##### Pretty-printed

 * *Similarity: 0.8330853174603176%*

 * *Differences: {"'Data'": "{'state': {'stores': {'sqDurationStore': {'displayRange': {'start': 1687581356121, "*

 * *           "'end': 1687667756121}, 'investigateRange': {'start': 1687062956121, 'end': "*

 * *           '1687667756121}}}}}',*

 * * "'ID'": "'D1827683-15C9-4194-A52A-6ADADBB2AF28'"}*

```diff
@@ -3,20 +3,20 @@
         "state": {
             "stores": {
                 "sqDurationStore": {
                     "autoUpdate": {
                         "offset": 0
                     },
                     "displayRange": {
-                        "end": 1681320554220,
-                        "start": 1681234154220
+                        "end": 1687667756121,
+                        "start": 1687581356121
                     },
                     "investigateRange": {
-                        "end": 1681320554220,
-                        "start": 1680715754220
+                        "end": 1687667756121,
+                        "start": 1687062956121
                     }
                 },
                 "sqTrendCapsuleSetStore": {
                     "items": []
                 },
                 "sqTrendMetricStore": {
                     "items": []
@@ -33,10 +33,10 @@
                 "sqWorksheetStore": {
                     "viewKey": "TREND"
                 }
             }
         },
         "version": 1
     },
-    "ID": "B66A34BE-1B59-4064-9E87-625808FC4146",
+    "ID": "D1827683-15C9-4194-A52A-6ADADBB2AF28",
     "Type": "Workstep"
 }
```

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 111771 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat      564 b- defN 23-Apr-12 10:29 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Datasources.json
--rw-rw-rw-  2.0 fat     1023 b- defN 23-Apr-12 10:29 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Datasource_Map_Auth_Seeq_Seeq.json
--rw-rw-rw-  2.0 fat      686 b- defN 23-Apr-12 10:29 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Datasource_Map_Time Series CSV Files_Example Data_Example Data.json
--rw-rw-rw-  2.0 fat    36190 b- defN 23-Apr-12 10:29 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Image_04FD9A9F-496F-483C-9349-4D76593E1525_istockphoto-93385233-612x612_v1.jpg
--rw-rw-rw-  2.0 fat     8338 b- defN 23-Apr-12 10:29 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Items.json
--rw-rw-rw-  2.0 fat      770 b- defN 23-Apr-12 10:29 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Journal_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648.html
--rw-rw-rw-  2.0 fat     3667 b- defN 23-Apr-12 10:29 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Workbook.json
--rw-rw-rw-  2.0 fat      587 b- defN 23-Apr-12 10:29 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648.json
--rw-rw-rw-  2.0 fat     1243 b- defN 23-Apr-12 10:29 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648_Workstep_2A224704-ADB3-4D08-8265-400B95B479F2.json
--rw-rw-rw-  2.0 fat    30175 b- defN 23-Apr-12 10:29 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648_Workstep_39AF2F17-938C-4FF7-A7E1-EE10665C763C.json
--rw-rw-rw-  2.0 fat      267 b- defN 23-Apr-12 10:29 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Datasources.json
--rw-rw-rw-  2.0 fat     1023 b- defN 23-Apr-12 10:29 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Datasource_Map_Auth_Seeq_Seeq.json
--rw-rw-rw-  2.0 fat    62414 b- defN 23-Apr-12 10:29 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Image_F5E5AEF1-D56B-41B9-881A-EC4A2EF52A67_company_logo_v1.png
--rw-rw-rw-  2.0 fat     4968 b- defN 23-Apr-12 10:29 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Items.json
--rw-rw-rw-  2.0 fat      867 b- defN 23-Apr-12 10:29 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Report_4DD085C0-E751-4715-A907-67B0CE7D7C29.html
--rw-rw-rw-  2.0 fat     1409 b- defN 23-Apr-12 10:29 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Report_4DD085C0-E751-4715-A907-67B0CE7D7C29.json
--rw-rw-rw-  2.0 fat     3230 b- defN 23-Apr-12 10:29 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Workbook.json
--rw-rw-rw-  2.0 fat      531 b- defN 23-Apr-12 10:29 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Worksheet_4DD085C0-E751-4715-A907-67B0CE7D7C29.json
-18 files, 157952 bytes uncompressed, 106789 bytes compressed:  32.4%
+Zip file size: 113732 bytes, number of entries: 19
+-rw-rw-rw-  2.0 fat      564 b- defN 23-Jun-24 21:36 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Datasources.json
+-rw-rw-rw-  2.0 fat     1023 b- defN 23-Jun-24 21:36 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Datasource_Map_Auth_Seeq_Seeq.json
+-rw-rw-rw-  2.0 fat      686 b- defN 23-Jun-24 21:36 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Datasource_Map_Time Series CSV Files_Example Data_Example Data.json
+-rw-rw-rw-  2.0 fat    36190 b- defN 23-Jun-24 21:36 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Image_04FD9A9F-496F-483C-9349-4D76593E1525_istockphoto-93385233-612x612_v1.jpg
+-rw-rw-rw-  2.0 fat     8384 b- defN 23-Jun-24 21:36 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Items.json
+-rw-rw-rw-  2.0 fat      770 b- defN 23-Jun-24 21:36 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Journal_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648.html
+-rw-rw-rw-  2.0 fat     4263 b- defN 23-Jun-24 21:36 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Journal_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648.json
+-rw-rw-rw-  2.0 fat     3667 b- defN 23-Jun-24 21:36 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Workbook.json
+-rw-rw-rw-  2.0 fat      587 b- defN 23-Jun-24 21:36 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648.json
+-rw-rw-rw-  2.0 fat    30175 b- defN 23-Jun-24 21:36 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648_Workstep_39AF2F17-938C-4FF7-A7E1-EE10665C763C.json
+-rw-rw-rw-  2.0 fat     1242 b- defN 23-Jun-24 21:36 Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648_Workstep_3CC234F4-2F6B-42ED-8A64-4A012FD4FEC6.json
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-24 21:36 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Datasources.json
+-rw-rw-rw-  2.0 fat     1023 b- defN 23-Jun-24 21:36 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Datasource_Map_Auth_Seeq_Seeq.json
+-rw-rw-rw-  2.0 fat    62414 b- defN 23-Jun-24 21:36 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Image_F5E5AEF1-D56B-41B9-881A-EC4A2EF52A67_company_logo_v1.png
+-rw-rw-rw-  2.0 fat     4968 b- defN 23-Jun-24 21:36 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Items.json
+-rw-rw-rw-  2.0 fat      867 b- defN 23-Jun-24 21:36 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Report_4DD085C0-E751-4715-A907-67B0CE7D7C29.html
+-rw-rw-rw-  2.0 fat     5911 b- defN 23-Jun-24 21:36 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Report_4DD085C0-E751-4715-A907-67B0CE7D7C29.json
+-rw-rw-rw-  2.0 fat     3230 b- defN 23-Jun-24 21:36 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Workbook.json
+-rw-rw-rw-  2.0 fat      531 b- defN 23-Jun-24 21:36 Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Worksheet_4DD085C0-E751-4715-A907-67B0CE7D7C29.json
+19 files, 166762 bytes uncompressed, 108462 bytes compressed:  35.0%
```

#### zipnote {}

```diff
@@ -12,24 +12,27 @@
 
 Filename: Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Items.json
 Comment: 
 
 Filename: Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Journal_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648.html
 Comment: 
 
+Filename: Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Journal_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648.json
+Comment: 
+
 Filename: Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Workbook.json
 Comment: 
 
 Filename: Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648.json
 Comment: 
 
-Filename: Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648_Workstep_2A224704-ADB3-4D08-8265-400B95B479F2.json
+Filename: Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648_Workstep_39AF2F17-938C-4FF7-A7E1-EE10665C763C.json
 Comment: 
 
-Filename: Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648_Workstep_39AF2F17-938C-4FF7-A7E1-EE10665C763C.json
+Filename: Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648_Workstep_3CC234F4-2F6B-42ED-8A64-4A012FD4FEC6.json
 Comment: 
 
 Filename: Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Datasources.json
 Comment: 
 
 Filename: Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Datasource_Map_Auth_Seeq_Seeq.json
 Comment:
```

#### Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Items.json

##### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'4B40EAFC-91ED-4AB0-8199-F21AF40A8350'": "{'Asset': 'Area A', 'Path': 'Example >> Cooling Tower "*

 * *                                           "1', 'Sync Token': '2023-06-25T04:26:23.032018300Z', "*

 * *                                           "'Old Asset Format': False}",*

 * * "'8A4F0E26-8A0C-4127-9E11-B67E031C6049'": "{'Sync Token': '2023-06-25T04:26:23.032018300Z'}",*

 * * "'B9CDE282-7A1A-4E28-A173-12E7347AB891'": "{'Sync Token': '2023-06-25T04:26:23.032018300Z'}",*

 * * "'E97BBE1D-F227-4AD7-ADAC-15B54FC50DB3'": "{'Sync  […]*

```diff
@@ -126,24 +126,25 @@
         "Type": "Folder",
         "Unmodifiable": true,
         "Unsearchable": true,
         "Updated At": "1654313433632766100"
     },
     "4B40EAFC-91ED-4AB0-8199-F21AF40A8350": {
         "Archived": false,
-        "Asset": "Cooling Tower 1",
+        "Asset": "Area A",
         "Cache Enabled": false,
         "Data ID": "root/Cooling Tower 1/Area A",
         "Datasource Class": "Time Series CSV Files",
         "Datasource ID": "Example Data",
         "Enabled": true,
         "ID": "4B40EAFC-91ED-4AB0-8199-F21AF40A8350",
         "Name": "Area A",
-        "Path": "Example",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Old Asset Format": false,
+        "Path": "Example >> Cooling Tower 1",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "Asset",
         "Unsearchable": false
     },
     "8A4F0E26-8A0C-4127-9E11-B67E031C6049": {
         "Archived": false,
         "Asset": "Area A",
         "Cache Enabled": false,
@@ -157,15 +158,15 @@
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2min",
         "Name": "Temperature",
         "Path": "Example >> Cooling Tower 1",
         "Source Maximum Interpolation": "2min",
         "Source Value Unit Of Measure": "\u00b0F",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "StoredSignal",
         "Unsearchable": false,
         "Value Unit Of Measure": "\u00b0F"
     },
     "B9CDE282-7A1A-4E28-A173-12E7347AB891": {
         "Archived": false,
         "Asset": "Area A",
@@ -180,15 +181,15 @@
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2min",
         "Name": "Relative Humidity",
         "Path": "Example >> Cooling Tower 1",
         "Source Maximum Interpolation": "2min",
         "Source Value Unit Of Measure": "%",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "StoredSignal",
         "Unsearchable": false,
         "Value Unit Of Measure": "%"
     },
     "E97BBE1D-F227-4AD7-ADAC-15B54FC50DB3": {
         "Archived": false,
         "Asset": "Area A",
@@ -203,13 +204,13 @@
         "Interpolation Method": "Linear",
         "Key Unit Of Measure": "ns",
         "Maximum Interpolation": "2min",
         "Name": "Compressor Power",
         "Path": "Example >> Cooling Tower 1",
         "Source Maximum Interpolation": "2min",
         "Source Value Unit Of Measure": "kW",
-        "Sync Token": "2023-04-12T17:01:39.766440500Z",
+        "Sync Token": "2023-06-25T04:26:23.032018300Z",
         "Type": "StoredSignal",
         "Unsearchable": false,
         "Value Unit Of Measure": "kW"
     }
 }
```

#### Topic Template (14079DF9-319F-4181-AEC1-9A4D48EF310B)/Report_4DD085C0-E751-4715-A907-67B0CE7D7C29.json

##### Pretty-printed

 * *Similarity: 0.79%*

 * *Differences: {"'Date Ranges'": "{0: {'Capsule Picker': OrderedDict([('Offset', 1), ('Reference', 'end'), "*

 * *                  "('Strategy', 'closestTo')])}}",*

 * * "'Definition'": "OrderedDict([('Archived', False), ('Average Run Time', '1318'), ('Background', "*

 * *                 "False), ('Cache Enabled', False), ('Condition Formula Now', "*

 * *                 "'1655956010011169700'), ('Created At', '1655947868715233400'), ('Cron Schedule', "*

 * *                 "'*/5 * * * * ?'), ('Description', '{{facility}} {{#sections}} Section […]*

```diff
@@ -24,20 +24,52 @@
     "Date Ranges": [
         {
             "Archived": false,
             "Auto Duration": "172800.0s",
             "Auto Enabled": true,
             "Auto Offset": "0min",
             "Auto Offset Direction": "Past",
+            "Capsule Picker": {
+                "Offset": 1,
+                "Reference": "end",
+                "Strategy": "closestTo"
+            },
             "Enabled": true,
             "ID": "58A15610-579B-4A74-A592-4ADE162053EC",
             "Name": "Last Two Days Live",
             "Type": "DateRange"
         }
     ],
+    "Definition": {
+        "Archived": false,
+        "Average Run Time": "1318",
+        "Background": false,
+        "Cache Enabled": false,
+        "Condition Formula Now": "1655956010011169700",
+        "Created At": "1655947868715233400",
+        "Cron Schedule": "*/5 * * * * ?",
+        "Description": "{{facility}} {{#sections}} Section {{section}} {{/sections}}",
+        "Document": "<figure class=\"table\"><table><tbody><tr><td style=\"background-color:#DDDDDD;\">\u00a0</td><td style=\"background-color:#DDDDDD;\"><h2 style=\"text-align:center;\"><strong>Facility {<!-- -->{facility}}</strong></h2></td><td style=\"background-color:#DDDDDD;\"><figure class=\"image image_resized\" style=\"width:42.85%;\"><img src=\"/api/annotations/F5E5AEF1-D56B-41B9-881A-EC4A2EF52A67/images/company_logo_v1.png\"></figure></td></tr></tbody></table></figure><p style=\"text-align:center;\">{<!-- -->{#sections}}</p><h3 style=\"text-align:center;\">Section {<!-- -->{section}}</h3><p style=\"text-align:center;\"><img data-seeq-content=\"BFA05D82-D900-44B0-95C8-4AE8B26F01BE\" src=\"/api/content/BFA05D82-D900-44B0-95C8-4AE8B26F01BE/image\" data-seeq-content-width=\"1050\" data-seeq-content-height=\"591\" data-seeq-content-border=\"true\"></p><p style=\"text-align:center;\">{<!-- -->{/sections}}</p>",
+        "DocumentBackup\u02c9mark.derbecker@seeq.com\u02c92022-06-23T01:31:00Z": "<figure class=\"table\"><table><tbody><tr><td>\u00a0</td><td>\u00a0</td><td>\u00a0</td></tr></tbody></table></figure>",
+        "DocumentBackup\u02c9mark.derbecker@seeq.com\u02c92022-06-23T01:32:00Z": "<figure class=\"table\"><table><tbody><tr><td>\u00a0</td><td><h2>\u00a0</h2></td><td>\u00a0</td></tr></tbody></table></figure>",
+        "DocumentBackup\u02c9mark.derbecker@seeq.com\u02c92022-06-23T01:33:00Z": "<figure class=\"table\"><table><tbody><tr><td>\u00a0</td><td><h2 style=\"text-align:center;\"><strong>Facility {<!-- -->{facility</strong></h2></td><td>\u00a0</td></tr></tbody></table></figure>",
+        "DocumentBackup\u02c9mark.derbecker@seeq.com\u02c92022-06-23T01:34:00Z": "<figure class=\"table\"><table><tbody><tr><td>\u00a0</td><td><h2 style=\"text-align:center;\"><span style=\"background-color:hsl(30, 75%, 60%);\"><strong>Facility {<!-- -->{facility}}</strong></span></h2></td><td><figure class=\"image image_resized\" style=\"width:42.85%;\"><img src=\"/api/annotations/F5E5AEF1-D56B-41B9-881A-EC4A2EF52A67/images/company_logo_v1.png\"></figure></td></tr></tbody></table></figure>",
+        "DocumentBackup\u02c9mark.derbecker@seeq.com\u02c92022-06-23T01:35:00Z": "<figure class=\"table\"><table><tbody><tr><td style=\"background-color:#DDDDDD;\">\u00a0</td><td style=\"background-color:#DDDDDD;\"><h2 style=\"text-align:center;\"><strong>Facility {<!-- -->{facility}}</strong></h2></td><td style=\"background-color:#DDDDDD;\"><figure class=\"image image_resized\" style=\"width:42.85%;\"><img src=\"/api/annotations/F5E5AEF1-D56B-41B9-881A-EC4A2EF52A67/images/company_logo_v1.png\"></figure></td></tr></tbody></table></figure><p style=\"text-align:center;\">\u00a0</p>",
+        "DocumentBackup\u02c9mark.derbecker@seeq.com\u02c92022-06-23T01:37:00Z": "<figure class=\"table\"><table><tbody><tr><td style=\"background-color:#DDDDDD;\">\u00a0</td><td style=\"background-color:#DDDDDD;\"><h2 style=\"text-align:center;\"><strong>Facility {<!-- -->{facility}}</strong></h2></td><td style=\"background-color:#DDDDDD;\"><figure class=\"image image_resized\" style=\"width:42.85%;\"><img src=\"/api/annotations/F5E5AEF1-D56B-41B9-881A-EC4A2EF52A67/images/company_logo_v1.png\"></figure></td></tr></tbody></table></figure><p style=\"text-align:center;\">{<!-- -->{#areas}}</p><h3 style=\"text-align:center;\">Area {<!-- -->{area}}</h3><p style=\"text-align:center;\">\u00a0</p><p style=\"text-align:center;\">{<!-- -->{/areas}}</p>",
+        "Enabled": true,
+        "ID": "F5E5AEF1-D56B-41B9-881A-EC4A2EF52A67",
+        "Is CK Enabled": true,
+        "Last Viewed At": "1655955791501000000",
+        "Name": "Facility {{facility}}",
+        "Plain Text Document": "\u00a0Facility {<!-- -->{facility}}{<!-- -->{#sections}}Section {<!-- -->{section}}{<!-- -->{/sections}}",
+        "Total Run Time": "1318",
+        "Type": "Report",
+        "Unsearchable": false,
+        "Updated At": "1655954031086217200"
+    },
     "Schedule": {
         "Background": false,
         "Cron Schedule": [
             "*/5 * * * * ?"
         ]
     }
 }
```

#### Comparing `Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648_Workstep_2A224704-ADB3-4D08-8265-400B95B479F2.json` & `Analysis Template (FADE0364-E39C-41AD-BA33-95198583B63D)/Worksheet_86DACAC6-9BDA-4B54-A3CF-0C29C37E0648_Workstep_3CC234F4-2F6B-42ED-8A64-4A012FD4FEC6.json`

 * *Files 19% similar despite different names*

##### Pretty-printed

 * *Similarity: 0.8329613095238096%*

 * *Differences: {"'Data'": "{'state': {'stores': {'sqDurationStore': {'autoUpdate': {'offset': 0}, 'displayRange': "*

 * *           "{'start': 1687581367988, 'end': 1687667767988}, 'investigateRange': {'start': "*

 * *           "1687062967988, 'end': 1687667767988}}}}}",*

 * * "'ID'": "'3CC234F4-2F6B-42ED-8A64-4A012FD4FEC6'"}*

```diff
@@ -1,22 +1,22 @@
 {
     "Data": {
         "state": {
             "stores": {
                 "sqDurationStore": {
                     "autoUpdate": {
-                        "offset": -1
+                        "offset": 0
                     },
                     "displayRange": {
-                        "end": 1681320562603,
-                        "start": 1681234162603
+                        "end": 1687667767988,
+                        "start": 1687581367988
                     },
                     "investigateRange": {
-                        "end": 1681320562604,
-                        "start": 1680715762604
+                        "end": 1687667767988,
+                        "start": 1687062967988
                     }
                 },
                 "sqTrendCapsuleSetStore": {
                     "items": []
                 },
                 "sqTrendMetricStore": {
                     "items": []
@@ -33,10 +33,10 @@
                 "sqWorksheetStore": {
                     "viewKey": "TREND"
                 }
             }
         },
         "version": 1
     },
-    "ID": "2A224704-ADB3-4D08-8265-400B95B479F2",
+    "ID": "3CC234F4-2F6B-42ED-8A64-4A012FD4FEC6",
     "Type": "Workstep"
 }
```

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Tutorial.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Tutorial.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959296218487395%*

 * *Differences: {"'cells'": "{16: {'metadata': {replace: OrderedDict([('keep_output_in_docs', True)])}}, 18: "*

 * *            "{'metadata': {replace: OrderedDict([('keep_output_in_docs', True)])}}, 21: "*

 * *            "{'metadata': {replace: OrderedDict([('keep_output_in_docs', True)])}}, 27: "*

 * *            "{'metadata': {replace: OrderedDict([('keep_output_in_docs', True)])}}, 30: "*

 * *            "{'metadata': {replace: OrderedDict([('keep_output_in_docs', True)])}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.8.10'}}"}*

```diff
@@ -502,15 +502,17 @@
                 "## Plotting the Results\n",
                 "Let's take a quick peek at the data we just pulled using the built in `DataFrame.plot()` function."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "metadata": {},
+            "metadata": {
+                "keep_output_in_docs": true
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<AxesSubplot:>"
                         ]
                     },
@@ -547,15 +549,17 @@
                 "\n",
                 "How about a matrix of scatterplots, with each variable plotted against each other? Pandas can do that easily."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
-            "metadata": {},
+            "metadata": {
+                "keep_output_in_docs": true
+            },
             "outputs": [
                 {
                     "data": {
                         "image/png": "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nXfeWcm3ICIiIiIiIjIrKhqg33PPPTzyyCN8//vf54tf/CLr16/niiuu4IorruCSSy4hGAweVzkdHR08/fTTh31s2bJlPPHEE5VstoiIiIiIiMisq2iAftNNN3HTTTcBpV7wRx99lB/84Ae89a1vxTTNiiy/JiIiIiIiIjIfVTxJ3MjICA8//DAPPfQQDz30EFu3bqWqqopLL7200lWJiIiIiIiIzBsVDdDPOecctm3bRlVVFZdddhl/8Ad/wOWXX86aNWsqWY2IiIjMEzsGUmztSxILerh4US1ed0Xz14qInJT+RIan94zic7u4ZEktYV/F+zVFDqviSeIuv/xyVq9eXcliRUREZB4aTGX55Uv7sR0HAMtyuGZlwyy3SkTOdtmCxY+e6yVXsAFIZgq8Z2PbLLdKzhYVDdD/6I/+qPx/Z+pgaxhGJasQERGReWI8XSgH5wCj6fwstkZEpGQyVywH5wAjk9o3yelT8XFk3/nOdzjnnHMIBAIEAgHWrFnDv//7v1e6GhERETnDtVYFiPgP9BUsb4zMYmtEREriQS+NMX/5tvZNcjpVtAf9a1/7Gn/2Z3/Gxz/+cS6++GIAHnvsMT760Y8yPDzMpz71qUpWJyIiImewoNfN+85vZ+/wJLGAh7bq41uOVUTkVHKZBjdvaGXn4ARet8miutBsN0nOIhUN0L/xjW/w93//99xyyy3l+2688UZWrVrFl770JQXoIiIiMkPY52Z1S2y2myEiMoPXbbKyOTrbzZCzUEWHuPf393PRRRcdcv9FF11Ef39/JasSERERERERmVcqGqAvXryYu+6665D7//M//5MlS5ZUsioRERERERGReaWiQ9y//OUv8973vpdHHnmkPAf9d7/7Hb/5zW8OG7iLiIiIiIiISElFe9Bvvvlmnn76aWpra/nxj3/Mj3/8Y2pra3n66ad5xzveUcmqREREREREROaVivWgJ5NJnnrqKfL5PH/zN39DXV1dpYoWERERERERmfcqEqA///zzvOUtb2FgYADHcYhEItx1111cf/31lSheREREREREZN6ryBD3z372syxYsIDHHnuMzZs3c/XVV/Pxj3+8EkWLiIiIiIiInBUq0oO+efNm7rvvPjZs2ADAv/7rv1JdXU0ymSQa1fqBIiIiIiIiIsdSkR700dFRWltby7fj8TihUIiRkZFKFC8iIiIiIiIy71UsSdwrr7zC/v37y7cdx2Hbtm2kUqnyfWvWrKlUdSIiIiIiIiLzSsUC9KuvvhrHcWbc99a3vhXDMHAcB8MwsCyrUtWJiIiIiIiIzCsVCdD37NlTiWJEREREREREzloVCdA7OjoqUYyIiIiIiIjIWasiSeJERERERERE5I1RgC4iIiIiIiIyByhAFxEREREREZkDKhagO45DV1cX2Wy2UkWKiIiIiIiInDUqGqAvXryY7u7uShUpIiIiIiIictaoWIBumiZLlixhZGSkUkWKiIiIiIiInDUqOgf9q1/9Kn/6p3/Kyy+/XMliRUREREREROa9iqyDPu2WW24hnU6zdu1avF4vgUBgxuOjo6OVrE5ERERERERk3qhogP63f/u3lSxORERERERE5KxR0QD91ltvrWRxIiIiIiIiImeNigboAJZl8eMf/5ht27YBsGrVKm688UZcLlelqxIRERERERGZNyoaoO/cuZO3vOUt9Pb2smzZMgDuuOMO2tra+MUvfsGiRYsqWZ2IiIiIiIjIvFHRLO6f+MQnWLRoEd3d3WzZsoUtW7bQ1dXFggUL+MQnPlHJqkRERERERETmlYr2oD/88MM8+eSTVFdXl++rqanhq1/9KhdffHElqxIRERERERGZVyrag+7z+UilUofcPzExgdfrrWRVIiIiIiIiIvNKRQP0t771rXzkIx/hqaeewnEcHMfhySef5KMf/Sg33nhjJasSERERERERmVcqGqD/3d/9HYsWLeLCCy/E7/fj9/u5+OKLWbx4MV//+tcrWZWIiIiIiIjIvFLROejxeJyf/OQn7Ny5s7zM2ooVK1i8eHElqxERERERERGZdyragz5t8eLFvO1tb+Mtb3kLExMTjI2NndDrs9ksN910E0uXLmXt2rVce+217Ny5E4DBwUHe9KY3sWTJElavXs0jjzxyKt6CiIiIiIiIyGlV0QD9k5/8JP/yL/8CgGVZXH755WzYsIG2tjYeeuihEyrrIx/5CNu3b+eFF17g7W9/Ox/+8IcB+NznPsemTZvYsWMHd955J+9///spFAqVfBsiIiIiIiIip11FA/Qf/vCHrF27FoCf/exn7N69m1dffZVPfepT/I//8T+Ouxy/389b3vIWDMMAYNOmTezduxeAu+66i49+9KMAbNy4kebmZh5++OFKvg0RERERERGR066iAfrw8DCNjY0A/PKXv+Q973kPS5cu5UMf+hAvvfTSSZf79a9/nbe//e2MjIxQKBTKdQB0dnbS1dV12NflcjmSyeSMPxEREREREZG5qKIBekNDA6+88gqWZXHvvfdy7bXXApBOp3G5XCdV5le+8hV27tzJHXfcccKvveOOO4jFYuW/tra2k2qDiIiIiIiIyKlW0QD9v/7X/8p73vMeVq9ejWEYXHPNNQA89dRTLF++/ITL+3//3/+Xe+65h1/96lcEg0Fqampwu93s37+//Jy9e/fS3t5+2Nd//vOfJ5FIlP+6u7tP7o2JiIiIiIiInGIVXWbtS1/6EqtXr6a7u5t3v/vd+Hw+AFwuF5/73OdOqKyvfe1rfO973+OBBx4gHo+X73/3u9/NP/zDP/ClL32JZ555ht7eXi6//PLDluHz+cptEBEREREREZnLKhqgA7zrXe+acXt8fJxbb731hMro6enh05/+NAsXLuTKK68ESsH2U089xV/91V/xwQ9+kCVLluD1evnud7+Lx+OpWPtFREREREREZkNFA/S/+qu/orOzk/e+970AvOc97+Huu++mqamJX/7yl6xZs+a4ymltbcVxnMM+1tDQwH333VexNouIiIiIiIjMBRWdg/4P//AP5URs999/P/fffz+/+tWveNOb3sSf/MmfVLIqERERERERkXmloj3o+/fvLwfoP//5z3nPe97DddddR2dnJxdccEElqxIRERERERGZVyrag15VVVXOlH7vvfeWs7g7joNlWZWsSkRERERERGReqWgP+jvf+U7e//73s2TJEkZGRnjzm98MwHPPPcfixYsrWZWIiIiIiIjIvFLRAP1v/uZv6OzspLu7m7/+678mHA4D0N/fz8c+9rFKViUiIiIiIiIyr1Q0QPd4PIdNBvepT32qktWIiMhZxnEcxtIFAh4XAa/rqM99pS/JYzuH6B3LsKY1zoK6EK/2J9m8b4ywz8XqljhXL6+nOuw75LW5ooXPffTyRURE5I0bTGV5es8IuwcnaasOcm5HNe01QfrGMzzy2hAA57TE2DMyiWkYXLSohnjQW359wbIZSuWI+N1E/MdedjtbsHj4tSES6QIrm6OsbolV9P2Mp/O4XSZh3xsLsSu+Dvq///u/8+1vf5vdu3fzxBNP0NHRwd/+7d+yYMEC3v72t1e6OhEROcMl0gXcpoFpGocNvm3b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\n",
                         "text/plain": [
                             "<Figure size 1200x800 with 9 Axes>"
                         ]
@@ -682,15 +686,17 @@
                 "    header='Name')\n",
                 "calculated_data.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
-            "metadata": {},
+            "metadata": {
+                "keep_output_in_docs": true
+            },
             "outputs": [
                 {
                     "data": {
                         "image/png": "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8xI5AKTwcjhd2FfXhaK0eKTGG8I9HFKxL8tb8d8t1ZiVl4yblk1Q1eSOiILz4Lqj+Pv6MvnXvz5vGm7yHGuh8bN2Vy3ueGUPXCJwydxcPHDFXGg06qob88KWGvxq7T751z89fSLuWDkljCMiUqZQxqEMxMfYtqp2bCprxbkzszEtJ7LHSkREROPH4XThj+8fwof7G3H2jGz85vxpXKwLk9qOPnRbHJianaDK4q2iKOLRjRV4Y2ctlpam4zcXTGNRQKIAMBBXUCBOREREREREyhfKOJTLrkRERERERETjiIE4ERERERER0ThiIE5EREREREQ0jhiIExEREREREY0jBuJERERERERE44iBOBEREREREdE4YiBORERERERENI4YiBMRERERERGNIwbiREREREREROOIgTgRERERERHROGIgTkRERERERDSOGIgTERERERERjSMG4kRERERERETjiIE4ERERERER0ThiIE5EREREREQ0jhiIExEREREREY0jBuJERERERERE44iBOBEREREREdE4YiBORERERERENI4YiBMRERERERGNIwbiREREREREROOIgTgRERERERHROGIgTkRERERERDSOGIgTERERERERjSMG4kRERERERETjSBfuAQRCFEUAgNlsDvNIiIiIiIiIKBpI8acUjwZDkYF4W1sbAKCgoCDMIyEiIiIiIqJo0tbWhqSkpKDeQ5GBeGpqKgCgpqYm6L8AotEsXLgQ27ZtC/cwKArwWqPxwmuNxguvNRovvNZoPHR1daGwsFCOR4OhyEBco3EfbU9KSkJiYmKYR0Nqp9VqeZ3RuOC1RuOF1xqNF15rNF54rdF4kuLRoN4jBOMgUrVbb7013EOgKMFrjcYLrzUaL7zWaLzwWiOlEcRQnDQfZ2azGUlJSejq6uLKFxEREREREY25UMahitwRNxqNuPvuu2E0GsM9FCIiIiIiIooCoYxDFbkjTkRERERERKRUitwRJyIiIiIiIlIqBuJEHo888giKi4sRExODxYsXY+vWrQCA9vZ2/PSnP8WUKVMQGxuLwsJC/OxnP0NXV1eYR0xKNdy1BgA333wzSktLERsbi4yMDFx88cU4fPhwGEdLSjbStSYRRRHnnnsuBEHAm2++Of6DJFUY6VpbsWIFBEEY9N8tt9wSxtGSko12X9u8eTNOP/10xMfHIzExEcuXL0d/f3+YRks0PAbiRABefvllrF69GnfffTd27tyJOXPm4Oyzz0ZzczPq6+tRX1+Pv/71r9i/fz/+85//4MMPP8SNN94Y7mGTAo10rQHAggULsGbNGhw6dAgfffQRRFHEypUr4XQ6wzxyUprRrjXJQw89BEEQwjRKUgNfrrWbbroJDQ0N8n9//vOfwzhiUqrRrrXNmzfjnHPOwcqVK7F161Zs27YNq1atCkmrKaKQE4lIXLRokXjrrbfKv3Y6nWJubq54//33D/n6V155RTQYDKLdbh+vIZJK+Hut7dmzRwQglpeXj9cQSSV8udZ27dol5uXliQ0NDSIAce3atWEYKSndaNfaaaedJv785z8P0+hITUa71hYvXiz+5je/CdfwiPwS8ctDI6WfPPHEE1ixYgUSExMhCAI6OzvDN1BSLJvNhh07duDMM8+UP6bRaHDmmWdi8+bNQ/4eqWWBTqcbr2GSCvh7rfX29mLNmjWYMGECCgoKxnOopHC+XGt9fX245ppr8MgjjyA7OztcQyWF8/W+9t///hfp6emYOXMm7rrrLvT19YVjuKRgo11rzc3N2LJlCzIzM7F06VJkZWXhtNNOwxdffBHGUZOSDReHVlVVnXDcRvrv1Vdf9fn9IzoQHy39pK+vD+eccw5+9atfhXmkpGStra1wOp3Iysoa9PGsrCw0NjYO+fr77rsPP/rRj8ZriKQSvl5rjz76KEwmE0wmEz744AOsW7cOBoNhvIdLCubLtXb77bdj6dKluPjii8MxRFIJX661a665Bs8//zw+/fRT3HXXXXjuuefw3e9+NxzDJQUb7Vo7duwYAOCee+7BTTfdhA8//BDz58/HGWecgbKysnAMmRRspDi0oKBg0FGbhoYG3HvvvTCZTDj33HN9/hoRvZ33wAMP4KabbsINN9wAAHjsscfw3nvv4emnn8add96J2267DQCwcePG8A2SoorZbMb555+P6dOn45577gn3cEilrr32Wpx11lloaGjAX//6V1xxxRX48ssvERMTE+6hkUq8/fbb2LBhA3bt2hXuoVAUGLhwPWvWLOTk5OCMM85ARUUFSktLwzgyUhOXywXAXfRUih3mzZuH9evX4+mnn8b9998fzuGRwowWh34zk2zt2rW44oorYDKZfP4aEbsjHki6MFEg0tPTodVq0dTUNOjjTU1Ng/6RdXd345xzzkFCQgLWrl0LvV4/3kMlhfP1WktKSsKkSZOwfPlyvPbaazh8+DDWrl073sMlBRvtWtuwYQMqKiqQnJwMnU4nH7O57LLLsGLFijCMmJTK1/vaQIsXLwYAlJeXj/n4SD1Gu9ZycnIAANOnTx/0+WnTpqGmpmbcxknK528cumPHDuzevdvvQs4RG4j7my5MFCiDwYAFCxZg/fr18sdcLhfWr1+PJUuWAHDvhK9cuRIGgwFvv/02dyYpIL5ca98kiiJEUYTVah2vYZIKjHat3Xnnndi7dy92794t/wcADz74INasWROmUZMSBXJfk643KXAi8sVo11pxcTFyc3Nx5MiRQb/v6NGjKCoqGu/hkoL5G4c+9dRTmDZtGpYuXerX14no1HSi8bJ69Wpcd911OOmkk7Bo0SI89NBD6O3txQ033CAH4X19fXj++edhNpthNpsBABkZGdBqtWEePSnJSNfasWPH8PLLL2PlypXIyMhAbW0t/t//+3+IjY3FeeedF+6hk8KMdK1lZWUNuVtZWFiICRMmhGG0pGQjXWsVFRV44YUXcN555yEtLQ179+7F7bffjuXLl2P27NnhHjopzEjXmiAI+OUvf4m7774bc+bMwdy5c/HMM8/g8OHDeO2118I9dFKp/v5+vPDCC/jtb3/r9++N2EA8kFQnokBdeeWVaGlpwe9+9zs0NjZi7ty5+PDDD5GVlYWNGzdiy5YtAICJEycO+n2VlZUoLi4Ow4hJqUa61urr67Fp0yY89NBD6OjoQFZWFpYvX46vvvoKmZmZ4R46KcxI1xpRKI10rdlsNnzyySdywFRQUIDLLrsMv/nNb8I9bFKg0e5rt912GywWC26//Xa0t7djzpw5WLduHWsRkF/8iUNfe+019PX14fvf/77fX0cQRVEMaqRjaPHixVi0aBEefvhhAO70k8LCQqxatQp33nmn/LqNGzfiW9/6Fjo6OpCcnBym0RIREREREZHS+RqHrlixAunp6QFlXUTsjjgwcvoJADQ2NqKxsVEu9rFv3z4kJCSgsLAQqamp4Rw6ERERERERKdBocSjgLjj5+eef4/333w/oa0R0ID5a+sljjz2Ge++9V3798uXLAQBr1qzB9ddfH44hExERERERkYL5crzr6aefRn5+PlauXBnQ14jo1HQiIiIiIiIitYnY9mVEREREREREasRAnIiIiIiIiGgcMRAnIiIiIiIiGkcMxImIiIiIiIjGEQNxIiIiIiIionEUkYH49ddfj0suuSTcwyAiIiIiIiIKuYgMxImIiIiIiIjUKuID8Q8//BCnnnoqkpOTkZaWhgsuuAAVFRXy56uqqiAIAt544w1861vfQlxcHObMmYPNmzeHcdREREREREREQ4v4QLy3txerV6/G9u3bsX79emg0Glx66aVwuVyDXvfrX/8av/jFL7B7925MnjwZV199NRwOR5hGTURERERERDQ0XbgHMJrLLrts0K+ffvppZGRk4ODBg5g5c6b88V/84hc4//zzAQD33nsvZsyYgfLyckydOnVcx0tEREREREQ0kojfES8rK8PVV1+NkpISJCYmori4GABQU1Mz6HWzZ8+Wf56TkwMAaG5uHrdxEhEREREREfki4nfEL7zwQhQVFeHJJ59Ebm4uXC4XZs6cCZvNNuh1er1e/rkgCABwQvo6ERERERERUbhFdCDe1taGI0eO4Mknn8SyZcsAAF988UWYR0VEREREREQUuIgOxFNSUpCWloYnnngCOTk5qKmpwZ133hnuYREREREREREFLCLPiLtcLuh0Omg0Grz00kvYsWMHZs6cidtvvx1/+ctfwj08IiIiIiIiooAJoiiK4R7EN51zzjmYOHEi/vnPf4Z7KEREREREREQhFVE74h0dHXj33XexceNGnHnmmeEeDhEREREREVHIRdQZ8R/84AfYtm0b7rjjDlx88cXhHg4RERERERFRyEVkajoRERERERGRWkVUajoRERERERGR2jEQJyIiIiIiIhpHYQnE77//fixcuBAJCQnIzMzEJZdcgiNHjgx6jcViwa233oq0tDSYTCZcdtllaGpqGvSan/3sZ1iwYAGMRiPmzp075Nd65ZVXMHfuXMTFxaGoqIjtz4iIiIiIiCiswhKIf/bZZ7j11lvx9ddfY926dbDb7Vi5ciV6e3vl19x+++1455138Oqrr+Kzzz5DfX09vv3tb5/wXj/4wQ9w5ZVXDvl1PvjgA1x77bW45ZZbsH//fjz66KN48MEH2RaNiIiIiIiIwiYiirW1tLQgMzMTn332GZYvX46uri5kZGTghRdewOWXXw4AOHz4MKZNm4bNmzfj5JNPHvT777nnHrz55pvYvXv3oI9fc801sNvtePXVV+WPPfzww/jzn/+MmpoaCIIw5n82IiIiIiIiooEi4ox4V1cXACA1NRUAsGPHDtjt9kG9xKdOnYrCwkJs3rzZ5/e1Wq2IiYkZ9LHY2FjU1taiuro6BCMnIiIiIiIi8k/YA3GXy4XbbrsNp5xyCmbOnAkAaGxshMFgQHJy8qDXZmVlobGx0ef3Pvvss/HGG29g/fr1cLlcOHr0KP72t78BABoaGkL2ZyAiIiIiIiLyVdgD8VtvvRX79+/HSy+9FPL3vummm7Bq1SpccMEFMBgMOPnkk3HVVVcBADSasP/RiYiIiIiIKAqFNRpdtWoV3n33XXz66afIz8+XP56dnQ2bzYbOzs5Br29qakJ2drbP7y8IAv70pz+hp6cH1dXVaGxsxKJFiwAAJSUlIfkzEBEREREREfkjLIG4KIpYtWoV1q5diw0bNmDChAmDPr9gwQLo9XqsX79e/tiRI0dQU1ODJUuW+P31tFot8vLyYDAY8OKLL2LJkiXIyMgI+s9BRERERERE5C9dOL7orbfeihdeeAFvvfUWEhIS5HPfSUlJiI2NRVJSEm688UasXr0aqampSExMxE9/+lMsWbJkUMX08vJy9PT0oLGxEf39/XLV9OnTp8NgMKC1tRWvvfYaVqxYAYvFgjVr1sjt0IiIiIiIiIjCISzty4ZrG7ZmzRpcf/31AACLxYI77rgDL774IqxWK84++2w8+uijg1LTV6xYMWRQXVlZieLiYrS2tuLCCy/Evn37IIoilixZgj/+8Y9YvHjxmPy5iIiIiIiIiEYTEX3EiYiIiIiIiKIFS4cTERERERERjSMG4kRERERERETjiIE4ERERERER0ThiIE5EREREREQ0jhiIExEREREREY0jBuJERERERERE44iBOBEREREREdE4YiBORERERERENI4YiBMRERERERGNIwbiREREREREROOIgTgRERERERHROGIgTkRERERERDSO/j/ofariWGwl1QAAAABJRU5ErkJggg==\n",
                         "text/plain": [
                             "<Figure size 1200x800 with 1 Axes>"
                         ]
@@ -959,15 +965,17 @@
                 "## Plotting Conditions Alongside Signals\n",
                 "Now let's use the new condition in a plot, this time using `spy.plot()`, which has a set of predefined plot configurations."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
-            "metadata": {},
+            "metadata": {
+                "keep_output_in_docs": true
+            },
             "outputs": [
                 {
                     "data": {
                         "image/png": "iVBORw0KGgoAAAANSUhEUgAAA+IAAAK0CAYAAACHuocVAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjQuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8rg+JYAAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOzdd3hUZfbA8e+dkt47KfTQey8KKChg772t3Z+ri6517W1VdNW1ra5d1947ShWQKr1DgJAC6b1Pub8/bu4QMEDKzNyZ5Hyex2dmkzv3niwpc+573nMUVVVVhBBCCCGEEEII4RUmowMQQgghhBBCCCE6E0nEhRBCCCGEEEIIL5JEXAghhBBCCCGE8CJJxIUQQgghhBBCCC+SRFwIIYQQQgghhPAiScSFEEIIIYQQQggvkkRcCCGEEEIIIYTwIknEhRBCCCGEEEIIL7IYHUBbOJ1O9u/fT3h4OIqiGB2OEEIIIYQQQogOTlVVKisrSU5OxmRq35q2Xybi+/fvJy0tzegwhBBCCCGEEEJ0MtnZ2aSmprbrHH6ZiIeHhwPw0fy1hISFGxLDCf0SDLmuMM7C7QWGXFe+1zoXd32fyfeNMY707yf/HsKdWvJ7oiN8z7nj92FH+P/BSJ3le02IlqqoqCAtLc2Vj7aHXybiejl6SFg4oQYl4hEREYZcVxgnNKzWkOvK91rn4q7vM/m+McaR/v3k30O4U0t+T3SE7zl3/D7sCP8/GKmzfK8J0Vru2B4tzdqEEEIIIYQQQggvkkRcCCGEEEIIIYTwIknEhRBCCCGEEEIIL5JEXAghhBBCCCGE8CJJxIUQQgghhBBCCC+SRFwIIYQQQgghhPAiScSFEEIIIYQQQggvkkRcCCGEEEIIIYTwIknEhRBCCCGEEEIIL5JEXAghhBBCCCGE8CJJxIUQQgghhBBCCC+SRFwIIYQQQgghhPAiScSFEEIIIYQQQggvkkRcCCGEEEIIIYTwIknEhRBCCCGEEEIIL5JEXAghhBBCCCGE8CJJxIUQQgghhBBCCC+SRFwIIYQQQgghhPAiScSFEEIIIYQQQggvkkRcCCGEEEIIIYTwIknEhRBCCCGEEEIIL5JEXAghhBBCCCGE8CJJxIUQQgghhBBCCC+SRFyIw9WWQU2J0VEIIYQQQgghOihJxIVoqiwbXhgMz/SGnb8YHY0QQgghhBCiA5JEXIimVr8B9RWgOmDxM0ZHI4QQQgghhOiAJBEXoqmdvx58nrMaqgqNi0UIIYQQQgjRIUkiLoSutgwKt2vPQ+K0x+yVhoUjhBBCCCGE6JgkERdCd2ADoEJUN+h3ivax3DWGhiSEEEIIIYToeCQRF0JXtFN7TBig/df0Y0IIIYQQQgjhJpKIC6ErztAeY3tBbHrjx3YbF48QQgghhBCiQ5JEXAidnojHpUNcb+15yW5wOoyLSQghhBBCCNHhtDoRX7x4MaeffjrJyckoisI333xzyOdVVeXBBx+kS5cuBAcHM23aNHbt2nXIMSUlJVx66aVEREQQFRXFNddcQ1VVVbu+ECHarSxLe4zuDpFpYLKAowEq8wwNSwghhBBCCNGxtDoRr66uZujQobzyyivNfn727Nm8+OKLvPbaa6xcuZLQ0FCmT59OXV2d65hLL72ULVu2MHfuXH744QcWL17M9ddf3/avQgh30BPu8GQwmSEsqfHjB4yLSQghhBBCCNHhWFr7gpkzZzJz5sxmP6eqKi+88AL3338/Z555JgDvv/8+iYmJfPPNN1x00UVs27aNOXPmsHr1akaNGgXASy+9xCmnnMKzzz5LcnJyO74cIdqooRrqK7Tn4Y0JeEQXqMiBiv3GxSWEEEJ0YGV1Zby/9X0W5SwipzIHk2IiPjieAbEDCHX2oX/kGKIDE4wOUwgh3K7VifjR7N27l7y8PKZNm+b6WGRkJGPHjmX58uVcdNFFLF++nKioKFcSDjBt2jRMJhMrV67k7LPP/tN56+vrqa+vd/3viooKd4YtxMHVcGsIBIZrz8O7NH5OVsSFEEIId/s993fuWnwXFQ2Hvq+rtlWTWZEJ/ARAj7BBjI2bzsjYaVhMVu8HKoQQHuDWRDwvT0tmEhMTD/l4YmKi63N5eXkkJBx6Z9NisRATE+M65nBPPvkkjzzyiDtDFeJQrrL0JFAU7XlEY3WGrIgLIYQQbrUwayG3LboNh+qgT3Qfrhl0DYPiBuFUneyv2s/6wvXM2b2YzKqt7K3azN6qzfyc+x5npt3AsJgpKPrfaiGE8FNuTcQ95d577+X22293/e+KigrS0tIMjEh0OFV6It7l4MckERdCCCHcblfpLu5ecjcO1cEpPU7h8YmPYzUfXOnuHtmdCSkT6BNwLmUNhawpns+S/K8ptxXx/p4nWF+6mEt63EWgOdjAr0IIIdrHrePLkpK0vbX5+fmHfDw/P9/1uaSkJAoKCg75vN1up6SkxHXM4QIDA4mIiDjkPyHcqumKuC68MRGX0nQhhBDCLexOO/f/fj+19lrGdhnLE8c9cUgSfriogHimdrmI+4d8wIzkKzEpZjaWLuHVHXdS56j2YuRCCOFebk3Ee/ToQVJSEvPnz3d9rKKigpUrVzJ+/HgAxo8fT1lZGWvWrHEds2DBApxOJ2PHjnVnOEK0nJ5sH7Ii3vhcVsSFEEIIt/h0x6dsLd5KeEA4Tx3/FBZTy4ozLaYApqdczi39nifEHE5W9Xbey3gMh+rwcMRCCOEZrU7Eq6qqWL9+PevXrwe0Bm3r168nKysLRVGYNWsWjz/+ON999x2bNm3iiiuuIDk5mbPOOguA/v37M2PGDK677jpWrVrF77//zl//+lcuuugi6ZgujKOviIc16W/QtFmbqno/JiGEEKIDqbZV8/qG1wGYNWIWccFxrT5H97AB3Nj3aQJMQWyv+IP5Bz52d5hCCOEVrU7E//jjD4YPH87w4cMBuP322xk+fDgPPvggAHfddRe33HIL119/PaNHj6aqqoo5c+YQFBTkOseHH35Iv379mDp1KqeccgrHHXcc//3vf930JQnRBpVH2SNuq4G6cu/HJIQQQnQgH277kNL6UrpFdOOc9HPafJ600D6c320WAL/s/4Dcmgw3RSiEEN7T6mZtU6ZMQT3K6qCiKDz66KM8+uijRzwmJiaGjz76qLWXFsJzXIl4kxVxazAERWpJeGUeEG1IaKJjsDltWGXsjhCik2pwNPDhtg8BuHHojS0uST+SkbFT2VS2lI2lS/km6zX+r+8z0kldCOFX3LpHXAi/VVOsPYbGH/rxkMayudoS78YjOoy86jwu++kyRnwwghvn3kh5vVRXCCE6n5/3/kxJXQmJIYlM7z693edTFIUz027ColjJqFzP1vKVbohSCCG8RxJxIZxOqCvTngfHHPq5kFjtUU/UhWgFh9PB7YtuZ0PhBgB+3/879y+9/6hVRUII0dGoqsr/tv0PgIv7Xey26qCYwESOTzwLgHmyV1wI4WckEReivhxUp/Y8+LDyc0nERTv8uu9XNhVtIswaxtPHP43FZGFRziJW5snKjRCi81hXsI7tJdsJMgdxXp/z3HruyYnnYVGsZFZtYXflJreeWwghPEkScSFqGsvOA8LAEnDo5yQRF+3w8XZtheaKgVdwSs9TOL/P+QB8sPUDI8MSQgiv+nb3twDM6DGDyMBIt547MiCW0XEnA/B7wbduPbcQQniSJOJC1JZqj4eXpQOENH6sRvaIi9bJq85jXcE6AM7prXUHvqjvRQAsy10me8WFEJ1Crb2WXzJ/AeDMXmd65BoT4k8DYGPp71Tb5XerEMI/tK9lpRAdgSsRj/rz52RFXLTR3H1zARiRMILEUK0bf8+onvSJ7sPO0p3Mz5rfrvE9QgjhD+ZnzafaVk1KWAojEkd45BqpoemkhPQmtyaDNcULmJR4tkeuI/xDrb2WLUVbyK7MpsZeg0WxkBiaSGpYKl0juhJgDjj2SYTwAknEhdBXu0OaWxGXRFy0zbx98wA4ufvJh3x8RvcZ7Czdya+Zv0oiLoTo8L7L+A6AM3qdgUnxXCHm2LgZfJX1MisLf+b4hLNklFkntKNkB29uepPfcn6j1l7b7DFmxUxaeBq9o3rTK6oXvaN70yuyF9FB0YRYQgiyBHn0+1SIpjpFIl7eUExRfS7VtnICzEFEWuNICO6KWTEbHZrwBfposmZL0yUR75BsdWCraf7mixvU2mvZWLQRgEkpkw753JS0Kby47kXW5K+hwdEgd+aFEB1WXnUeKw6sAOD0Xqd79FojY6fyXfbr7K/dw4HavSSH9PTo9YTvqLPXMXv1bL7Y+QUq2lSShJAEekf1JiIgggZHAweqD5BTmUOlrZLMikwyKzKZlzWv2fNZTBYCTAEEWYLoHtGdwXGDOb3X6fSN6evNL0t0Ah02Ea931LKs8AdWF/3Kgdq9f/p8gCmI9IjhjIg5gYFR4wk0BxsQpfAJrtL06D9/ThLxjmfDJ/DTnVBfAYPOhbNe+3OTvnbaVLgJu9NOQkgCqeGph3yud1RvYoJiKKkrYVPRJkYmjnTrtYUQwlf8sOcHVFRGJIwgLTzNo9cKsYTTL3IUm8uWs7F0iSTinURedR63LriVbSXbAJjefTp/GfQXBsQM+FNVhKqqFNYWklGWQUZpBrvLd5NRlsHe8r1UNVS5kni7047daafGXkNJXQlrC9by3tb3OLPXmdw79l5CraFe/zpFx9ThEnFVVVlXspCvsl6m2l4BgIJCXGAyoZZIGpz1FNcfoN5Zw5ay5WwpW06wOYzjEs5kUuLZhFmjjP0ChPe1qDRdmrV1CJlL4esbofGPLZu/hPAuMP0Jt15mTf4aAEYmjvzTGwFFURiTNIY5mXNYdWCVJOJCiA5JVVW+zdC6mJ/Z2zNN2g43JPp4VyI+I+VKr1xTGKegpoCrf7ma7MpsogOjmT15NuO6jDvi8YqikBCSQEJIAhOSJxzyOVVVqXPUUWOrwea0YXPYqLJVkVGWwcLshczdN5dvd3/LztKdvH7S60QHNbN4I0QrdahE3O5s4JPM51hTrJWaxAemcGKXCxkcPZFQy8FxGU7VSV5tJutLfmNNyXxK6vOYe+BDFud/xbTkS5iceC5Wk5SLdhqu0vTmVsQbk/P6ChRHA6qUEfsvWy18+1dAhSEXQf/T4NPLYOXrMO7/IDLFbZfSE/FRiaOa/fyYLo2JeN4qbuImt11XiPZQVe0GlTv31tbaa1FVlRBriNvOKfzDpqJNZFZkEmQO4uRuJx/7BW4wMGo8JsXMgdpMCupySAhKPfaLhF+qbKjk+l+vJ7sym5SwFN6e/jbJYcltPp+iKARbggm2HFoh2z+2P6f3Op11BeuYtXAW20q2cfui2/nvyf/FarK298sQnVyH6UZQa6/i9Z33sqZ4HiZMzEi+krsHvcW4+FMOScIBTIqJ5JCenJL6F+4b/B5X9XqQ1JB06p21/JjzFk9vvoaMivXGfCHC+442viwoChp7CVgbSr0Xk3C/te9D6V6ISIFTZkP/06HrBHDaYJ375no7VSebijYBMDxheLPHjEzQVsE3F23G7rS77dpCtEV5fTmPr3icKZ9NYcQHIzj727P5YOsH2By2Np9zY+FGbph7A2M/HMvYj8Zy07ybyKnMcWPUwtfpq+Endj2RsIAwr1wzxBJOevgwADaWLvHKNYX3qarKw8seZnf5bhKCE3jz5DfblYS3xPCE4bw9/W1CraH8kf8Hr2943aPXE51Dh0jEG5z1vLnrATIqNxBoCuGGvk8xPeVyzKZjL/ibFDNDYyZx24BXuLTHPURaYymuP8ArO+7g66xXsTkbvPAVCEMdrTTdZHJ9PKBeytP9lsMGy17Snh//dwhqvDk3srF0cfNXbrtUVkUWNfYaAs2B9Ijs0ewx3SO7E2YNo85Rx+6y3W67thCtlV2RzbnfncunOz6lpK4Eu2onoyyD2atnc+GPF5JZntnqc36w9QOu+PkKlu1f5tpzuTR3KZf+dCkHqg64+SsQvqjOXsfPe38G4KzeZ3n12kOijwdgc+kyr15XeM/nOz/n132/YlEsPH/C83/qxeIpvaJ68fD4hwF4e/Pb7KvY55Xrio7L7xNxp+rkwz1PsqdqE0HmUG7u9y/6RLR+TqVJMTEqbhr3DH6H8fGnArA4/yte2f53KmySgHVoRytNb/Jxa0OFlwISbrfteyjPhtAEGHbpwY/3mQEmCxTtgGL3JMTbS7YD0De6L5Yj3Aw0KSYGxg4EcK2eC+FtZXVlXD/3evJr8ukW0Y3Xpr3Gr+f+ygPjHiA6MJpdpbu49KdLWXVgVYvOp6oqL697mdmrZ+NQHczsPpOfzv6JH87+gfTodErqSrhnyT04nA4Pf2XCaAuyFlBpq6RLaBfGdhnr1WsPiNKul1W9nWp7uVevLTwvrzqPZ/94FoBZI2cxJH6IV68/vft0JqZMxOa08e+1//bqtYVvONJovLbw+0R83oGP2Fi6FLNi5Zrej5IWmt6u8wWZQ7ig+21cl/4EIeZw9lVv4/mtN7O/Zo+bIhY+p7ZMezxSIh4UBYClQf6g+611/9MeR14J1qCDHw+OgrTGN4n7fnfLpbaWbAWgX0y/ox43KG4QoJWnC2GEf676JzlVOaSGpfLujHeZmDKRLmFduKDvBXx15lcMiR9CRUMFN8y7ge93f3/Uc6mqyuzVs3l9o1aueevwW3l60tOkRaTRLaIb/57yb0KtoawtWMt3u7/zxpcnDPRNxjeA1qTN2zOZowLi6RLcHRWVHeVrvXpt4XmzV8+m1l7LsPhhXD7gcq9fX1EU7hh5BwDz9s1jT7nkB52Jqqo8scJ9DX79OhHPqNzAnNz3ALig+230jhjqtnMPiBrLrAEvkRCURllDIa/uuEOS8Y7I6YT6Su15Y8L9J41lzLIi7qfKc2D3Au1509VwXdoY7TG7Zat+x7K9WFsR7x/b/6jHDY4bDMiKuDDGkpwl/Lz3Z8yKmWcmP0NccNwhn48LjuPt6W8zo/sM7E47/1j6D17b8JqroVtTDY4G7l16L//bpt3wumfMPVw35LpDmr6lRaRx01CtMeHrG1/H5mz7/nPh2w5UHXDNDj+zl3e6pR+uX+RoALaVu+f3uvANKw6sYO6+uZgVM/ePu9/rN3l0vaN7c0LaCaiovL/lfUNiEMZ4b8t7R5w/3xZ+nYh/vvd5VFTGxs1kTJz7O3LGB6Xyt/4vkhbSh2p7Ba/uuJPCuly3X0cYqL4C1yiroIjmjwmOAsBik0TcL236AlCh23EQ08ye7dTGRDxntVsut6N0BwD9Y46eiA+M00rT95TtocEhvSiE9zhVJy+sfQGAS/tf6qrOOFygOZCnJz3NXwb9BYBX1r/CrIWzyKvOcx2zp2wP1/xyDT/u+RGzYuaxiY9xaf9mbngBF/S9gNigWHKrcpmzd457vyjhM77d/S0qKqOTRntt7+7h+kdqv9d3lP+BU3UaEoNwL1VVeWmd1uvlwr4X0jemr6HxXDlQ6zHz096fqLZVGxqL8I61+Wtdfzvdxa8T8Qp7CfGBKZzT7a8eu0aIJZwb+z5Nakg61fZy3tz1ALX2Ko9dT3hZfWNybQ4ES2Dzx7hK0yUR90tbtc69DD63+c/rK+KF2w920G+j0rpSSuq0ngM9o3oe9djEkETCA8Kxq3b2lu9t13WFaI1f9/3KztKdhFvDuX7I9Uc91qSYuH3k7Tww7gEsioUF2QuY+eVMLvvpMi764SLO/PZM1heuJ8waxqvTXj1qY65gSzAX9bsIgK8zvnbnlyR8hM1h4/MdnwNwdu+zDYujR9hAAkxBVNpLXX07hH9btn8ZGws3EmgO5Loh1xkdDiMSRtA9oju19lp+yfzF6HCEh5XXl3P3krtxqA5mdJ/htvP6dSIOcGGPOwgwHSGBcpMQSzjXpj9OlDWegros/rfnyWbL84QfqmtMro+0Gg6uFXGrTfaI+53SfbB/LSgm6Hda88eExkFMY9Kcu6Zdl9MT6uTQ5D/NIj2coij0ie4DwM7Sne26rhCt8cEWbVzfpQMuJTIw8hhHay7oewGfnPYJY5LGYFftbCjcwJbiLQBMSZvC56d/zoTkCcc8z1m9z0JBYXXearIrstv+RQif9Mu+XyioLSAuOM6tb1Zby2IKoHfjGDO9TF74L1VVeXXDq4D2u+jwrTRGUBSFs9O1m036qD7RMamqyoO/P0hedR7dIrpx5+g73XZuv07Ex8efSq/wwV65VmRALFenP4pFsbK1fCWf7fjMK9cVHqaviAceJRGXFXH/ta2xKVS3iRCWcOTjkhq7rha0b+VEb9rSI6r5sWWHk0RceNuGwg1sLNqI1WTlwr4Xtuq1fWP68tb0t/jh7B94ZtIzPDflOX459xdeOvGlFpcgJ4UmMSFFS9h/2PtDq+MXvktVVf63VesTcFHfi7CarYbG0ydiOECLu/4L37WhcAMbCzcSYArg6kFXGx2Oyyk9TgFgXcE6imqLDI5GeMq3u79lQfYCrCYrsyfNJtQa6rZz+3UiPj3Zu90S00LTOS1VK4d59o9npZy0I3CtiB9lVUhfEZeu6f5HL0sfcIyGQfGNe80K25eI678TekRIIi5804dbPwRgZo+ZbV5V6hbRjRk9ZnBSt5NIDktu9eund5sOaCOuRMexOm81W4q3EGgO5Py+5xsdDr0jhgGwtmCtNAf0cx9v/xiAU3qe4hOr4bqk0CSGxA1BRWX+vvlGhyM8oLCmkNmrZwNw87CbGRA7wK3n9+tEPNAc4vVrHp94Fn0iRlLnqOOfK/8pJer+rq4xuT5aaXpjkm6xVXohIOE2lfkHG7D1P/3ox+qJeFH7EmJ9RfxY+8N1kogLbyqpK2HuvrkAXNb/MsPimJI2BZNiYnvJdnIqcwyLQ7hP00ZaZ/U+i5igGIMjgi7BPQi1RFBrr2VL0RajwxFtVFRbxK/7fgVw9ZjwJdO6TQNgbtZcgyMR7qaqKk+sfILKhkoGxA5wNehzJ79OxI1gUkyc3+1vBJgCXGMUhB9rRWm6rIj7mYzG8RJdhkF40tGPjW+c+V24Hdpxc621K+K9o3qjoFBUW0RxbXGbrytES/ya+St21c6A2AHHHK/nSdFB0YxMHAnAwuyFhsUh3GdB1gLWF64nyBzEDUNuMDocQHu/1itcG2u78sBKg6MRbfXVrq+wO+0MiR/CwNiBRofzJyeknQBoHbVr7bUGRyPcaWH2QuZnzceiWHh0wqNYTBa3X0MS8TaIC0rm6sHaHpVn/niGOnudwRGJNmvJiriML/NPGY03ydJbMNowtrfW0K2uHKry23S5Onsd+6v2A9AjsmWJeIg1hLTwNAB2le1q03WFaKmf9v4EHNzXaKTJqZMBWL5/ucGRiPaqsdXw1OqnALh8wOXEh8QbHNFB6Y0N21bnuWc8pfAuVVX5brfW6+WCPhcYHE3zukV0o0toF2xOG2vy29fwVfgOm8PGv/74F6CNqvPUuDxJxNvomkHXkBSaRF51Hp/v/NzocERbuVbEj7JHvOmKuGxF8A8OO+xu3H+aftKxj7cEQnRj8ly4o02X3FexDxWVyMDIVpVl6uXpO0radl0hWiK3Kpd1BetQUAztZq0b12UcAH/k/4HNIft3/dns1bPJq84jJSzFJ8ZKNZXeuE98feF6GhwNxgYjWm1L8Rb2VewjyBzkKgH3NYqiMD55PCA3FjuSj7d/TFZlFnHBcR79vSaJeBsFWYK4cciNALy56U1qbDUGRyTapBXN2kxOGyaHVD/4hZzV2up2cDSkjGzZa+K0hJjitq1MNy1LVxSlxa/rHd0bOLi/XAhP+HnvzwCMSRpDYmiiwdFAenQ6MUEx1Npr2VS0yehwRBt9vetrvtz1JQoKj0x45JhjG70tIagrccFx1Dvq2VC4wehwRCv9uOdHQCv/dmenandzJeIHJBHvCMrqynht42sA3DL8Fo9+70ki3g5n9D6DtPA0SupKXB0dhZ+pb8Ec8YAwUMyAlKf7jV1aYxd6TQWTuWWvie6uPZZltemSrtFlLSxL1/WM1Bq77SmTRFx4jv6G9pSexpelg7Z/d0zSGEDmPPur+VnzeXj5wwDcOPRGxnYZa2xAzVAUhdGJowFYlSdjzPyJ3Wl33UA8teepBkdzdOOSxqGgsKt0F4U1hUaHI9rprc1vUdlQSd/ovpzZ6xhTd9pJEvF2sJqs3DhUWxX/37b/SdmTP9L3iB+tWZuiuFbMrTJL3D+0Zn+4Lqqr9li6r02XzKrUEvhuEd1a9To9cd9TvkemMAiP2Fm6k4yyDKwmq0+Vd+rl6ZKI+5/Veau567e7cKpOzup9FjcNvcnokI5oTBftho/ME/cvf+T/QXFdMVGBUUxImWB0OEcVFRTlaoApv8/8W2ldKZ/u+BSAW0fcirmlizltJIl4O83sMZPEkESKaotcKw7Cj9S1YEUcDjZsk87pvq/iAORtAhToPbXlr9MT8TauiOtjmPTmay3VPaI7CgoVDRWU1JW06dpCHI3+t2lS6iQiAo7xu86LxiVrifjGwo1U26oNjka01I6SHdyy4BYanA2cmHYiD41/qFXbcbxNr7zYWLRRulr7kUXZiwCtLN1qshoaS0vo32frCtYZHIlojw+2fkCtvZYBsQM4PuV4j19PEvF2spqsrnms7215T1a0/E1LxpfBwYZtUpru+/SxZcnDITSu5a9zUyKeGp7aqtcFWYJIDksGZJ+4cD+n6nSVd/pCt/SmUsJSSA5NxqE6ZP+unyioKeDm+TdTbatmVOIoZk+e7ZGRPu6UFp5GUmgSdqddvs/8hKqqrkR8StoUI0NpsWEJwwCtMaDwT5UNlXy0/SMArh9yvVduMEoi7gbn9jmXUGsou8t3szR3qdHhiNZoSbM2cK2YW2xVHg5ItFtbytLhYCJeUwT1rft3rrHVUFynzQFvbSIOB8vT9YZvQrjL+oL1HKg+QJg1jEmpk4wO50/0N68bCiRB8nUOp4PbF91Ofk0+PSJ78MIJLxBoDjQ6rGM6ZJ+4lKf7hYyyDHKrcgkwBbi2sPi6ofHazPqM0gwqZBujX/o241uqbdX0iuzlmg/vaZKIu0F4QDjnpJ8DwPtb3zc4GtEqLWnWBhAYDoDFVunhgES7OGywe6H2vCVjy5oKjjp4Q6Y8u1UvzanSVsMjAiLaVPqrN2yTRFy4m16WPrXrVIIsQQZH82fDE4YDUs7pD97d8i4bCjcQZg3jlamvEHm0sZ8+ZnSSloj/kf+HwZGIltBXw8cljyPEGmJoLC0VFxxHWngaKiqbCmUShL9xqk5X4+1L+l+CSfFOiiyJuJtc2v9SFBRWHFhBVkXbSluFlzkd0NC48nmsNxSNn5dE3Mdlr9JuroTEaqXprdXG8vS2lqXrXJ3TpTRduJHNYeOXfb8AvtMt/XD6ivjGoo04nA5jgxFHVFRbxOsbXwfg7jF3t7oXhtFGJY0CYFPRJhk36wcW5SwC/KcsXTcsfhgg5en+6Pfc38mqzCLcGs5pPU/z2nUlEXeTlLAUJqZMBOCLnV8YHI1okfomSXVg2NGPdZWmSyLu09oytqypqMaO563snN7WRm06KU0XnrD8wHLK68uJDYplbJLvjZYCSI9KJ8QSQrWtmoyyDKPDEUfwxsY3qLXXMiRuiMfH+XhCaliqa5+4JEm+raKhgs1FmwG80izLnfQbi1Lh438+2/EZAGf2PtOrVRiSiLvR+X3OB+CbjG9klJk/aGjs0muyguUY+9wam7mZpbOvb9MbtbV2f7gusnFFu3J/q16WXamVsqeGtW9F/ED1Aeod0tVXuMcPe34AtOkenh7B0lZmk5kh8UMAefPqq0rrSl0LDLeMuMWnO6QfiaIorq7Wf+RJebovW523GqfqpHtEd5JCk4wOp1X0feIbC6XCx58U1xa7enyd3/d8r15bEnE3mpQ6iYSQBErrS5mfNd/ocMSxuMrSj7EaDrIi7g8q9kP+ZkCBXie27RzhjX/0K/Na9TJ9j3hbS9OjgqKICYoBoKCudfvThWhOja3Gtc/S17qlH07fJy4rlb7pm4xvaHA20D+mv89WVrTEqEStPH113mqDIxFHs2K/NofbX5q0NdU7qjfBlmBq7bVS4eZH5mTOwa7aGRw32LUw4i2SiLuRxWRxNW37fOfnBkcjjknvjB3QgkRcmrX5vl2N3dJTRkJobNvOEd5Fe6w80KqXtXePOBwsT8+vlR4Tov0WZi+k1l5L1/CuDIobZHQ4R+Ua+1Ow3tA4xJ+pqup6P3NRv4v8cjVcpzds21y0WfaJ+7CVeSsB/0zEzSYz/WP6A7C1ZKvB0YiW+m73dwCc3ut0r19bEnE3Ozf9XEyKidV5q+VumK9raE0iLiviPq+tY8uaasOKuMPpILcqF2h7aTocTMQL6iQRF+33096fAK1Jm68nT0PihmBSTORW5VJQU2B0OKKJjUUbya7MJsQSwozuM4wOp11Sw1NJDk3Grtrlpo+Pyq/OZ2/5XkyKydVgz98MiB0AwNZiScT9we6y3Wwt3orFZDHkd5wk4m6WFJrkai4hTdt8XJtK02WOuE+yN8DuRdrz9GltP4++Il7R8hXxwtpCbE4bFsXSrv1sejlUviTiop2Kaov4Pfd3wPfL0gHCAsJIj0oHZFXc1/yaqTXAnJw22W/GSB2NntytzpfydF+kr4YPiBngV+PxmtIT8W3F2wyORLSE/jvuuOTjiA6K9vr1JRH3AL1p23e7v5Ombb6sVaXp+vgyScR9UvZKaKiEkDjo0oaxZTp9Rby+/GAzv2PYX6U1dksMTcRisrT50q5EXErTRTv9uOdHHKqDIXFDXJUWvk5v2LaxcKPBkQidqqrM3adVGk3vNt3gaNxDL09flbfK4EhEc9bkrwFgdJfRBkfSdnpp+raSbdKwzQ/My9Ka/E7r1o5FnHaQRNwDJqZMJCEkgbL6MhZkLTA6HHEkrtL00GMfK3vEfZtelt57Gpja8WstMAL0VZ8Wlqfvr9YS8eSw5LZfl4Ol6UX1+3E47e06l+i8VFXlm4xvAG0Mi79wdRsukkTcV+ws3cmB6gMEW4Jd41n9nZ6IbynaIvvEfZA+OWFEwgiDI2m7HpE9XA3b9lW0bhSq8K7symx2lu7ErJgNm1kvibgHNG3aJuXpPsxVmh5+7GP10nR7FaiqB4MSbaI3aks/qX3nUZQmDdtalojnVWvHdQnt0q5LJ4UmEWwJxqHaKa5vXbM4IXTbSraRUZZBgCmAGT38Z0+vnohvKdqCzWEzOBoBsGz/MkDrNh5kCTI4GvdICUshJSwFh+qQcXk+pqyuzNVbSf994I/MJjN9o/sCsKV4i8HRiKPRF0tHJY0ybCuEJOIecnbvs1FQWJm3kuwKGUfkk1pVmq4l4orqxGyXWeI+pSwbCraCYmr72LKmWtk5/UCVdlx7552aFBPdI7oDsk9ctJ2+Gj6161QiAiKMDaYVukV0IzIwkgZnA9tLthsdjgCW718OwITkCQZH4l76GDMpT/ctGwo3ANA9orshe3XdSRq2+Yd5+7Sy9KldpxoWgyTiHpIcluwq5fpy15cGRyOape8BbklpujUYp6Lt/5V94j5m1y/aY9pYCIlp//la2Tn9QLWWiLd3RRygV1QvAPJqpZzNp9RXweq3YNHTkLfZ6GiOqMHR4OqW7k9l6QCKojAkrnGfuJSnG67OXufar9vREnG9PP2PvD8MjkQ0pVcoDE9oR58XHyGJuO8rqytz3fw5Ie0Ew+KQRNyDzks/D9BWKGxOKbXzOQ2N+71b0jVdUbBbteMkEfcxOxsT8faMLWvKlYi3cEXcA4l4viTivqO6GN44EX68HRb9E16fBBs+NTqqZv2W8xvl9eUkhCT45QxevRx1Q8EGgyMRGws30uBsICE4wW8a/rWUa5948RaqbVLh5is6UiLeP1Zr2La9ZDtO1WlwNKI5Kw6sQEWld1Tvdlc0tock4h40KW0SsUGxFNcV81v2b0aHIw7nKk1vwR5xaJKIS8M2n9FQA3sXa8/7uGk/bGi89lhTfMxDVVU9mIiHtT8R1zun59VJIu4TnA748moo2gFhSdBjMqgO+PZmyNtkdHR/8m3GtwCc0esMzCazwdG0nt45XV+lEMZZW7AWgBGJI3x+Dn1rJYclu/aJ66v+wlg2h821n3pogv/uD9f1jOxJkDmIGnuNNGzzUb/v10Z8Tkw2thGlJOIeZDVZOTv9bECatvmk1nRNBxxW6Zzuc/YuBnsdRKZBQn/3nFNPxKsLj3lopa3StaKSFNL+O6p6Il5Qly130X3Bho9hzyKwhsLlX8Pl30DfU8Bpgzn3Gh3dIYpqi1iauxSAM3v5V1m6bnDcYBQU9lfvp7Dm2D9/wnP0ee4dYXWyOXrFiL4PXhhrW8k26h31RAVG0SPC/yswLCYLfaL7ALCjZIfB0YjDqarqakY5IcXYrTeSiHvYOb217unL9i8jtyrX4GjEIfQ94i0pTQfskoj7Hn1/eJ/pWsdzd9AT8aqCYx6qN2qLCowiRB971g6p4amYFSs2Zz2lDfntPp9oB3s9LHpKez7lHkgcoI3GO+UZMFkhcwlkrTQ2xiZ+2P0DDtXBsPhhdI/sbnQ4bRIWEObaniHzxI3jcDpYX7ge0FbEOyJ937u+KiaMpZelD4sf1mEqMPrGaJ3Tt5VsMzgScbjdZbspqCkg0Bxo+Kg8ScQ9LC0ijXFdxqGi8tWur4wORzRV35hQt7g0XTvOLHvEfYOqNtkfPt195w2N0x6ri455qLtGl+ksJgsJQanauWWfuLE2fgbl2VoX/THXHfx4ZCoMu1h7vvR5Y2I7jKqqfLtbK0v3tyZth3PtEy+S8nSjZJRlUG2rJtQaSnpUutHheMS45HGYFTN7y/eyv2q/0eF0evqNt45Qlq7rF9MPkBVxX6TfgPOF0YySiHvBuX3OBeCbXd9gd9oNjka4tLI0XZq1+Zj8LVCRC5Zg6HG8+87btDT9GDPj3dmoTZcU3A2AgloZYWYYVYXVb2jPx94I1uBDPz/+Fu1x169QaXzlwtbirWSUZRBoDmR6dzfelDKANGwz3uYibTLAoNhBftlroCUiAiJcPQlkVdx4+qrxwNiBBkfiPnoiLuMYfc/qvNUAjE8eb3Akkoh7xdS0qcQExVBQWyBN23xJq0vTpVmbT9HL0ntO/nOi1B76irjTBnXlRz3UnY3adAlBXQFp2Gao3LVwYAOYA2H45X/+fHwfSB2tNW7b9Jn34zvM1xlfA9os1PAWVvj4Kj0R31q8VaaNGEQfuTQgboDBkXiW3qTp91xJxI1U0VBBdmU2AP1j3NTrxQekR6djUkwU1xVTVHvsCjvhHQ6ng7X5WjPKUYmjDI5GEnGvsJqtnJOu7RV/d8u7xgYjDnJ1TZc94n5p2/fao7u6peuswQe3KxyjPF3fI+6JFXEZYWagDR9rjwPOhNDY5o8Z2lievuET78R0BPWOen7e+zMAZ/U+y9BY3KF7ZHfCA8Kpc9Sxs3Sn0eF0Snr3an0Wckc1MUVLxFceWCk3fQykl26nhKUQFRRlbDBuFGwJpluE9vdcVsV9x66yXVTaKgm1hrr28RtJEnEvubT/pVhNVtYXrnc1pRAGcjpBnx8qibj/Kd0H+9eBYoJ+p7n//K594kfv3KyviLtzBmViYyKeV5uFeozSeOEBDjts/UZ7PuSCIx838GxQzJC/GUozvRFZs37L/o2KhgqSQpMYkzTGsDjcxaSYDo4xk/J0r7M5bK4bIB2pTLg5A2IHEB0YTZWtSpoDGkivwOhIq+G6ftFSnu5r9JGFwxKGYTFZDI5GEnGviQuO44xeZwDw9ua3DY5GuJJwaH3XdLvsETfctu+0x24TISze/edv4QgzT+wRjw9MwYSJemcN5bZjzzIXbrb3N+3fPTgGek458nEhMdCtcezJ9p+8ElpzftjzAwCn9ji1w+znHRqnladvLJLkyNsyyjKwOW1EBESQGpZqdDgeZVJMrj2iS3KWGBxN5+VKxGM7YCIeK4m4r/kj7w/AN8rSQRJxr7py4JUoKCzKXsSesj1Gh9O56WXpihla2DFRmrX5kC3faI8DPNQhugWJuM1po7BW+3xyWLLbLm0xWYkLSgGkPN0Qm7/UHgeeBWbr0Y/te4r2uP1Hj4Z0JOX15SzJ1RKI03p6oDLEINKwzThNk6KOMkbqaKakTQFgQfYCYwPpxPRGbR15RVw6p/sGVVVdK+KSiHdCPSJ7cGLXEwH4z4b/GBxNJ9fQZH94C99sSLM2H1GWDbl/AAr0P90z12jBCLPCmkKcqhOryUpMUIxbL58YpJenSyLuVfYG2KatMDPovGMf368xEc9aBjUlnovrCH7d9yt2p52+0X3pHd3b69f3lMHxg1FQyKnKobhWqkK8qbPsD9cdl3IcFpOFveV72VMuCyTeVmOrIbM8E+iYK+J9YvoAsK9iHzW2GoOjEXsr9lJaX0qgOdBntt5IIu5lNw29CQWFOZlzXH/whAH0RLyFZekge8R9ht6kret4CHff3uxDuFbEC454SNP94SbFvb9Kk4K1zun5dTLCzKv2/Q715RCaoH1/HUt0d0gcBKrz4Ex7L/pxj7YSf2rPU71+bU8KDwinZ2RPANm762X6irivvEn1tPCAcMYmjQVgYdZCg6PpfHaU7kBFJSE4gbjgOKPDcbu44Djig+NRUaX5pA/Q/54MjB2I9VgVb14iibiX9Y3p63rT9Pya56UZk1Fa2TEdmibiUppuqC1faY+eKksHCGnslH2UVc79VfsB9+4P1yVK53Rj7NC6j9N3Bpha+Oex70ztcZd3E/EDVQdYk78GBYWZPWZ69dreMDRBK09fX7je2EA6EYfTQUZZBnBwBnJnoFcqLsiS8nRvc43K68AVGDJP3HfoibjeENQXSCJugL8O/ytWk5WVB1Yyd99co8PpnFyl6aEtfomsiPuAol2Qs1rb2z/wLM9dJ6Sx1Lz2yIl4XnUe4JlEPMnVOT1TbtZ5i6oeTMT7tCKxTT9Ze8xYoHVc95I5mXMAGJU0yq1d+33F8IThAPyR/4fBkXQeOVU51DvqCTIHdfhGbU2dkHYCCgobiza6fq8L7+jIjdp0koj7jk1FmwBJxDu9lLAUrh50NQD/XPlPyuvLDY6oE6pvQ2m6RTvW5LRhctR7IipxLPp8595TPVeWDlrHbIDa0iMe4uqYHuaBFfGgrpgUMzWOSsoajt65XbhJwVYoz9KaNx6tW/rhUkZq3y/15ZC90mPhHW5htlZGe3K3k712TW/SR7FtKdpCddMpF8JjMkq11fCeUT07TAf+logPiXfd+Jmzd47B0XQuHblRm06fVS0N24xVY6txbQ8YHDfY4GgOkkTcINcNuY7uEd0privm6VVPy6qXt7lWxMNb/BKHNRQVrbGbrIobwOmADZ9oz4dd4tlrBUdrjzUtSMQ9sCJuMQWQ1NiwLbcmw+3nF83Y0TiCrOcJEBDS8teZzNB7mvZ816/uj6sZJXUlbCjUOorrXZ87muSwZFLDUnGoDleXW+FZu8p2AdA7quM0/mspfcugPg5QeF6dvc41QagzrIjvKtuF3em9qilxqK3FW3GqThJCEnyqikwScYMEmgN5ZMIjmBQT3+/5nq92fWV0SJ1LG0rTUUw4rNrxkogbYO9vUJELQVGtKx1ui1aUpnvqF3pySC8Acmt2e+T84jCu/eFt+N7qM1173OWdrUZLcpbgVJ30j+nvU28o3G1MF21VfHXeaoMj6Rx2lWqJeJ/oPgZH4n3Tu0/HYrKwo3SHqzJAeNau0l04VAcxQTEkhiQaHY7HpIWnEWIJod5Rz74K6ftiFFdZepzvlKWDJOKGGpE4gluG3wJoJerrC9YbG1Bn0obSdDi4T9wsDdu8b9Wb2uOQC8DastnvbaaviDdUaSOtDqOqqkebtQGkhmirUpKIe0FlHuQ2rrrqSXVr9DoRFBMUbCGwer97Y2vGouxFQMddDdfp5ekrD3iv5L8z0xu1dcYV8cjASI5POR6AH/f+aHA0nUNnmVlvUkyu8nS9FF94ny82agNJxA139aCrOSHtBBqcDfzf/P+T8Qbe0tD6rukgDdsMU5oJOxtXLEdf5/nrBUVC4zaE5vaJVzRUUGPXZoJ6KhFP0VfEa2V1xuP00WMpI9vWeyAkBlJHAxCXt9iNgf1Zg6OB3/f/DnSeRHx7yXbppeJhDY4G12pdZ0zEAU7reRoA32Z8i81pMziajk9PSgfEdNyO6bq+0bJP3Ggbi7RE3Jf2h4Mk4oYzKSaenvQ0w+KHUdlQyXW/Xse2Yrlj5nFtTcQbG7ZJIu5lq9/UZjX3PAHivVA2aTJDcJT2vJnydL0sPSYohiCLZ1bn9dL0kvo8au1SgeFR7SlL1zV2T4878JsbAjqyDYUbqLXXEhcc16EbHIHWRKtnZE9UVJYfWG50OB3a3vK9OFQH4QHhJIQkGB2OIU5IO4GYoBgKawv5LduzP8eic3RM10nndGPlVedRUFOAWTH73Kg8ScR9QLAlmJenvkz/mP6U1JVw9S9Xy544T2tzabqeiEti5DX1lbD2fe352Bu8d92jdE7XG7V5cn9uiCWc6ABt35yUp3tQQw3s0TqQ0/eUtp+nMRGPyV/m0akKq/JWATA6aXSHLufUTUqdBMDibM9WGnR2eqO29Kj0TvF91Ryr2co56ecA8OmOTw2OpmOzOWyu77mOfkMRDibiO0p2SHNmA2wp2gJo1T4h1lY0Y/UCScR9RGRgJG9Nf4tRiaOoslVx49wbZca4JzU0jsNxc2n6nsrN/GfH3Ty16Rq+3PcSVbay9kQpAFa9AXXlEJt+cGazN7g6p/95RdyTHdObOrhPXMrTPWbvb2Cvg8iukNCOO+VJgyG8C2ZHLVGFnruRuuqAloiPTRrrsWv4ksmpkwFYkrsEh9NhcDQdl96gLD063eBIjHVen/NQUFhxYAWZ5ZlGh9NhZZRlYHfaiQiIICUsxehwPK53dG/MipnS+lIKagqMDqfT2VqiVV8MjBtocCR/Jom4DwkPCOe1k17jxLQTaXA28PdFf+fj7R8bHVbH1Jau6TRNxP+8Ir6jfA2v7Pg7OyvWkF+3j6UF3/LU5qvJrNra7nA7rYZqWP6y9nzSHVrJuLeEHHtF3OOJeKj2pjirWsrZPEYfW9Z3JrRnJVBRIP0kAOIOLGp/XM2otde69rnp+6c7umEJw4gIiKCsvsz1tQv368yN2ppKCUtxVWG8t/U9g6PpuFzzwzt4ozZdoDmQHpE9ANhRKvvEvU3fEqBXJvgSScR9TKA5kOemPMcFfS5AReWfK//Ji2tflFKWFqqz1/GPJf/guE+O4x9L/kGdva75A+sbV7QDWz5HHI68Im5zNvDZvudxqg6GRB/HX3o9RJfgHlTbK/jPjrvYWbG21V+LQNsbXlMM0T1g0HnevXbwkUeYHajyTiLePUxbod0rN3M8w+mEnY2zv/vOaP/5PLxPfF3BOuxOO11Cu5AanuqRa/gai8nCcSnHAQe7xQv300eXdfZEHLQmuqA1bcuvzjc4mo5J3x/eGRq16fQkUPpAed/2YknERSuYTWbuH3c/fx32VwDe2PQG9/9+v3TxbIHn1zzP93u+p7y+nO/3fM8r619p/sA2l6Y336xtaf43lNTnEWmN5ZIedzMk5nj+1v9F+kSMpMFZx5s772d7+R+t/no6taoCWPys9nzSnWC2ePf6LSlND/NsIt41tB8KJkob8ilrKPLotTqlvA1Qlaf9Huh2XPvP13MKTpOVkKp9BFdmtv98h9HL0jvL/nCdXp6+IGuB3JT2gKqGKvY3jt3r7KXpoI2WHZEwApvTJqviHqIno52hUZvOtU9cVsS9qri2mILaAhQUV/d6XyKJuI9SFIUbht7AIxMewayY+W73d9y39D7ZI3cUuVW5rgYrZ/Q6A4CPtn1Ead2fS4vbXpr+52ZtTtXJkoJvAZiRchWB5mAAAs3BXJf+GIOixmNTG3hr1wNsK191zGvYnA1kV+9iR/kacmsyOu+/+fxHoL4CkofD0Iu9f30fKE0PMoeQHKKVs2VWbfHotTolfTW85xSwBLT/fIHhlMaNAjxTnr62QKusGZ002u3n9mWTUicRaA4ksyJT5vB6wO5yrRlkQnACkYGRBkfjG64fcj0An+/4XFbF3czutLuS0c7QqE2nzxKXzunepf//3S2im881agNJxH3eOenn8PyU57GYLPy892ceXfEoTtVpdFg+6cudX+JQHYzrMo7HJz7OgNgBNDgb+H73938+2NU1vf2l6XurtlDakE+gKYQRsScecrzFFMCVvR5kUNQE7KqNN3c9wMK8z3GohybXDc56NpYu5YPdT/DAunN5butNvLbzbp7dciNTPpvC6xteP3KZfUeUswbW/U97PvMZMBnwq0pfET+sNN3mtFFYUwh4tmu6rnuY1lxkryTi7rdzjvbYxw1l6Y2Ku0wB3F+ebnPaXOWcQ+OHuvXcvi4sIMw1M/3HPT8aG0wHpDdq6x0tZem6CckTGJ4wnDpHHS+vf9nocDqUveV7qXfUE2oNpWtEV6PD8Zp+0dqKeHZlNlUNMnnHW/Sbt75Ylg6SiPuFE7qewNPHP41JMfHVrq/499p/Gx2Sz1FVlTmZ2pvqc9LPQVEU16r4vKx5hx/c9jnizSTia4q18w+NOZ4AU+CfXmMxWbmy1wOMjJmKU3XwXfbrPLXpL3y17xV+zHmLN3bezwPrzuWdjIdZW7KQemctoZYIugR3J8gcQll9GS+vf5krfr7CtTe5Q3M64ec7tedDL4E0g1b/XIl42SEfzq/OR0UlwBRAbFCsx8Po0ZiIS9M/N6sqgP2NvRvc2I2/qItWRh1duAqzrdpt591ZupN6Rz0RARF0i+jmtvP6i1N6aKPlftr7k2zTcjN9jJTsDz9IURTuGHUHoO0Vl1VM92maGJmUzpOGRAVFuW7e7yzdaXA0nYcvN2oDScT9xsndT+bRCY8C8Pbmt/km4xtjA/IxW4q3kF2ZTbAl2LWfcGrXqQCsL1hPZUOTPd22GqBxn2Gbu6Zr51NVlc1lywEYEXPiEV9nMVm5tOc9nN9tFqGWCIrq97Ok4GvmHfiYreUraHDWERUQz5TE8/hb/xd5dNgX3DXoTR4f/jVPHf8U0YHRbCvZxjW/XtPxR19s+Bhy10BAOEx7yLg49NL0w/aIN90f7o19unrDtpyaXTQ4OlFVhKftahwP2WUYhCe67bQ14T2oCU3D5LQRU7DcbefdVLgJgMFxgzvVm1fd8SnHExsUS1FtEQuzFhodTocio8uaNyR+CDO7z0RF5fEVj3febWJuplf2dKaydJ2+Ki5bbLxnR4lvb4PofH/N/diZvc/khiE3APDI8kdYk7/G4Ih8x8Js7Y3ZpNRJrj0gSaFJpIaloqKysbDJ2Bu9LB2l3XvE8+r2UWkrwWoKpGf44KO+VlEUJiScxv1D/sdlPe/lhKTzOS7hTM5Iu4E7Br7Og0M+4syuN9I9bIDrjbZZMXNqz1P55LRPSAlLIbsym78t+BsNjoZWxe036sph3sPa88l3QbjnS7+P6Ail6d7aH66LCUgi0hqHU3VIebo7eaAsHQBFoaixPD3WjeXp+u+wIfFD3HZOf2I1Wzkn/RwAPtnxicHRdCz6inh6lCTih7t91O2EWkPZULhBvu/cRG/UNiC283RM1+n7xPXkUHhWja2GfRX7AOgXKyviwg3+b9j/cVK3k7A77cxaOIvcqlyjQ/IJ6wvWAzC2y9hDPj4sYRigjf1xaVqW3soVzcNXxHdVaOftETYIq6llzZ6CzCGMjJ3KGWk3cG63Wzgh6XxSQnoddXU1OSyZN05+g4iACDYXb+b5Nc+3Km6/8dtsqC6A2HQYe6OxsQQ336zNW6PLdIqi0DdyJADby1d75Zodnr0BdjeuqvZxX1m6rrixPD1+/wJw0yrapqKDK+Kd1fl9zsesmFmdt9pVISDap7i2mJK6EhQUekb1NDocn5MUmsTtI28H4N9r/01meaaxAfk5p+o8OEPcR1coPUkvj5atDt6xo3QHKioJIQnEBMUYHU6zJBH3MybFxBPHPcGA2AGU1Zdxx6I7Ou7qaAvZnDbXm9Rh8cMO+dzwhOHAwUQdaHPHdDiYiJsddShOG7sa54P3iRje6nO1Vlp4Gv887p8AfLjtQzYXbfb4Nb2qcAesfE17PuMp93Sxbg+9NN1eBw01rg97a3RZU/0itX3y2ytkBJ5bZC2DhkoITYAu7v/ZLUkYhy0gksC6QqKL2n/zpLy+nMyKTKBzJ+Jdwrpwas9TAXht42sGR9MxZJRpZelp4WkEW4INjsY3ndfnPMYmjaXWXsvff/t752qc6mb7KvZRa68lyBxE98juRofjdXoinlGWIb0uvECvvvDV/eEgibhfCrYE8/yU512ro8+sfsbokAy1s3QntfZawgPC6RXV65DP6SviG4s2YnfatQ+6Oqa3rlEbgMN68DXmhkr2VGrJcO/wYa0+V1tMTpvMaT1PQ0XlkeWPHPya/J2qwpx7wGmHvqdA+jSjI9IqJkyNs8ublKd7uzQdoE/ECBRM5NVmUlrfwXsEeIM+tiz9ZI905FfNARSkaCvtiVk/tPt8+k23bhHdiAqKavf5/Nn1Q67HpJhYnLPYNVddtJ2eiEujtiMzKSaePP5JYoJi2Fm6k6dWPWV0SH5LT4z6xvTFov997URSwlIIs4Zhc9rYW77X6HA6PF9v1AaSiPut5LBknjz+SUDbL/fTnp8Mjsg4+mr30Pihf2pi1DuqNyGWEGrttWRVZGkfbGPHdADVZMHROCe8rGYPNY5KzIqVlJBex3il+9wx6g4iAiLYXrKdL3Z+4bXretTOX2D3AjAHwPQnjI5GoyjNlqfvr9oPQHJostdCCbVEuJq2bSxd4rXrdliu/eHuL0vX5XU9DYDEnF9Q2lm1pJdyDojpfHsqD9ctohvn9zkfgCdXPYnNIatK7bGrVNsffvhNbHGo+JB4np70NAoKX+76ks92fGZ0SH5Jb9Tmy4mRJymKIvPEvUj//9iXt0FIIu7HJqVO4rrB1wHw8PKH2VO2x+CIjKEn4oeXpYN2J1u/07+zrHFcREPbZojr9PL07CrtBzwlpCcWk7VN52qL2OBY/jr8rwC8vvF1amw1x3iFj3PY4Nf7tOfjboIYH9qn6GrYpiXiqqqSV50HeHdFHGBYjLbveF3JIq9et8Mp3g0lu8FkhZ4neOwypfFjqA9KwNpQTmz+7+06l97Yx1ebzXjbLcNvISowioyyDF5Z/4rR4fg1PRHvE9PH4Eh837gu47hl+C0APLHyCX7Ldl8zxs5iS7HWcHRg7ECDIzGOfhNCrw4QnmFz2FyNKH35xo8k4n7u5mE3u/Yu3bboNv9PytpAb8Sm7wc/nD6SRX/D4SpNb8MecTjYOT2rtnFvXWjfNp2nPc5LP4+UsBSKaov4aPtHXr++W61+E4ozIDQejr/D6GgOFRSpPdaVA1BaX0qdow4FhcRQ9428aolhMZNRMLGvehvF9Z1gnryn7PxFe+w2AYIiPHcdk5n8tJlA+8vTXeV10b77ZsKbIgMjeWi8Ntrw7c1vM2/fPIMj8k9O1el6o9onWhLxlrh28LWc3ftsnKqTOxffyZYimWTRUk7V6VoRHxjXeRNxfXVWvykhPGN3+W7sTjvhAeGkhKUYHc4RSSLu58wmM09Neor44Hj2lO/h0RWPoqqq0WF5zYGqA+TX5GNWzAyKG9TsMfqKuD4rtT2l6XBwRXxfnVbqnhbi/TcwVrOVm4fdDGhvRKtt1V6PwS1qSmBR4367E+7zbGLUFocl4vr+8LjgOALM3m0mF2GNIT1iGADLC3706rU7FFdZ+nSPX0ovT4/fP/+Qhn+t0XT8iqxaHjSt2zQu6nsRKip3L75bxnm2QU5lDrX2WgLNgXQN72p0OH5BURQeGP8AE5InUGuv5f/m/1+nrUZsrcyKTGrsNQSZg+gZ6UOVb16m9y7aUrSl0zdb9qSmjdqONpXIaJKIdwBxwXE8O/lZzIqZH/f8yOc7Pzc6JK9ZX7ge0Bp/6PPDD+daEW+8809DY9LahmZtoCXiKpBp00qU00KNeXN8So9T6B7RncqGSj7f4af/5r89DXVlkDgIRlxhdDR/dngiXuX9julNHZdwJgDLC3+kwVlvSAx+ra4C9i3Tnqd7PhGviBlCTWgaFnsN7Py5TefYVbYLFZW44DjiguPcHKF/u3vM3ZyQdgINzgZumncTi3MWGx2SX2m6P7wzNs5qK6vJyr8m/4v+Mf0pqSvh2l+vPdiDRhyRXj3QL6Zfp/5+6xrelejAaBqcDa7+H8L9/KFRG0gi3mGMSBzB30b8DYCnVj3lKv/p6I5Vlg4HV8RzKnO00v16bQZ4e1bE881matUGTIqZxCBjVhLMJjNXD7oagPe3vu9/d1aLdsGqN7Tn058Ak9nYeJoTHKU9HrYi7u394bqBUeOICUiixlHJisLO26CxzfYsBKcNYnpBnBe6RCsK+V21cVts/qpNp9D3h+sNfsRBFpOF2ZNmMzFlIrX2Wm5dcCufbP/E6LD8xs5SrW+KlKW3XlhAGK+f9Drp0ekU1hZyza/XkFuVa3RYPk3K0jWKojA0YShw2Ghd4Vb+0KgNJBHvUK4aeBVT0qZgc9q4fdHtVDRUGB2Sx7katTWW+jQnNjiWmKAYVFRtFm+7S9PDyAjQmrPFB6ZiNvDO7mk9TyMhJIHC2kK+3/29YXG0ydyHQHVAnxnQc4rR0TTvsBVxIzqmN2VSzEztchEAv+7/gFp7lSFx+K1djWPLvFCWrtP3iZMx72B/ilaQ/eFHF2QJ4qUTX+KMXmfgUB08sfIJHl3+qHRTbwE9EU+PSjc4Ev8UHRTNGye9QY/IHuRV53HNL9e4mnmKP5NGbQfpzYU3FG4wNpAOyqk6XX87ff0mtiTiHYiiKDw+8XFSwlLIrcrlgaUPdOj94jW2GnaUaqtFzXVMb0rf/5ZVmeWW0vTdVi0RTwru1qZzuIvVbOXKAVcC2l5xh9NhaDwttm8Z7PgRFDOc9KjR0RzZYYm4/iYrKTTJqIgYGz+TxKCuVNsr+Cb7P4bF4XdUFXYv1J73nuq1y1ZF9qM6rDvY6w7uT28FV8d0Hy+vM5LVZOXxiY8za8QsFBQ+3/k51829jpK6EqND82muFXHpPdBmscGxvHnym3QN70puVS7X/HIN+dX5Roflc+xOuysx6uwr4nCwinNdwboO/T7dKDmVOdTYawgwBdAjsofR4RyVJOIdTGRgJP+a8i+sJisLshfw/tb3jQ7JYzYWbcSpOukS2uWYiVHXCC0Rz67IdkPX9HB2B/hGIg5wXp/ziAiIIKsyi4XZC40O59hUFX69X3s+4gqI9+G7lXoiXlsGwP7qxhXxMGNWxAHMipnzu89CwcSqol9YUdi2vcedTtFOqMgFcyB0neC96yoKBWkztOdbvm7VSw/pai3J0lEpisI1g6/hpRNfItQaypr8NVz8w8WuGxniUDW2GrIrswEpTW+vhJAE3pr+FilhKWRVZnHtr9dSWFNodFg+ZW/5XmrttYRYQuge0d3ocAw3IHYAFpOFotoicqpyjA6nw9H33qdHp2P14njhtpBEvAMaGDuQu0ffDcDza5537aPuaI42P/xwaeFpgL4iru8Rb+sc8bAmK+Ld23QOdwqxhnBh3wsBeGfLO75/d3XLV5C7RtsaMOVeo6M5uiOsiBu1R1zXK3wIJydfBsBnmc/zR5GMbzomfTW823gIaL6xo6e0tTz9QPUBau21WE1W6WrdQpPTJvPRKR/RNbwr+6v3c/nPlzN331yjw/I5u8t2u5oAxgTFGB2O30sKTeLt6W+THJpMZkUm1/56LUW1RUaH5TP0svQBsQMwKZJ6BFmCGBA7AEAmPniAvzRqA0nEO6wL+l7AzB4zcagO7vjtjg5ZoteS/eG6bhHaynVWRftL022WMNeKeKIPrIgDXNL/EqwmKxsLN7o6yfskez3Me0R7PvFvEO7dWdyt1iQRr7XXun6OjOqa3tT05MsZFzcTFScf7n2Kn3Pfxak6jQ7Ld+1eoD32OtHrl66K7AfRPbTy9D2LWvy63WW7Aege2b1TdxlurZ5RPfno1I8Y32U8tfZabl90O6+uf1V+PpqQRm3ulxyWzJvT3yQxJJE95Xu47lfZHqHTO6bL/vCDxiaNBWDFgRUGR9Lx6Cvivt6oDSQR77AUReHh8Q/TI7IHBTUF3LP4Hv/ZP9wCDqfD1eTiaB3TdYfsEW9naXqBWaXaZMKsQnxgSpvO4W5xwXGc3ut0AN7d/K6xwRzNiv9A2T4IS4LxNxsdzbE1ScT11fBQayjh1rZVU7iToiic3/02TkzSqiF+3f8/3s14lHpHrcGR+SB7PWQu0Z4bkIijKJB+svY8o+Wrs/p84l6RvTwRVYcWGRjJq9Ne5bL+WuXIfzb8hydWPOH7FUNeIo3aPCMtPI23p79NQnACGWUZXPfrdZTVlRkdluE2Fm0EZH94U+OTxwOwYv8K+b3kZtuLG1fEY2VFXBgoxBrCc5OfI9gSzPIDy/nvxv8aHZLb7C7fTZWtimBLsGtO+NGkRWil6UW1RdS0s2t6llqjndMBFh/ae6I3bVuYvZDM8kxjg2lOWZY2Nxxg2kNtvhHiVUFR2mNd+cEZ4qFdUBTFuJiaMCkmTk+7jot73IlZsbKpbCn/3nYLZQ1SEnmI7FVgq4HQBEgw6I2gnojvmqv1SWiB3eXainjPqJ6eiqpDs5gs3D3mbh4e/zAKCp/t/IynVj0lb3rB1ei0JX8/Ret0jejKW9PfIi44jp2lO7lu7nWU15cbHZZhamw1rl4NLdlK2FkMjR9KkDmI4rpiMsoyjA6nwyisKaS4rhiTYvKLih9JxDu43tG9eWDcA4C2IrBs/zKDI3IPvSx9SPyQFpVsRgREEB0YDUC2Q0ukCWzbqma2U/uD2svuWxUGPaN6Mjl1MioqH2z9wOhwDqWq8NOdWjLU7TgYerHREbWMviLeUMmBSq2hitH7w5szJm46f+33L8KtMRyozeTV7X+XZkFNucrSTwCTQX/2uk8ES5DWMK5ga4teIivi7nFun3N5dOKjKCh8tP0jnv3j2U6djDucDrYVa6Wb+j5V4V7dI7vz1vS3iAmKYXvJdq6fe32nGCnbnM1Fm3GoDhJDEn1iW5evCDAHMDJxJCDl6e6kl6V3j+hOsCXY4GiOTRLxTuD0Xqdzbvq5qKjcu+TeDjFaQ29A15KydJ2+Kr6PBu0DbVyR3W8vBaBnfX2bXu9JVw7UVsW/3f0txbXFBkfTxJp3tNFNJiuc9pxWqusP9EQc2F+xDzC2Y/rRdA8bwKz+LxEdkEhhfS7Xz72eGluN0WH5hj2Njdp6nmBcDNZg6KqVIpL5+zEPV1XVtSLeK0oS8fY6q/dZPDT+IQDe3/o+725519iADJRZkUmNvYZgSzA9I6XawlN6RvbkrZPfIjowmq3FW7lx7o1U6s1iO5G2vF/rLMZ1GQdIIu5O/tSoDSQR7zTuHXsv/WL6UVJXwp2L78TmtBkdUru0pmO6zrVP3GLWPtDG0vQCu9Z8pUdDDfjYvvtRiaMYGDuQekc9n+741OhwNHmb4Od7tOdTH/TtcWWHM1vBqt2wOVCZBRg7Q/xYYgIT+b++zxBhjSWjLINHlj/SqVf+AKguhv3rtee9DEzEQVsVB9h37EQ8vyafals1FsUiHdPd5Nw+53LnqDsBeG7Nc/y8t3OO/ttctBnQGhmZTWaDo+nYekf35o2T3yAqMIpNRZv4v3n/R629c/Xx0BvItqSxbmej7xNfdWCV3Dh3E0nEhU8KNAfy3OTnCLOGsa5gHS+ufdHokNpMn7uooDAkfkiLX+eaJW5tLGVv44p4oU2rKEiz2bHYq9t0Dk9RFIWrBl0FwCfbPzH+D37pPvjwAnDUQ/p0GP9XY+Npi8ZV8dwqbYZ4aniqkdEcU1xQMlf2uh+zYuanvT/x1a6vjA7JWJmLARUSBkC4wTdRuumJ+LJj7hPXy9K7RnTFavadXhT+7oqBV7gauN239D7+yPvD4Ii8b1PRJgAGxQ0yOJLOoW9MX944+Q3CA8JZX7ieu367C7vTbnRYXuFUna7GupKI/1mf6D6khKVQ56hjae5So8PpEPRtN/1jfb9jOnggEXc4HDzwwAP06NGD4OBgevXqxWOPPXbIqoyqqjz44IN06dKF4OBgpk2bxq5du9wdijhMWkQaj018DIB3t7zLgqwFBkfUNnqZU+/o3oS3Yha4vqq0z2IBawi0YSXA7mxwNcJKs9mx2HyvzGxa12mkhKVQWl/K97u/Ny6QrJXw1slQuR/i+8HZrxm3P7c9GhPxnBrtBkxqmG8n4gA9wwfztxF/A+Bff/yrc8+zzWx8c9NjkrFxACSPAHMgVBdA8e6jHipl6Z5zx6g7mNZ1GjanjdsW3UZuVa7RIXmVPkpqcNxggyPpPPrF9OPlE18m0BzIopxFPLbisU5RrbS7bDeVDZUEW4L9onGWtymKwkndTgJg3r55Bkfj/8rry8mp0vr5+MPoMvBAIv7000/zn//8h5dffplt27bx9NNPM3v2bF566SXXMbNnz+bFF1/ktddeY+XKlYSGhjJ9+nTq6urcHY44zLRu07h8wOUA3L/0frIrsw2OqPX0FYyRCSNb9Tp9JTPXamlzWXpxfR4qKqFOlRin0ycTcYvJ4vo3fn/r+94dW1dfpTXG+vJaeHs6VOVBfH+4/GsIifFeHO4UFEmdolDQoDXp84dEHOCKAVcwMHYglbZKZq+ebXQ4xtH3Y+ur0UayBkFK4++t7KPvCdRniMseXvczm8w8efyTDIwdSFl9GX9b8LdOUxZqc9hcHdNllJR3jUgcwexJszEpJr7a9RUvrXvp2C/yc3/ka+/XhsQNwepDU2Z8iZ6I/5bzG/UO3+s95E/0svSUsBQiAyOPcbRvcHsivmzZMs4880xOPfVUunfvznnnncfJJ5/MqlWrAG01/IUXXuD+++/nzDPPZMiQIbz//vvs37+fb775xt3hiGbcNvI2hsYPpdJWyd8X/d3vfvD1X+yjkka16nV6ApVvNtMQENKmaxfVa+XJKQ4FBXwyEQc4u/fZRAREsK9iHwuzF3ruQqoK2ath/qPw3xPgqa7wwdmw6XNA1bqjX/MrRPhmg7MWCYpkf2NfgTBrmN/8cjebzDw4/kFMiomf9/7cKUtwqS6GQq1MzScScYCUEdqjvm/9CPaUN3ZMlxVxjwiyBPHCCS8QExTDjtIdPLTsoU6xQrmzdCc2p42owCi/uanYkZzY9UQeHPcgAG9seoNPt/tILxcPWb5/OQDjkscZHInvGhQ3iMSQRGrsNSzL7RiTjYzij9Mg3J6IT5gwgfnz57Nz504ANmzYwNKlS5k5cyYAe/fuJS8vj2nTprleExkZydixY1m+fLm7wxHNsJqsPDv5WaICo9hWso3Zq/xntaysroydpdr3lj72oaVigmIINgWgKgoHgtqYiNdpJYzJqrbP3GKratN5PC3EGsKFfS8E4JX1r+BUne6/SP4WbdX7rWmw5F+wfy2oDohMg+GXw/WLtHL0oAj3X9ubgiLJsWj/3qnhqT4zQ7wlBsQO4Lz08wB4fu3znSLROITeFC2+P4TGGhuLLrmxc/CB9Uc8RFVVWRH3gqTQJJ6b8hwWxcKczDm8vflto0PyOH2/7sDYgX71u6wjObfPudw87GYAnlz1ZIcZK3s4u9PO6rzVwMHu4OLPTIrJtSr+/R4DtxN2AFtLtNGg/lKWDh5IxO+55x4uuugi+vXrh9VqZfjw4cyaNYtLL70UgLy8PAASExMPeV1iYqLrc4err6+noqLikP9E+ySFJvHU8U+hoPDZzs/4cc+PRofUImsK1gDQI7IHccFxrXqtoiikBEQBkGMNatP19RXxZLTX++qKOGijzMKt4WSUZbi/O/CmL+C/UyB7pbbndeA5cNZrMGsz3LYZznz5YMLh74IiXQ3+/HEF6cahNxJsCWZj4UYWZPtnX4g20/eHd/eR1XA4+HORtwkczU+vKK4rpqKhApNiontkd+/F1gmNTBzJPWO0qQ4vrnuxw69I6RVlIxJHGBxJ53bDkBs4o9cZOFQHd/x2B3vL9xodktttLtpMla2KiIAIv0qMjHB2+tkALMxa2Ll7urSTvzVqAw8k4p999hkffvghH330EWvXruW9997j2Wef5b333mvzOZ988kkiIyNd/6Wlpbkx4s5rYspErh9yPQCPLH+ETYWbDI7o2PTy2lGJrStL16VatdXZHGvbRrboiXiSSdtj7suJeGRgJH8Z9BdAWxV328i6Ld9oe8AdDVon9L9tgPPfgWEXQ1QH/NkMjjpkRdzfxIfEu7pEv7zuZc9UR/iqfT60P1wX3QMCI8FeB4Xbmz1EXw1PC08j0Bzozeg6pQv6XsA56efgVJ3cteSuDtu8TVVV1uRrN7Pb+jdUuIeiKDw0/iGGxQ+jsqGSWxbcQnl9udFhudXyA1qV69guY2VM3jH0ie7DkLgh2FU732R8Y3Q4fqnaVs2+in2A/4wuAw8k4nfeeadrVXzw4MFcfvnl3HbbbTz55JMAJCVp42Py8/MPeV1+fr7rc4e79957KS8vd/2Xne1/DcZ81U1Db2Ji8kRq7bXcPP9mMsszjQ7pqPQ3EaOTRrfp9almrSQ9p43f+UV1jYm4Wdsn7MuJOMCl/S8lJiiG7MpsvtrphjFW+Vvgm5sAFUZcCRd/AhFd2n9eX9a0NN0PV8QBrhp0FWHWMDLKMliY5cGeAb6kpkT7fgXfSsRNJkgeqj0/wj5xKUv3LkVR+MfYfzAwdiDl9eXctvA26uwdr3ns3vK9lNSVEGgOlNFlPiDAHMALJ7xAl9Au7KvYx98X/d19N8x9wIr9WkNKfVa2OLoL+2nbCT/c9qHf9W7yBTtKdqCikhCS0OqKWSO5PRGvqanBdNiIIrPZjNOprcL06NGDpKQk5s+f7/p8RUUFK1euZPz45n9YAwMDiYiIOOQ/4R5mk5l/TfkXA2IHUFpfyo3zbmR/47xkX1NUW8S2Eq3spM0r4qYAAHKV1ncSd6gOShoat1ZYtP2mZh/dI64LsYZww5AbAHhp/UuU1pW2/WQOO3x9I9hqoNeJcNrz/jmOrLWCIsmx+u+KOEBEQAQX97sYgNc3vt459opnLQdUiOsD4YnHPNyrEhuToIJtzX5aGrV5X6A5kOenPE90YDTbSrZ1yPFSq/K0prnD4ocRYA4wOBoBEBscy0snvkSwJZiVeSt5etXTRofkFmV1Za5+BOO7SCLeEjO7zyQpNImi2iK+zfjW6HD8jp4f+FOjNvBAIn766afzxBNP8OOPP5KZmcnXX3/Nc889x9lna/sfFEVh1qxZPP7443z33Xds2rSJK664guTkZM466yx3hyNaINQayqtTX6VreFdyq3K54ucrXG8EfcmSnCWA9kMWHxLfpnOkNjZZy1EbWv3a0vp8nKoDi2Ilwqol4lYfXxEHreyyT3QfyuvLeX7N820/0ar/Qt5Gba722a+3aQ67P1IDI8htXBFPCUsxOJq2u3zA5QRbgtlWso2luUuNDsfz9jXu9e02wdg4mhPfWDZX2HwiLivixugS1oVnJj+DSTHx3e7v+HRHx+porf/cj+0y1uBIRFN9Y/oye9JsFBQ+3fEpH2//2OiQ2u23nN9wqA76RPfx2xvY3mY1W7lq4FUAvLbhtU4zUtFdthZrjdoGxHTyRPyll17ivPPO4//+7//o378/d9xxBzfccAOPPfaY65i77rqLW265heuvv57Ro0dTVVXFnDlzCApqWwMt0X6xwbG8Nf0tekT2IL8mn8t+vIz5WfOP/UIvWpyzGIApqVPafI7Uxu2xOY7aVr9W3x8eG5iMo3GElaXB9xsHWkwW7h93PwBfZ3zNygMrW3+SyjxY+IT2/KRHISzBjRH6thKzmVqTCUWF5DD/HcMWHRTN+X3OB+C/G//b4Vb7/iRH69ZLmg8mHQmNjWRkRdznjO0ylttG3AbA06ueZn3BemMDcpM6e53rd/+k1EkGRyMONyVtCrNGzgK07zt/76Q+L2seANO6TjvGkaKp8/ucT0pYCoW1hby1+S2jw/EreiLuT43awAOJeHh4OC+88AL79u2jtraW3bt38/jjjxMQcLAMSlEUHn30UfLy8qirq2PevHn06dPH3aGIVkoKTeK9Ge9pzUNslcxaOIt7ltxDfnX+sV/sYbX2WtcfpklpbX8TkWzXStIrVVurG6MUNybicUHJ2AO0RNza4B/NVYYnDOeCPhcA8I8l/2h9ifqS56ChClJGwfArPBCh78puvGmT4FT9vpzzyoFXEmAKYH3helf35A7JXn9w/3XqGENDaZa+Il55AGoP/VksqSuhpK4EBYUekT0MCE5cOfBKpnefjl21c/ui2ymsKTQ6pHZbnbeaOkcdiSGJ9ImW91u+6C8D/3Kwk/oi/+2kXtlQ6ZoffmLXEw2Oxr8EmAO4feTtALy96W1XcimOrtZe67qB7W8d+jvBBk/RGtFB0bw9422uHHAlCgo/7vmRGV/N4K7FdzE/a75hXT0XZC2gxl5DSlhKu37Igm21xDUm4zlVOa16rd6oLS4wGVuA3qzNPxJxgL+P+js9IntQUFvA/b/fj8PZwn3yFfthzbva86kPdI594U3ss5UB0N1mNzYQN0gISXCNSXl94+sGR+NBBzaCox6CYyDWB1eVgyIgorFcs+DQzul7yrQ3E8lhyQRbgr0dmaBxsWDCo/SO6k1hbSF//+3v2I4was5f6BVuk1InyfxwH3VIJ3Wb/3ZS/yXzF+od9fSM7Ck3fdrgpG4ncVK3k7Crdv6x5B8dsnGku+0q3YVTdRITFENCiH9VbHaud9SiRawmK3eMvoOPT/uYkYkjsTvt/Lz3Z2YtnMVxnxzHiZ+dyNW/XM19S+/jxbUv8tmOz1ics5gdJTsory/3SMnrd7u/A+D0XqdjUtrxbVtfSapdS6hyKluZiNdrI23igpKxNY5Bs/pBabouxBrC7EmzCTAFsDhnMU+vfrpl/1ZLn9eSmm4TocdkzwfqY/bVFQPQraEOnP4/+uvqQVdjUSysPLCyw5Td/kmO1pSKtDHgq0lHQvP7xKUs3TeEWEN44YQXCLOGsa5gHQ8vf9hvR//V2ev4NfNXAGb2mGlwNOJo/tRJ/Tf/66SuNxo7q/dZctOnDRRF4YFxDxAbFMvu8t08vPzhjr+VrJ22FGsTUvrH9ve77zmL0QEI3zUwdiDvzniXbcXb+CbjG5btX0ZmRSaFtYUU1h65VC/YEkxiSCJp4Wn0i+lH/9j+9I/pT0pYSpt+QLIrsllxQBuDcUbPM9r89QDQUEWK3c56Als9K7ao/gCgrYjbiQLA4iel6bp+Mf345/H/5I7f7uDj7R8TERDBzcNuPvK/S20ZrPuf9nzy3b6b1HhQZo3WKb+7zQ4NlVqzOj+WHJbMGb3P4KtdX/Hahtd47aTXjA7J/bKbJOK+Kq4vZMyDooxDPqw3ausVKYm40bpFdOPpSU9z64Jb+W73d4QHhHP36Lv97o3eopxFVNoq6RLahZGJI40ORxyD3kn98p8vZ+WBldy75F6ePv5pv5jFvbN0J+sL12NSTJzW8zSjw/Fb0UHRPDXpKW6ceyM/7vmRHhE9uGHoDUaH5bM2FW4CYEjcEIMjaT1JxMUx9Y/t72p+UNFQwb7yfeyr3EdedR551Xnk1+STX51PXnUepfWl1NpryazIJLMikyW5S1zniQyMZEzSGMZ1Gcek1EkkhTY/N57qYpj/MBTugIFn86bjAE7VyXEpx5EWkda+L6a+ilRH61fEnaqTYldpegq2xu7rVlsFqE5ozyq9l03vPp386nye+eMZXt/4OmX1Zdw95m6sJuufD97wsTauLGEg9OicDX72VmYB0N1mg3r/T8QBrh18Ld9mfMvv+39nY+FGhsT73x+vo9ITcV/cH66LbeyIXnLohAo9EZf94b5hUuokHpv4GP9Y+g8+3PYhAaYAbht5m18l459u17q/n9rz1PZVlAmv6RvTl+emPMctC27hl8xfCDIH8ejER33+3++9Le8BWpO2tk63EZpxXcbxj7H/4LEVj/Hy+pdJDkvm9F6nGx2WT9pYtBHAL9/LSCIuWiUiIILB8YMZHD+42c/X2evIr9GS8j3le9hesp1txdvYVbaL8vpy5u6by9x9c1FQGNNlDGf1PouTu518sAlWXQW8ewoUavsmM/LW8l2q1qlan4fdLg1VpKqtT8QLawqxqQ2YFDPRgYnYndo5FNWJ2VaNIyC8/bF50RUDr8BqtvLkyif5dMenbCvZxtPHP33omBFVhdVvas/HXNspV8OdqpOsiiaJeF0F+H8eTlp4Gqf3Op1vMr7hPxv+w3+m/cfokNynPAcq94NihpQRRkdzZDGNK94luw/58O5y7X/3jurt7YjEEZze63QqGyp5ctWTvLPlHYpqi3howkMEmgONDu2Y1hdojRktJgsX9r3Q6HBEKxyXchzPTnqWv//2d77d/S02p43HJj7ms01D86rz+GnvT4DW8FC03wV9LyCrIov3tr7Hg78/SGxwLBOSfXAkp4HK6srYV7EPgMFxzecmvsy3b60JvxNkCaJbRDfGdhnLxf0u5pEJj/DZ6Z+x6pJV/O+U/3HzsJsZnjAcFdVVcnXSFyfx4toXOVB1AOY9pCXh4V2oGXs998THYkdlStIYhiUMa3+A9VppOtCq0vSsxlXRmIBEzIoZpzkQh1kbt2dtKGt/XAa4uN/FPD/lecKt4Wws3MhZ35516OzKPYugOAMCwmHwBYbGapQD1QdocDZgVRs77tf7T0+AY7l+8PWYFTNLc5e6yro6BH01PGkQBIQaG8vRxDSuiJdmQmPjxPL6copqiwDoGSUzxH3JJf0v4dEJj2JWzHy/53su+uEidpTsMDqso1JVlZfWvQTAGb3OOHIVmvBZU7tN5cnjn8SiWPhp70/cNO8mn23g9tK6l7A77YxOGu2XK5O+6vZRtzOz+0zXFIftJduP/aJORF8N7x7RnchA/1spkURceIXVbGVo/FBuHHoj7898nznnzuH/hv4fCSEJlNSV8MamN5jx5Qz+lvU9c0JD+H7itVzWsJsdgQFEOxw85IxpfxCqCg1VpDV2v95ftb/FncOzK7MBbX+4zhbQ2LDN5r/J2dRuU/ns9M8YnTSaekc9r6x/hZO/PJn/bPgPxasa9w4PuxgCw4wN1CCZ5ZkAdFVNmEErTe8g0iLSOLXnqQC8sv4Vg6NxI38oSweITAVzADgatFV8DpaldwntQqjVh28idFJnp5/Nq9NeJSYohoyyDC744QIeWvaQq8Ger/km4xtW5a0iyBzEdYOvMzoc0UYze8zklWmvEGoNZVXeKi74/gKfa7S5uWgz3+/+HoDbRtxmcDQdi0kx8fhxjzM6aTTVtmpumndTq3scdWQbC/23LB0kERcGSQlL4aZhN/HLub/w/JTnGZM0BidOFoQGc2dCHP/Y8R67ynYRZQnhxfxC4jZ/41o1arOGakAl3uHAarJiV+3k17RsRrorEQ9KcX3Mbm0cYeZnDdsOlxqeylsnv8Uzk56hW0Q3yuvLeXX9q0yr38LtCXEs6z7ab7sFt1dmRSYA3ZXGEtQ6//63PtwNQ27AYrLw+/7fWZa7zOhw3MPVMX2ssXEci8kM0Y37wBvL0/WydFkN910Tkifw5RlfclK3k3CqTr7a9RVnfnMmV/58JV/v+prKBt+4Wbe3cgtPrHwCgP8b9n+HbjsSfmdC8gTem/EeqWGp7K/ez1VzruKV9a/4xFg9u7OB+5fej4rKqT1PPeLWRdF2ejf99Oh0imqLfLoywtv0RHxo/FCDI2kbScSFoSwmC9O6TeOt457mm/2FXFJeybCIXgyLH8ZfBv2F78/+gWFKMFQXQPbK9l2soQoAs2IiOVRb2W7pXUV9n3BsYBfXx/RZ4v40wuxIFEVhRo8ZfHvmt8yeNJtBATHYFYW5oSHcsPoxTvnqFN7Y+AaFNUfult8R6Svi3cyNq5MdaEUcoGtEVy7qexEAz/zxTMtny/sqW602QxwgbbSxsbSEPuO8uDERb1wR7x0p+8N9WVxwHM9NeY4PZn7AlNQpmBQTawvW8uCyB5ny6RRuW3gb8/fNN+TnSVVV1hTP57Wdd1PvqGdK6hSuGHCF1+MQ7tc3pi+fn/45p/Q4BYfq4LUNr3HRjxexrXjbsV/sQV9mvczu8t3EBMVw9+i7DY2lI4sIiODVqa+SGJLI3vK93LboNv//m91OTtXJpqLGjumyIi5EO2z+kl71tdwb2I0Pzv6GD075gNtH3k5USDykT9eO2TW3fdeo1xJxAsJcqwMtbdjWXGm63ZWIl7UvLh9iNpmZmTaVj3P280XuAS5OGEt4QDi5Vbm8uO5FTvriJGYtnMXS3KWdYpXctSLe+G/dkfaI624ceiMRARFklGXwdcbXRofTPvvXg9MGoQkQ1c3oaI6t6T5xmowukxnifmFYwjBemvoSv5z7C7cOv5XeUb1pcDYwL2sesxbN4tzvzmVxzmKvxVNYl8PrO+/hf3uepMFZx/gu43l6kn+MvRItExYQxlPHP8XTxz9NVGAUO0t3cvGPF/PSupdocDR4PZ5FeV+wovAnFBT+edw/iQ6K9noMnUlSaBKvTXuNEEsIq/NW89+N/zU6JEPtKdtDla2KYEuw3zY4lURc+Ib1H2mPwy758+d6HK89tntFvHE1s0kirifYR6OqqqsjY3zQwfI+fY+4pQOsiB9i23dQXUDfwDj+cfJ/WHD+Ap447gmGJwzHoTqYnzWfm+bdxKlfncpnOz6j3lFvdMQes7d8LwA9AmO1D3SwFXHQxgreOPRGQGu2U1pXanBE7ZDTZH64P3T5j+qqPZZpFTd6Ii6l6f4lKTSJ64Zcx1dnfMUXp3/BXwb9hYiACHaX7+bm+Tfz+IrHPfp70u60MXf/h8zefB07KtZgVqxMT76cV6e9Sog1xGPXFcZQFIVTep7C12d+zUndTsKhOvjvxv9y4Q8XsqVoi9fiWFH4E99ma71kZo2cxcSUiV67dmfWO7o3D4x/AID/bPgPa/LXGByRcfRGbQNjB2Ix+ecgMEnEhfEKtsGB9WCywKBz//z5ruO1x5w/wN6ONzP6inhgGKlhWkLdktL0otoiauw1KJiaL023dbB9Oqvf0h5HXgVmK0GWIM7odQbvz3yfr874ikv7X0p4QDg5VTk8tuIxZnw5g3c2v0OtvdbQsN2tvL7c1UOgV+NWBuo62E2XRhf1vYjeUb0pqSvhqVVPGR1O22U3ScT9QWSa9lieTXl9OYW12taPXpGyIu6PFEWhb0xfbh95Oz+f+7OrJPzTHZ9yw9wbqLZVu/2aVbZyXt1xJz/lvoNdtdE3YiR3D3qDGSlX+u0bU9Ey+haJZyc/62ogeNnPl/Hjnh89fu11xQv5LPN5AE5MupC/DPyLx68pDjqt52mc0esMVFQeWvZQh14QOZp1BesA/y1LB0nEhS/Y8In2mD4dQuP+/PnY3hASB456rfS0rRoa3wQFhJESrjVdy6k6dmm6vhoeHZiAxWR1fbyjNGs7RP4WyFqm3RQZ8ec5oOnR6dwz5h7mnz+fe8bcQ1JoEkW1RTy35jlO++o0vtz5pWvGur/LKMsAtA7W4cGNXfs74Io4aFMNHpv4GCbFxE97f2J+1nyjQ2o9VYWc1dpzX++YrotqTMTLsl2dtxNDEgkL6JxTCjqSiIAI7hx9J69Ne40waxhr8tdww9wbDo6HdIPS+nz+ve0W9lZtJsgcymU97+WGPk8dUrklOr7p3afz9Zlfc2Laididdu5Zcg/vb3nfY9fbVr6K/+19ChWVCfGncVrqtSj+UIHUwdw95m7ig+PZV7GP1za8ZnQ4hvgj7w8ARiWOMjiStpNEXBhLVWHrN9rzIec3f4yiQNdx2vOs5W2/VsOfV8RbskdcnyGeEHjomxvX+LKOVJq++k3tsd9pENHliIcFW4K5tP+l/HT2Tzw64VFSwlIoqC3g4eUPc+5357IwayGqqnopaM/YVboLQNt3FKj9W3fEPeK6QXGDuHKgdvPlgaUPtGjbhk8pz4GqfFDM0MVPuqfqK+I1Rewu0hou+es+N9G8iSkTefPkN4kIiGBD4QbuXnK3WxosVdsreH3nvRTV7ycmMIlZ/V9kZOxUSYg6qZigGJ4/4XlXFcYzfzzD5zs/d/t1Mqu28m7GozhVByNiTuDcbrfK95xBIgIiuG/cfQC8s/mdTjdfPK86j5yqHEyKieEJw40Op80kERfGyt+iNSqyBEH6yUc+LrWxA3LexrZfS1/NDAh37REvqSs55gqF3rCr6egyAFtAFNCBVsTrKmDDp9rz0de26CVWs5Wz08/mu7O+485RdxIZGMme8j3cuvBWrppzlc/NOm0NPRFPj04/mIh3sPFlh7tl2C0MjR9Kpa2S2xfd7tbVO4/L1e6MkzQIAvxkX2xQJASEA7C7UOv8KvvDO56BcQN5ddqrBJgCWJS9iH+v/Xe7zmd32nkn42Hy67KItMbx177PkRjsB80JhUeZFBN3jr6TqwddDcBjyx9jUfYit52/sC6XN3beR4Ozjn6Ro7m4x12YFEkjjDS161RXn4B/rvyn3y+AtMbqPK0CbkDMAL+uIpOfIGGs7Y17mXqeAAGhRz4ucaD2mN+ORiRNVsTDA8KJaFzRPtY+cX102eHlfnbXingHSc42fAK2aojvB92Pa9VLA8wBXDHwCn465yeuHXwtgeZA1has5fKfL+dvC/7GnrI9Hgrac3aVNUnEg/QV8Y5Zmq6zmq08O/lZogOj2V6ynVsX3Oo/e89yGhPxVD8YW6ZTFFd5+u6ynYDsD++ohsYP5fHjHgfgnS3vMGfvnDaf67UNr7G7ciOBphBu6PMk0YEJ7gpTdACzRszivD7noaLyjyX/cG2vaw+bs4H3dj9KjaOSbqH9uKrXg4ds1RPGuXv03QRbgllXsI45mW3/veJv/shvLEtP8t+ydJBEXBht+w/aY//Tjn6cnogX7QJbXduu1WR8GdDiEWYHO6YfviKuN2vrAOXKqnqwLH30tW3uOB0REMHfRvyNH8/+kXPTz8WkmFiQvYCzvzub+5fe7+oK7eucqvPginhUOgRqq5YduTRdlxSaxCtTXyHEEsLKvJXcMv8WKhv84AaEvj88xc/+KDeWp2c03hCU0WUd18weM7lm0DUAPLjsQdfvmNZoOrLogu630SWkh1tjFP5PURT+MeYfDE8YTqWtklkLZ7W7uumbrFfJrdlNqCWSq3o/RKA52E3RivZKDE10VUE8t+Y56uxtfI/sZ/T94aOT/OjmezMkERfGKcvSSs0VE/SZcfRjw7tAcDSoDija0bbrNVkRBw7uEz9Kwzan6nTtlY0PPHxFvAM1a8tcqv3/ag2FIRe2+3SJoYk8POFhvj5DayDjVJ18u/tbzvr2LG6efzMrDqzw6RKq7MpsqmxVBJgCtFLhwM6xIq4bHD+Yl058iWBLMMsPLOeyny5jR0kbf+68wd4ABzZoz/1pRRwgKo1ik4lCezUKilaBITqsW4bfwrgu46i11zJr4SwqWtFjpLSulHsW34OKyti4GYyIPcGDkQp/ZjVb+dfkfxEfHE9GWQaPrXiszX9z1xYvYFnhDygoXNbzXqIC4t0crWivqwZeRVJoEnnVeby75V2jw/G4vOo8siqz/H5/OEgiLoy08xftsev45rulN6UokNDO8vQme8QBV+f0o5Wm51fnU++ox6JYiA5MPORzNqu+Il4Jbmi+Y6jVb2iPQy88WIbtBj2jevLvE//NR6d8xEndTkJBYXHOYq779TrO+vYsPt7+MVX6DRIfos9i7RfTD6vJenBFvIOOL2vOmC5jeHfGuyQEJ7CnfA8X/XARz65+lqLaIqND+7P8zWCvg6AoiPWzFeXINHYEBADQNaIrodajbNERfs9sMjN70mySQ5PJqsziviX34VSdx3ydqqo8+PuDFNQW0D2iO2d3vdkL0Qp/Fh8Sz7OTn8WsmPlhzw98teurVp9jT/kePs18DoBpXS6hX6SfVRx1EkGWIG4feTsAb29+m/zqfIMj8qxl+5cB2vzw8Mb39P5KEnFhnF1ztcf0k1p2fHv3iR9pRfwopel6o7bU8FTMivmQz9mb/PD7dXl6xQHY1rhFoIVN2lprcPxgnpvyHN+f/T0X9b2IEEsIe8r38M+V/2Tq51N5YsUTPrWPfEux9j02IHaA9gH95oSjvn2z7P3MgNgBfHr6p0zrOg27aue9re8x/YvpzFo4i693fc2Okh3YnDajw2yyP3xUm7dVGCYqjR2B2l7LvtF9DQ5GeEN0UDTPn/A8geZAFuUscpWaH837W99nUc4irCYrz0x+RkqDRYuMSBzBLcNvAeDJVU+2qrKp1l7L3xf9nQZnHb3DhzEj5QpPhSncYEb3GQxPGE6tvZYX171odDgetTR3KQDHpbSun5EvshgdgOikbHWwd7H2vHcLE/H4xjepRTvbds027BHX94d3i/hzR1rVZMVuCcVir8bSUIEtMLptcRlt7XtayX/XCQdvdnhIt4hu3DfuPv424m98v+d7Pt7+MXvL9/LJjk/4ZMcnjE0ay2UDLmNy6mRDR6JsLd4KaN2OgYOl6aBVVlgCDYjKGHHBcTx/wvMszlnM6xtfZ2PhRuZnzXfNGjcpJmKCYogNiiUyMJJgSzAhlhCCrcEHn1uCXf8FWYIINAcSaA4kyBJEgDmAIHMQwZZguoR10SoQWivXDxu16SK7sr1xRbxvjCTincWA2AE8MO4B7v/9fl5d/yoDYgcwKXVSs8euyV/D82ueB+Cu0XfRL6YfOXkde8VLuM9fBv2FNflrWJK7hDt+u4NPTvukRZU3T658koyyDMIt0Vze6x+YDluMEL5FURTuHHUnl/x0Cd/t/o5L+l/CwFjPvqczgt1pZ8X+FYA2HtLfSSIujJG1DOy12t7vliZ/sY3zdYvb2PDrCCviuVW5qKrabOKXUZYBHLmBki0gCou9GmtDGbX44fgYhw3WvKs9H32N1y4bFhDGxf0u5qK+F7EybyWfbP+EhdkLWZm3kpV5KxnXZRwPjHuArhFdvRaTzuF0HEzE9T9iJrO2f95WrTVsO9ZWig5oUuokjk85nu0l25m7by5rC9ayo2QHVbYqimqL3FKyHmAKYGDcQKZ3n86pPU4lKiiqZS/UG7Wl+mHZZFQaOwO0mw/9ImWGeGdyZu8z2VS0iU93fMo9S+7h01M/JS0i7ZBj9pTtYdbCWThUB6f0OIUL+7a/h4foXEyKiSeOe4Lzvz+fzIpMHln+CE8f//RRb3Z/tuMzvs74GpNi4vJe9xFhjfFixKKtBscP5tSep/Ljnh95ZvUzvDP9nQ43531j4UYqbZVEBkYyKHaQ0eG0myTiwhi75mmPvae2vJRU3/tZmqklkOZWrpwdtke8S2gXzIqZOkcd+TX5JIUm/ekleiLeO6o3NFORbAuMJrgmF2t9Seti8RU750DlAQiNh/5neP3yiqIwrss4xnUZx4GqA3y842M+3PohKw6s4Pzvz+fB8Q9yas9TvRrTrrJd1NhrCLWG0iOySUfioAgtEe9E+8QPpygK/WP70z+2P6A1MyyqLaK4tpjiumIqGyqpsdVQa6+l1l5Ljb3J88aP1znqqLfXU+849L9qWzW19lrWFaxjXcE6Xl73MtcOvpYrBlyB9Wg/69XFUNK4rSFlpBf+X3CvusAI9lobS9Mb+06IzuPu0XezvWQ7Gwo3cM2v1/DM5GcYGj8UgBUHVnDXb3dRVl/GoNhBPDT+oQ73plp4R3RQNM9Mfoa/zPkLP+/9mZEJI7mwX/M3ddbmr+XJVU8CWnPB7uZhXoxUtNesEbOYt28ea/LXsCBrAVO7TTU6JLfSy9IndJmA2eT/VRqSiAtjZDTuD29pWTpAeDJYgrWV9LKs1jdlOmxF3Gq20i2iG3vK95BRlvGnRFxVVVcinh6dTk5eM6dsLEcPqC9tXSy+4o+3tcfhl4ElwNBQuoR14faRt3N++vk8uOxB/sj/g3uW3MPO0p3MGjHLa29A1+SvAWBYwjAspia/IgPDtZsWnWCEWUuZFBMJIQkkhLR/jrE+oWBp7lK+3PUlu0p38cLaF1iQtYB/TflXszfKAMjV/r2ITdcmK/iZ3RV7cSgK0Q4HCbYGo8MRXmY1W3luynNc88s1ZFZkctlPlzEodhAO1cG2km0A9I/pz6vTXiXEGmJwtMKfDU8Yzq0jbuX5Nc/zz1X/JCIwgpk9Zh5yzJaiLfx1/l+xO+2c3O1krhl0DfO3FRgUsWiLpNAkrhx4Jf/d+F/+teZfTEqddPSb2X5mSe4SoGOUpYM0axNGKN2n7fNWzNBzSstfZzJBTE/teXFG66+rr2QGHmyypo8Kam6ea1FtEeX15ZgU06Ero03YArVyrQB/XBEv2QO7FwAKjLjS6Ghc0iLSePPkN7l+yPWA1gH0gd8f8FpTMD0RH5lw2OpqJxth5m0mxUS3iG5c2v9Svjj9C5447gnCA8LZWLSRi364iIzSI/zMu8rS/XB/OLCjVGue1KfBhlLVzN0+0eElhCTw4akfckavMzApJjYXb2ZbyTYsioUL+17IezPfIzrI/24yCd9z1cCrOCf9HJyqk7sW38Uzq5+hqLaIGlsNH277kKvmXEWlrZIRCSN4bOJjUoHhp64ZdA1xwXFkV2bz0faPjA7HbbIrs9lesh2zYj5iTw1/IyviwvsyGsvS08ZAcFTrXhvbCwq2tG2fuL6S2aTxVnpUOr/wS7OJ+K4y7WNdw7sSaG6+OVdDYyLul6Xpa97THntPhZjmbzQYxWwyc8vwW0gNS+WR5Y/w7e5vqXPU8fTxT3u0FElVVdbmrwVgZOLhiXjnG2FmFJNi4oxeZzA8YTizFs5iZ+lOrvn1Gt6Z/o42170pf94fDmwu2gxA//oGbYKB6JQiAiJ44rgn+Ouwv7KxaCMKCkPihxy5EkSINjApJh4c9yAhlhD+t+1/vL/1fd7f+v4hx0xMmcizk56VCgw/FmIN4Zbht/DQsod4fcPrnNHrjA5xM2/ePi1/GJU4qkN8PSAr4sIIeiLee1rrX+tq2NbKFXFbHTgayz6bzMnuHa2dT0+6m9KTc33VvDkNrhXx4tbFYzR7Paz7n/Z85F+MjeUozk4/m+enPI/FZOGXzF94bMVjqKrqsevtLttNcV0xgeZABsUd1gQkSFbEvS0tPI23p79Nv5h+lNSVcOO8GymubfKz5nRCrnbjxF8T8U1FmwAYXF+vbX0QnVqXsC5M7z6dk7ufLEm48AizyczdY+7m5RNfPjiiE0gJS+G+sffx6tRXCWucLiP815m9zqRvdF8qbZX8e+2/jQ7HLfREfFq3NuQPPkoSceFd9nrY85v2vKXzw5vSS9NLWjlz2pU8Ka5mbQB9ovoAWmdau9N+yEv0laqjzfb129L0bd9DTZHWtb7PDKOjOaoTup7A08c/jUkx8eWuL3n2j2c9lowvztVG6o1OGk2A+bA98/qKeH25R64tmhcZGMkbJ71B1/CuHKg+wO2LbsfmaNymULxL+/ewBEOC/41pqbXXum74DalvkERcCOE1k9Mm8+lpn7L84uUsuXAJc86dw0X9LsKkSGrQEZhNZu4Zcw8AX+76klUHVhkcUfvkVee5qoWmdu04Dejkp014V9YKrfN0aAIkDm7966MbR4SVZ7fudfVN9oebDn7bp4SnEGwJpsHZwJ7yQ5N7faVqaMLQI57Wb0vT/3hHexxxJZh9f4fKyd1P5uHxDwPw/tb3eXPTmx65zuIcLRFvdu9RYGNHa1kR97qooChemvoSYdYw1has5cV1L2qf0MvSU0b4xffx4bYWb8WhOoi3hpHocEhpuhDC68ICwlo+KlL4lVFJo7igzwUAPLz8YWrttQZH1Ha/Zv4KaI1040PiDY7GfSQRF97l6pY+7ZCEuMUiG2esludAa1ZF6xpXMZs0agNtv9SQuCEArMtf5/p4UW0RuVW5KChHnVN4cEXcj7qmF+6EfUtBMcGIK4yOpsXOTj+bu0bfBcCL617ki51fuPX85fXlrC9YDxwhEddL02WPuCF6RvbkieOeAODdLe+yfP9yyFqufdJPG7VtKmwsS4/ohQKyIi6EEMKtbht5G4khiWRXZvt1ifp3u78D4JQepxgciXtJIi68S58fnt7G/R0RKVoCaa+DqlaM1GimUZtuROIIANYUrHF9bGPhRgB6RfU66l4pv1wRX9O4Gt5nBkSmGBtLK10+4HKuG3wdAI+teMy1X8gd5u6bi0N1kB6dTkpYM/+/uErTZUXcKCd2PdF1d/++pfdRmrVM+0S3CQZG1Xb67xx9bjSVB1p3g1EIIYQ4irCAMB4a/xAAH2770LWy7E92lOxgR+kOrCbrn0bu+TtJxIX3lOdA4TYtke55QtvOYQnQ5omDNku8pfRVzKAjJ+LrCg6uiK8vXA80eYN8BA1BsVpY9hpM9rqWx2MUewNs/FR7PvIqQ0Npq1uG38K56ee6xq+4a9/T97u/B+D0nqc3f4BrfJmsiBvpjtF30DOyJ4W1hTxqrkBFgbSxRofVag6nwzUqb3TXKdoHbTXy/SU023+CH26Hlf/VeqsIIUQbHZ96PH8ZqDXmfXDZg81OCvJl3+7+FoApaVOI1LcJdhCSiAvv0bulp4yCkJi2nydKL09vRSJ+lBXxIXFDsCgW8qrzyK3KBWBp7lJA219zNA5LKE6TFfCTVfGMuVBTDGGJ0Ms/m10oisID4x5gWtdp2Jw2bl14q6uxXltlVWSxtmAtCsqRy55kfJlPCLYE89TxT2FRTMwLDeGH5PTWj0H0ATtLd1LZUEmIJYT+icMhqPHNhewTFwufhE8uhj/egp/vhA/OkWRcCNEut464lVGJo6i2VXP93OvJrmhlryWD2Bw2ftzzIwBn9DrD4GjcTxJx4T16It6WbulNRXXVHluzIq6XEzezIh5iDWFIvLZPfEHWArIqsthVuguTYuK45OOOfl5F8a8RZus/0h6HXOCXza10ZpOZpyY9xeik0VTbqrnml2tYeWBlm8/3zhatXH9iykQSQxObP0jGl/mM/rH9uTG4FwBPBtnJq84zOKLWW52nNZobkTgCi8miTTAA2Sfe2e1dDL89pT0ffIF283jfUljynLFxCSH8msVk4YUTXiA9Op2i2iKu+uUqthVvMzqsY5q7by4ldSXEB8czMWWi0eG4nSTiwjsctoNjy3q3cyXWlYi34m5e3ZFXxEHryg3wdcbXfL7zcwDGJ49vUSdRm78k4tVFsHOO9nzoJcbG4gaB5kBeOvElxiaNpcZew03zbmLO3jmtPk9edR7fZmhlT9cOvvYoF5TSdF9yTXE+g+vqqVTtPPj7gx6dL+8Jyw5o+9vHJI3RPiCJuFBVmPew9nzU1XDuG3BG44SAJf+CogzDQhNC+L/IwEj+e9J/6RnZk4KaAq6ccyVf7PwCp+o0OrQj+mi7toB0ft/zsTZWoHYkkogL78hepSUwIbHQZXj7zqV3Tm/ViniT8WXNOK3naYRaQ9lVuot3t7wLwEV9L2rZqYO0MQqBtYUtj8cIm74Apx2Sh0PiAKOjcYtQayivTHuFqV2nYnPauHPxnTy16inqWrFf/6lVT2Fz2hiZOJKRiSOPfKAk4r6jrhxL3hYeLyom0BTA8gPL+XTHp0ZH1WI1thpXb4PJqZO1D0oiLvb9DrlrwBIEU/6hfWzAWdqUEacNlr1oaHhCCP8XFxzHB6d8wMTkidTaa3lk+SNcNecqVhxY4XM3tLcUb2FD4QYsJgvn9znf6HA8QhJx4R16WXqvqW0bW9ZUW0rT9fFlzZSmg3aX8LYRt7n+95S0KQffIB9DfXACAIG1rejiboT1H2qPHWA1vKlAcyDPTn6WqwddDWhdQc/97lwW5yw+5h+Vz3d+zvys+VgUC/eOufcYF2rSNd3H/lh1OtmrAJWeYWncNup2AJ5b8xxZFa34nWCgZfuXYXPa6BrelR6RPbQPRjQm4rJHvPNa8R/tcdilENY4J1dR4Pg7tOcbPoEqH7/hK4TweREBEbwy9RXuHHUnwZZg1hWs47pfr+PCHy7ky51f+sy88Q+3au9bT+p2EnHBcQZH4xmSiAvvaDo/vL30RLw8u+UJkWtF/MjdFi/sdyEfnfIRL5/4Ms9PeR5FUVp26mBtT3FgnQ8n4nmbIW8jmKww+Dyjo3E7i8nCbSNv4+UTXyYhOIGsyixunn8zl/50Kd/v/p4aW80hxzucDt7f8j6Pr3gcgBuH3kjfmL5Hv4h+E0d1QkO1J74M0VL7Do4tu7jfxYxJGkOtvZb7lt6Hw+kwNrYWWJC1ANBu+Ll+z8iKeOdWWwo7f9Gej77m0M91HQfJI8BRD+v/5/3YhBAdjtlk5oqBV/DdWd9xSb9LCDQHsq1kGw8vf5ipn09l9urZ7KvYZ1h8uVW5/LT3JwCuGHCFYXF4mv92axL+ozIP8jZpz3ud2P7zRaYCijbqp6YYQltwl+wo48uaGhw/uNXhuBJxX14R36Tte6fP9PZ1rPdxk9Mm823it7y24TU+3fEpm4o2sWnpJiwmCwNiB5ASmoKKyrqCdeTX5ANwXp/zuH7I9cc+uTUEFDOoDm1VPPDI8+WFh+1ZpD12m4hJMfHYxMc457tzWF+4nne3vMs1g6856suNVG2rZl6WViF0UrcmjSslEe/ctn2vlZ8nDITEgYd+TlFg5JWwfy1s/ByOu635cwghRCslhSZx79h7uWnoTXyT8Q2f7viUnKocPtj6AR9s/YAJyRO4pN8lTEqd1OIFKnd4Z/M7OFQH47uMZ1DcIK9d19tkRVx43m5t9Yfk4QfL7drDEgjhSdrzshberdM7XR+hWVt76KXpAbX5bj+3W6gqbPlKe94BV8MPFxYQxh2j7+Dnc3/m/4b9H13Du2J32tlYuJGfM39mTuYc8mvyiQyM5IFxD/DguAdb9sdFUZqUp8s+ccPUlMD+ddrzXicAkByWzN2j7wbg5fUvs6Nkh1HRHdMvmb9Qa6+le0R3hsYPPfiJsMZu/VJ63Dlt+Vp7PNLv6AFngjkACrYcvLEthBBuEhUUxVWDruLHc37k1amvaok3Csv2L+OvC/7KDXNv8Nr2r8KaQr7epf1OvG7IdV65plFkRVx43i43lqXrorpqK0dl2ZBylAZbumM0a2uP+qDGPeK+Wpqeu0bbT28NhfTpRkfjNXHBcdw09CZuHHIjOZU5bCzaSGldKQ7VQY/IHoztMpZAc2DrThoYAXVlMsLMSHt/A1SI7w8Rya4Pn9X7LBZkL2BR9iLuW3ofH5/6MVazb3VYVVWVT7Z/AsDZ6WcfegMoTPs9QlW+dvPMiysPwmC2uoPbLfqd2vwxwdFaRdO272Hjp5B6i/fiE0J0GibFxPGpx3N86vHkVObw6Y5P+WjbRyw/sJzzvz+fh8Y/xCk9T/FoDK9vfJ0GZwPD4ocxKnGUR69lNFkRF57ldBxcEXdnIh6Zqj2W57Ts+BaWpreFq1lbXRGK0+7287fb5sbV8L4zISDE2FgMoCgKaRFpnNrzVC4bcBlXDrySSamTWp+Eg6yI+4LdC7XHxtVwnaIoPDT+IaIDo9lRuoNXN7xqQHBH91vOb2wr2UawJZizep916Cf1RNxRf7C5pOgcclaDvQ7CkiCuz5GPG3Kh9rjpC+1vqxBCeFBqeCp/H/V3vj7za0YljqLGXsPdS+7m8RWPY/fQ+92siiy+3PklALeOuNWr5fBGkERceFbuGm0FMSgSUtx4V6vViXjjG1sPlKY3BMaiKiYU1YnV12aJO50HSx4HnWtsLB2BfiOnThJxQ6hqk0T8z/0m4oLjeGD8AwC8tektfsv+zZvRHVW9o55/r/03AJf0u4SYoMN6NViDDzaTrPLR6hrhGXsXa489Jh29EiL9ZO17pPIAUUVrvBObEKLT6xrRlTdPfpMbhtyAgsKnOz7l1gW3/qkRrju8uO5F7Kqd41KOY3TSaLef39dIIi48Sx9b1vMEMLtxJ4Q+S7w8+9jH2upAH8XgiUZlJjP1QVrDOJ9r2Ja9Air3a2/eek81Ohr/13SEmfC+4t1QnqXtle02odlDTup2Ehf0uQAVlbsW38Wu0l1eDvLPVFXluT+eI6Msg5igGK4aeFXzBzYtTxedR9NE/GgsgdD/NAASs3/ycFBCCHGQ2WTmr8P/yr9P+DdB5iCW5C7h6l+upqSuxG3XWHlgJb9k/oKCwt9G/M1t5/VlkogLz/LE/nBo3Yp4XZn2qJggwP17xKHJPnFfS8Q3a+U99D9NexMn2kcScWNt/0F77DYRAkKPeNg9Y+9hdNJoauw13LLgFgprjGuAZnfa+C77dT7a/hEAj054lKigqOYPdjVsk0S806ivgtw/tOfHSsQBBp0DQGLOHN/cCiWE6NBO6HoCb05/k+jAaLYUb+HKn68krzqv3ee1OWw8sfIJAC7oewH9Yvq1+5z+QBJx4TmVedq4FYD0k45+bGu1JhGvLdUeg6LA5Jlv+foQbfRQcE2uR87fJg47bPlGe9745k20kyTixtr2vfbY//SjHmY1WXlu8nOkhqWSW5XL9XOvp0y/IeclVbZyFuV9wezN17Io/wsA7hx1J5PTJh/5Ra4VcR+7oSc8J2s5OO0Q1Q2iux37+B6TITiGgPoSogtWej4+IYQ4zND4obw38z2SQpPIrMjk8p8vZ2/53nad881Nb7K3fC8xQTHcMrzzNKOURFx4zs452mPKyIPjxtxFT8RrisBWe/Rja8u0x+Bo98bQ9BKhWql8cFUL96x7Q+YS7f+f4BjtzZtoP73HgDRr877y3MaVQ+XInaWbiAqK4r8n/Zf44HgyyjK4cd6NVDVUeTzM3JoM3t/9BA9vuJBvs1+jsD6XUEskz0x+hisGXnH0F8uKeOezt7GPQUtWwwHMVhhwBgCJ2T96KCghhDi6HpE9+GDmB/SI7EFedR5X/nwlW4q3tOlcGws38vrG1wG4a/RdROr9UjoBScSF5+z4WXvsO9P95w6KgoAw7Xn5MVah9RXx4Cj3x6FfIqwxEa9uwZ51b9Fnhw84Q3vzJtpPEnHjbG9MOtLGtvjGXlpEGm+c/IarhO6meTdR0eCZf7uyujLu/O1Ont1yI+tKFuJQ7aSF9OH8brO4f8j7zOg+49gn0VfEq2WWeKeh7w/vOaXlrxmoVTgl5M5FcTS4PyYhhGiBpNAk3p3xLgNjB1JaX8o1v/w/e+cd32Z1/f+3JNvy3jOJk9jZewMhgTDChoa9Ryij/IBSoLTf0gEUyiiUFiizQFkNEDZhQwIJGRCSkL3jxImT2I73npJ+f1w9kp14SNZ4NM779fLrXmvce2zL0nPuOedzrmNVySq31qhpqeEPS/+AxWbhjMFncGaeb1ujBRriiAu+obUBdi9W8xE++KcyGDqkp/fi/Doccd9FxBvjB6ot6vf5bA+3sLTBVns97RhJS/cakpquH1s+VmMvaemHMyR5CM+f8jwJUQmsK1vH9V9d71VxGVCn+RcsuIAvC7/EgJHJqSfx29HPceeYZzk282yiTd3Xs3dCxNrCi8ZKKN6g5oOPc/15g2fSEp1OZGsNqYdW+MY2QRAEF0iNTuXl017mqOyjaGhr4KZvbuK7fd+59NxWSyu3f3c7RXVF5MTl8Kdj/hTy7coORxxxwTfsXqz6oiYPhMzRvtnD1TpxPzjijtT0hiLVYklv9nwPTZUQm66ErQTvIO3L9KFqL+xdBhgcabnuMDptNP897b+kRqeytXIrc7+cS2mDd5zddYfWceM3N3Ko6RCDEwdzx+inuWrIHxkQN8z9xSQ1PbzYuxywQcZISMhy/XlGE4cGnAZA1j5RTxcEQV/iIuN4dvaznJR7Eq3WVu5YfAfzts7D1sP1cIulhd8t+R2rS1cTFxnH0yc/HVYp6RriiAu+Ybv94mDEWT33RfUEVx1xTaTJh454c2w/bAYjJkszUc3lPtvHZbZ8pMZR53i3bVy4IxFxfVj/lhrzjleHe31gZOpIXj39VbJis9hTs4erv7ia3dW7PTJr3aF13LTwJhraGjgq+yjmnz2f3LjhfV9QxNrCi91u1od3oCRX6SRkHlyI0dLiTasEQRDcxmwy8/gJj3Pu0HOx2Cw88tMj3LTwJnZU7TjisYU1hfzyy1/ybdG3DnHV4SkefHYGMXKFLngfqwW224XafFEfruFuRLy7lkFewGaKojm2HzEN+4lp2EdrTIbP9uqVTmnp5+pnRygS6o54ewv8/Lo6SGushLShMO26bnt2+wVLO6ydp+aTrvRoqbykPF4/43Vu+PoG9tXt48ovruTJE59kWvY0t9c63An/90n/JjYyFvDgtaFFxBvK1Puo0dT3tYTAx9X+4V1Qkz6Z5pgsoptKSStZSll/L7cIFQRBcJMIYwT3H3s/o1JH8c81/2TFwRWsWLCC6TnTmZw1mQhjBJvKN7G4aDEWm4WEyAT+deK/ODrnaL1N1w2JiAve58AapdZtTvLtBXySSgcPhBpxgKY4dTAQq3edeOFSe1p6Ggyaqa8toUYoi7UVb4Bnp8Pnd0HBt1C8Dja9B6+cAV/9STnEerDtU6jZp9T/3awP74p+8f1448w3GJ8xnrrWOm785kY+3f2pW2t074R7SGw6YACbFRorPF9PCFzqSqB8O2DoW/mQwUhprjroztrn3utXEATBVxgMBi4fdTnvnvMupw1WJTQ/FP/AM+ue4cmfn2TRvkVYbBaO638c7//i/bB2wkEi4oIv2Ga/KBg227dq3QFUIw7QkJBP6qEfiavZ5dN9emXzh2oc9QtJS/c2Dkc8xCLiBd/BW5dBexPEZ8Oxt6po+LbPYO0b8MPT0FoPZz/hu1KTrrDZ1N4A066HyBivLJsancrLp77MH5f9kW/2fsPdS+9mb+1ebhp/E6ZeotCrSlbx629/7X0nHNT/a1y6iojXlzpT1YXQY89SNeZMgNjUPi1RMvAXDNrxKpkHviGquZzW6HQvGigIgtB38pLy+Mesf/DrSb9mcdFiCqoLsNgsDEgYwIm5JzIydaTeJgYEcpUueBebDTZ/pOaj3BdVcouOjrjN1r2D4OgjnuxTc+pSlChdQnXf+ih6BUlL9y0dU9OtVjCGQFJRwbd2J7wZ8k+EC//rdAxGnKHaKr1/Pax5FdKHw/Rb/Gfbzm9g/yowmZUj7kWiI6L5x6x/8K81/+LVza/y/PrnWVO6hodnPkxWXNfCWV8Xfs3dS++m1drqfSdcIz7L6YgzzrtrC4GDu/3Du6AudSw1qRNIqlxP/93vsGf0zV4yThAEwTsMShzENWOu0duMgCUEriKFgOLgWqjeC5GxMOxU3+6V0A8wgKUFGnoQSPNTRLwuZYwyq2qLfsrpkpbuWzTVdGwqQhxgJFRtpn/B26QcWqlqjHtj1yKnEz78DLh8/pHRuXEXwumPqPk398LBdV63u0ss7bDor2p+9K/cU5V2EaPByG+n/pYHZz5ITEQMq0pWce7H5/KfDf+hpqXG8bjShlLuW3Efv13yW1qtrZw88GSeOfkZ7zvhIIJt4YLDEZ/l0TJFw5RuwoBd/8PY3uSpVYIgCIIfkYi44F20tOjhp0GUDy5SOxIRBQnZUFes6sTjuxFI85MjXp84DKsxkqjWaqIbD9Bsrxn3K45sBFFL9wkR0WCMAGu7ioo7HHOdsdkYvu5BBu583XnbhiFw9j9VRLsrtn4C7/0SLK0w4ky46FWIMHf92KN/pQ55tn0Kn/wGbvjW90JiK5+D0k1Ka2LmHT7d6hdDfsH49PH8Yekf2FyxmX+v/TfPrX+OvKQ8rFYru2t2Y0Mdrl0z+hrumHJHrynsfUZamIU+VYVQvU+9lww8xqOlSgecwZBNTxLTsJ8Bu95k38jrvGOjIAiC4HMkIi54D5vN2TZrzHn+2bO3OnGrBZrtkS0fqqaDUk6vT1LtFxKquk5PN7XVM2TD40xbeAETv7+e1JJl3jPA0qacK4DR53pvXcGJwRCQyukDds1j4M7XsWGgMvMY2qKSoLIAXp8D79/QObpqtcKKp+Gdq5UTPuocuOi17p1wUD/32f9STnHxOlj1sm9/oNIt8O2Dan7qA32uoXWHwUmDefOsN3nkuEcYljKMdms7O6t2UlBTgA0bU7Km8Orpr3LXtLt854SDRMTDAU0tvf9UMMd7tJTNFMXu0apcZPC2F4hsFpE/QRCEYEFCZoL3OPizOuWPjIWhp/hnz6QBqoa0O0e8sRLskSx/XMzXJY8msWozSRXrKRtwWqf7zI0lTFx6Awk12x23pZd8z5YpD3BwyCWeb77ne2da+uDjPF9P6BpzosqyCBDl9IjWWoZs+hcAOyf8gX0jrsXUWseJB1+An16Eje+odmQjz1ZCYLsWQtk29eSJV8I5T7qWPRGfCbPvgc9+C98+AKPn+CRdnIZymH+FEo4bchJMvtr7e3SD0WDkrPyzOCv/LIrqiiisKcRoMDI0eWi3deNeRyLioY8Hbcu6omTQHAbufJ2E6q2MWPs3Nh3zT/+KKgqCIAh9QiLigvfQ0qKHn+77tHSN3iLiDWVqjEn1rYK7ncpMlWaYVto50m1qa2DishtJqNlOS3QGm45+jAN5FwIwas09pJYs93zzDe+ocfQcSUv3JQHWwqz/7neIbKujPnEY+4YrQRRLVAKc+ZhKIc+ZqOrZN7ytFMjLtqmf4ex/wZyn3XutTLkW+k1WP/ui+73/wzSUw2vnQOVuSBoI57+km0ORm5DLcQOOY0b/Gf5zwqGDIy4R8ZDEZnM64vme1Yc7ljRGsGXq37AZjGQXfUburje8sq4gCILgW8QRF7yD1QIb31Nzf6WlQ++9xBvsF7N+agNUmTUDGwYSqrcRo/UTt1kZveoPJFRvo8WcxqqT51MyaA5bpz7IgbwLMWBj1Oo/YWrzQPyrpd6Zlj7hMs9/EKF7Aiw1PafwfQD2DbsaDIe9pfefDDcuhrmfwaz/g6P/H5zzFNyxCab+0n0n12hSDj7Auv/B/tWe/wAah7bCy6fCoS2qhdpVH0JcmvfWDxYkNT20Kdumsh0iomHANK8tW5c6jp3jfgfA8HUPkVqy1GtrC4IgeJ22ZvUV5ogjLniHwqVQd1DVYQ8/rdeHe43eIuL19oh4XDdCbl6mLTqVyqwZAAzY9SbYbAzZ+C+y9n+F1RjJhhnPOEXcDAZ2TPwTTXEDiGk8yOBt/+n7xts+hbYGSM336sWd0AUB5IjH1BUSX1uA1RhJ6cCzun6QwQCDZ8KJf4QzHoEp10B0Ut83HTAVJl6h5p//TtWce8qm9+HFk1Rde+IAmPsppA/1fN1gRFLTQ5tdi9Q4aEbPugx9YN+IX3Jw0LkYbFbGr7jNfx0OBEEQXKVyD7x9BTyUAw/1U/PuruHDAHHEBe+wfr4ax5zn9YuLHuk1Nd0eVfKTIw5QNOwqAHJ3vcH4FbeQt+0FALZOuZ+a9MmdHmuJjGPHxLvV43e+TlRzD23YemL922ocf6nUBvoaTSm9Wf/U9PRi1QKpOn0KlkjPRJ/c4uR7ISpB6UKsm9f3dSzt8NWflHp7W6Nq5fSrJZA+zHu2Bhvae1VzNbS36GqK4AMKvlXjkJO8v7bBwNapf6My8xgi2htg3kVQe9D7+wiCIPSF4vXwnxNU8MhmBZtFzV86BWoO6G2dLogjLnhOayNsXaDmEy71795aanrDoa5TXOr9m5oOUJ5zAof6z8ZobSPzwEIAdkz4A8V5F3T5+LJ+s6lJHUdEeyODt77g/oa1B509acdf3FezBVcJoIh4WomqNS3P9k6tqcskZMEJf1DzhfdBU7X7azRVwZsXqbp1gJl32tPR071lZXASkwJGu56FpKeHFm1NsNeuBzL0ZJ9sYTNFsf7YZ6hLGqE+Fz+4UZWOCYIg6EldCbxxvjpk7j8F/t8P6it9uMqoffsy1f0nzBBHXPCcbZ8pMaiUwZB7tH/3jklRKu0AtV2cpjXYI8x+jIhjMLDpmH+xc/zv2Z9/CT8f/wr7Rvyyx8cXjL0TgAEFb2JuLHFvvw3z1cniwOmQmueB4YJLBIgjbrC0knJoJQAVOd5RX3aLo25UH6CN5bDkUfeeW74TXpqtooORsXDx6zD7Xt/3Jg8GDAYRbAtV9q6A9mZI6AcZI322jSUqgY3HPgWRcapsbO3/fLaXIAhCr9hs8NH/U9cLWWPhqo8ga7T6uuI9JahcvB5WPq+3pX5HHHHBczbomBZtMPScnu5nsTYNq8nM3pHXs23qA1Rmz+j18ZVZx1KVPhWjtY1B219yYyMLrPqvmk+6so/WCm7hUE2v0dWMhOqtmKyttEYl05CoQz11RBSc/oiar3xe9f52hV2L4MWToWKXymj55VdK6V9w4hBskzrxkKJjWrqPPysbE/KULgTAkr+raLwgCIIebPlIvf9FxMCF/3WW+AGkDIJT7F1YFj8CDRW6mKgX4ogLnlFX4ry40CstuidHvN7/NeJ9wmBgz5hbAOi/ez5RTS5GwrZ/ATX71Gni2K5T3wUv43DE9Y2IJ1ZuBKA2dZx+ugBDT1b9yW0WVefd2tj9Y202+OFZmHehOsTIPQZu+A5yxvvP3mBBBNtCkx1fqXGoD+rDu2La9Ur8sPaAZ1oOgiAIfaW9Bb65V81n/AYyRhz5mIlXQM4ElV0bZlFxccQFz9j4nkqLHnAUpA3RxwaHI95FCzOtj3icfyPifaEy81iq0yZjsrS4HhX/yV5TPuUaiIzxnXGCkwBJTU+s2gRAbarOjuzZ/1L/X2Vb4YMblADb4bQ2wIe/gq/uVu8XE6+EaxZAfIAfkOmFRMRDj7LtULETTFEw9BT/7BkZDdPVAS8/v+6fPQVBEDry04tQvVe1JZ1xW9ePMRqVTgyo69oWD9r5BhniiAt9x2ZznrJP1LF3dfIgNVbu6Xy7zeZ0xIPhgt9gYLc9Kj6g4O3eFdQProM936ve0VOv8719giJAVNM7RcT1JD4TLnoVTGalfvrWpVBndyBtNpWK/p8TlJaBwQSnPQRznvZvd4VgQyLioYcmaJp/Que0TF8z/hIl/le8Hoo3+G9fQRCEtmZY/qSan/QniIrr/rGjzoGUPGiugc0f+se+AEAccaHvFK+HQ1vUBfiY8/WzI81eH1tZ0Pn25mqwtKp5oKem26nMmklN6nhMlmYGbeslKr7k72ocewEk5/reOEERABFxY3sjcXXq9V6borMjDjB4hnLGI6Jh1zfwxDglxvbEePjf+VC+QzmX13yiInTSYq9nEkSsLeTY/LEaR53j333j0mDkWWq+6T3/7i0IQniz4W2l1ZQ4ACb0ErAzmlR2J4RVBo844kLfWf+WGkeeBTHJ+tmhpcRX7Op8e22xGmNSgidt22Bg95hbAdWHPKZub9eP2/cjbP9cRcNn/Z8fDRQCwRGPr92FwWalJTqd1pgAOWQaeSZcvxAGTANLC+xfpfQLIuPgqF/BLSuVwy70jkTEQ4uSjVC6UUWmR57t//21PXcu9P/egiCEJ1YLrPi3mk+/GUyRvT9nwuVgjID9P6lynjAgQm8DhCClvRU2vKPmE6/Q15bUfDU2VUFjJcSmqu+1mnGthjxIqMieRXn2caSXLGXkz3+FaZ+o+hkNSxt8eoeaT7oS0ofpY2i44hBr0y81Pa5WRcN1UUvviexxcN03cGirioLHJEO/yf5NxQ0F4rPVWCeOeEiwzn5oPeIM5+eTPxl6MmCAQ5uh5gAk9fe/DYIghBc7vlIBsuhkmHyNa89JyIKhs2HHlyo9/YQ/+NTEQEAi4kLf2PkVNFWqC8YhJ+prS1Sc6ssKUNEhPd3hiAdZ2rbBwI6Jf8JiMpNWugyWP9H5/i/+T5UExKbB7L/qYmJYoznirfXqxFcHYjVHPCFfl/17xGBQvUHHnOv/ethQoaNYm82mry2CZ7Q1OVt86nVoHZsKA6aq+a5v9LFBEITwYrW9te7kq8Ac7/rzRp+rxi0fe92kQEQccaFvrHtTjRMuUXUdeqOlp3esE9famQWbIw40JuazY+Kf1DeL/goL74ND2+CT38DqlwEDzHlGn+hKuKOlpoNyxnVAi4g3JgagIy54jpaabmlRWhdC8LLuTWisgOSBKtKjF0NOVmPhcv1sEAQhPKjaC7vspTBTrnXvuSNOV2U8h7ZA2Q7v2xZgiCMuuE99Gez8Ws0nXK6vLRqaYFvHOvHqfWoMstR0jQP5l7Bn5K/UN8v+Bc8eDWteBQxw+iMqzVHwPxFm9SEBuimnx9XtBqAhUaeWgYJviYyG6CQ1F8G24MXSBj88rebH3AImHasBc49S4/6f9LNBEITw4OfXARvkzXK/tXFMisqmA9ga+lFxccQF99n4LljbVe1n5ki9rVFoddIdxR00p1yv/uaeYjBQMP63cOF/IXu8UqTuPwWu+gCOuUlv68IXg8GZbq2DYJvB0kpMvTpkakgI0te20Dsi2Bb8rHoJKndDbLrS89CTAVMBA1QVqsN0QRAEX2Bpg7VvqPlUN6PhGqPnqHHLAu/YFMCIWJvgPlpa+sQAiYYDZI5WY+lmNdpsznrxtAATtHKXsReoLyFwMCeodFMdHPHY+n0YbRbaI+Joicny+/6Cn4jPUoJ3ItgWnNTsh8UPq/lJf3avRtIXRCdBxggo26Y6Gow8U197BEEITXZ8qQ6Q4zJhxFl9W2PEGYABSjZAXQkkZHvVxEBCIuKCe5RuVm1YTFGB5RxmjVVj5W5obVBvAq31qr1XymBdTRNCEB1bmMU0KBHCxvhB0o87lJGIePDS1gzv/RKaa1Tm2OSr9bZIMWCaGiU9XRAEX+HoqHQZRET1bY24dOg3Sc13hXbbRXHEBffY9L4ah50aWEJh8Rn2lj82OLgOSjep21PyVE2vIHgTs71+t6XG71vH1CtHvCk++EQIBTcQRzw4aa6Bty+HopWqw8KF/w0MQVNQpU0AxRv0tUMQhNCkpc6pITX2Qs/W0sQtxREXBDs2m9MRH3u+vrZ0hSZGU/SjcsYB+k3UyxohlNE1Iq66ATTFBacIoeAiCeKIBx2Fy+C5GVCwCCJj4bK3IDVPb6ucaJljWgmXIAiCN9n+BbQ3q5LQ7HGerTXsFDUWfAuWds9tC1DEERdc5+BaJfQSGQvDT9fbmiMZOF2Ne76HA2vUPGeibuYIIUwApKY3xUlEPKSRiHjw0N4CX/8FXj0baopUOdQ1n8DgmXpb1pnMUWqsL4GGcn1tEQQh9Nj0gRrHnO956Vz/KRCdrLKMtGv6EEQcccF1tGj48NMhKk5fW7pi2Klq3L0Ytn+u5nnH62aOEMJoquk6tC+LtkfEmyUiHtrEZ6pRxNoCm5oD8PIpsOIpwKbqwW9aZlcpDzDM8apcCyQqLgiCd2mqcqaReyNr1miCISepecEiz9cLUMQRF1zDaoXNH6p5IIm0dSR9qGrzpZEyGHIm6GaOEMLoFRG32TpExMURD2ni7SqxEhEPXEo2wYsnQfF6iE2DS9+EX/zb+f4QiGSNUaM44oIgeJNtn4G1TXUx0rJvPCV/lhoLl3lnvQBEHHHBNfavgtoDSnxGE1AIRE75K2BPhznlflGVFnyDTo54ZEsVEe2N2DDQHNffr3sLfkZLTW+qhPZWfW0RjqR6H/zvfJXmnTEKbvgORvaxVY8/kTpxQRB8Qce0dG8x+Dg17l8FbU3eWzeAkD7igmts+0SNw0+HyGh9bemJISfBbWtVzV7mSL2tEUIVsz013c+q6Vo0vCUmE6tJugGENDEpYIwAazs0HIIkyYAIGCxtMP8qla2QOQau/RxikvW2yjW0z8Xy7fraIQhC6NBQrspCwbtizqn5kNAP6g5C0U/OCHkIIRFxoXdsNthmr7keeaa+trhCap444YJvcTji/o2IRzceBKA5VqLhIY/RKIJtgcqSR6F4nRISuuKd4HHCQakZA1Ts0tcOQRBCh60LwGZR5aBpQ7y3rsHgFL0sXOq9dQMIccSF3infCZUFYIoK7LR0QfAXOqWmRzeWANAcm+3XfQWdEMG2wKOiAJY/oebnPBF8mQqp9ovkpiporNTXFkEQQgNfpKVr5NnT0/eIIy6EK9s/U+Pg4wJbhEYQ/IVOqunmpmIAWmLEEQ8LRLAt8PjmHrC0qkPp0efqbY37RMVCov3woHynvrYIghD81JU4xdTGnOf99bWI+IE10Nro/fV1RhxxoXeCKS1dEPyBbhFx5ZBJRDxM0CLi9Yf0tUNQlGyCbZ8CBjj1weAVA02X9HRBELzElo8BGwyYBimDvL9+Sh4k5ChF9oM/e399nRFHXOiZ+kNKrRBghDjiggDo5oibm1Rqektsjl/3FXTCUSNeoq8dgmLZv9Q45tzg1iFx1IlLRFwQBA/xZVo6qAPP3KPUvOgn3+yhI+KICz2z40vABv0mQWI/va0RhMBAE2trawCrxW/bRjeq1PRmSU0PDxI0R1wi4rpTuRs22y84Z96hry2ekjZMjRIRFwTBE2r2Q9GPgEEdUPqK3KPVKI64EHbsWqjG4afra4cgBBIdtRJa/FMnbrC2E9VcBkhqetigRcTrJCKuOz+9CDarqg3PmaC3NZ6Rmq/Gyj362iEIQnCz+UM1Dpzu22CdwxFfqTo5hRDiiAvdY2l39gUccrKupghCQBFhBq2Pt5/S06OayzHaLFgNJlrN6X7ZU9CZeImIBwRtzbD+LTU/+iZ9bfEGWh1n9b6Qu6gVBMGPaGnp3uwd3hXZ49U1V1Ol6lwRQogjLnTPwZ+huUb1Su0/WW9rBCGw8HOduFYf3hqTCUaTX/YUdKZjH3FxmPRj6yeq3VdSLgw5SW9rPCd5oBpbatXPJQiC4C6Ve5SfYDDC6Dm+3SsiSpXIAuwPrfR0ccSF7tm1SI35J8iFvyAcjp9bmDl6iEt9ePigOeKWFmiu1tWUsGbNq2qcdFVofBZGxkCcXZG/eq++tgiCEJxomhmDj3N2+PAlDsG2lb7fy4+IIy50T4HdER8qaemCcAT+jog3q/Tklhg/fOAJgUFkNEQnqXmd9BLXhco9sHeZivpMulJva7xHx/R0QRAEd9lkrw8fe4F/9gtRwTafOOIHDhzgyiuvJC0tjZiYGMaNG8fq1asd99tsNu655x5ycnKIiYlh9uzZ7NwpbTQCiqYqOLBGzUMhFU8QvI2mnO4nsbao5nIAWqOlPjysSLAL4NQd1NeOcGXT+2rMOx6S+utrizdJtjviVRIRFwTBTcp3QulGMEbAqHP8s6cWET+0VZXNhghed8SrqqqYMWMGkZGRfPHFF2zZsoXHH3+clJQUx2MeffRRnnrqKZ5//nlWrlxJXFwcp512Gs3Nzd42R+gruxcrhdj0EZA0QG9rBCHw8LMjbm5Siukt0RIRDys0JdpaccR1QXPEx16orx3eRqsTl4i4IAjuoom05Z8Isan+2TM+E1IGAzZnoDAEiPD2gn//+9/Jzc3llVdecdyWl5fnmNtsNp544gn+/Oc/M2eOKu5//fXXycrK4qOPPuLSSy/1tklCXyj4To2Sli4IXePn1HStdZlExMMMccT1o3QLHNoCpij/RX38hSM1XSLigiC4gc3W4YDSx2rph9NvElQVQvH6kMnW9XpEfMGCBUydOpWLLrqIzMxMJk2axIsvvui4f8+ePZSUlDB79mzHbUlJSRx99NH88MMPXa7Z0tJCbW1tpy/BxxQuU2PeLH3tEIRAxe814vaIeEyGX/YTAoREezp07QF97QhHNr2nxqGnQEyyrqZ4HYmIC4LQFw5tgfLt6oBy5Fn+3TtnghoPrvPvvj7E64747t27ee655xg2bBhfffUV/+///T9uu+02XnvtNQBKSpTyb1ZWVqfnZWVlOe47nIcffpikpCTHV25urrfNFjpSexAqC5Q4zcBj9LZGEAITP6umO2vExREPKyQirg96Rn38QbL0EhcEoQ9oaelDT3GKifqLnIlqLF7v3319iNcdcavVyuTJk3nooYeYNGkSN954IzfccAPPP/98n9e8++67qampcXwVFRV50WLhCAqXqzF7fOhFAQTBW/gzIm61ENVSobYTRzy8cDjixfraEW4cWKNSICNjYcQZelvjfZIGAAZoa4SGMr2tEQQhGND7gFKLiFftgaZq/+/vA7zuiOfk5DB69OhOt40aNYp9+1T6U3a26oFbWtq5FUtpaanjvsMxm80kJiZ2+hJ8SOFSNQ6eqa8dghDIOBxx30fEo1oqMdis2DDQZvaTMIoQGDgccUlN9ysb7WnpI86EqDh9bfEFEWbna0vS0wVBcIXidcoJjoiB4af7f//YVGc2T4hExb3uiM+YMYPt27d3um3Hjh0MGqR+cXl5eWRnZ7No0SLH/bW1taxcuZLp06d72xyhL2j14YOP09cOQQhkzPaULD844maHUFsaNqPXNTaFQEZzlpoqoa1JX1vCBasFNtvTL8eFmFp6R7Q68apCXc0QBCFI0NLSh58G5nh9bNCi4uKId80dd9zBjz/+yEMPPcSuXbt48803+c9//sMtt9wCgMFg4Pbbb+dvf/sbCxYsYOPGjVx99dX069ePc88919vmCO4i9eGC4Bp+TE0XxfQwJjpZpUeD1In7i73Lob5U/e6HhHDnkCS73o5kWwiC0Bs2G2z+UM311M3oN1GNxev0s8GLeD20Mm3aND788EPuvvtu7r//fvLy8njiiSe44oorHI/5/e9/T0NDAzfeeCPV1dXMnDmTL7/8kujoaG+bI7iL1IcLgmv40RF39hCX+vCww2BQUfGKXcoRTxuit0Whj1YDOeociIjS1xZfIkKAgiC4yv5VUFMEUfEw7FT97NAE20JEOd0nOY5nn302Z599drf3GwwG7r//fu6//35fbC94gtSHC4Jr6BIRF0c8LEnIUY54nQi2+RxLG2xZoOahnJYO0hpPEATX0dLSR5wJkTH62aE54pUFqmtNdHDrhnk9NV0IcqQ+XBBcw4/tyxw9xMURD0/EYfIfu5eoevy4DBgU4gfSSfbXVY28rgRB6AFLO2yyC1iOvUBfW+LSnGU1JRv0tcULiCMuOJH6cEFwHbPdEW9vUlE0HyI9xMMcSSH2H1pa+uhzwRTiwojyuhLqSuHjW+Hpo+DNS+HgWr0tEgKRgm9Vm8PYdBgaALoZDsE2ccSFUELqwwXBdbTUdPB5erqWmt4SI2JtYYk4TP6hvQW2farmekd9/IGWaVFf6vPDRCEAqdwNL58Ca9+A8u2w4wt4+TQo+klvy4RAY/1bahx3EZgi9bUFIGuMGg9t1tcOLyCOuOBE6sMFwXVMkaqXJvi8hZlZasTDm6QBaqwp0teOUGfXQvW/nNAPco/W2xrfE5sOpijAJvoD4UZbM7x9JVTvhZQ8uGSe6hBgaYH5V0F9md4WCoFCUzVs+0zNJ1yqqykOMkersXSLvnZ4AXHEBSdSHy4I7uEnwTYtNV1qxMMUrd9z9T597Qh1tLT0seeDMQwuj4xGJQQIkm0Rbnz3oIomxqbDtV/AqLPh4tchYyTUl8CSv+ttoRAobPlYHdBkjHKmhOuNFhEv2wZWq762eEgYfNIILiH14YLgPn5wxI3tTUS0NwLQak7z2T5CAKM54k1VfhEHDEtaG2D7F2quZ49cfyNCgOFHRQH8+Jya/+LfkGg/jDHHw5mPqfmaV1TquiCsf1uNEy5V7TQDgdR8iIiGtkao2qO3NR4hjrigkPpwQXAfPyinR7VUAmA1RmKJjPfZPkIAY06AmFQ1r96rry2hyo6v1EVdymDoN1lva/yHKKeHH4vuB2sbDJ0NI8/sfF/e8TDkJLC2w4/P62OfEDhU7oF9KwADjL9Yb2ucGE2QMULNDwV3ero44oJC6sMFwX38EBGPaqkAoNWcGjin0YL/SRmkxipxxH3ChvlqHHN+eP2fiRBgeFG2XaUaA5xyf9ePmX6LGte/BS31/rFLCEw2vKPG/FnO94pAIdOenh7kdeLiiAsKqQ8XBPfRWpj5UKwt0h4RbzOn+mwPIQhItjviEhH3PnWlsPMbNZ9wmb62+BtJTQ8vlv4TsMHIs511toeTf5JK/W2pdfaOFsIPm82plh6I74tZdsG2IFdOF0dckPpwQegrfnDEtdR0qQ8Pc7SIuAi2eZ+N74DNAgOmQcZwva3xLw5HXCLiIU9VIWx8V82Pu7P7xxmNMPkaNd8ojnjYsn+Vqr+OjFMHN4FGiCiniyMuSH24IPQVf6SmN2uOuETEwxpNsE1S072LzQbr3lTziZfra4seOFLTJSIe8qx4Wh045Z8I/af0/Ngx56mxcBlRTYd8b5sQeGjR8NG/UEJ+gYbmiFcWQHuLvrZ4gDjigtSHC0Jf8YMjrqWmt0aLIx7WJA9Wo6Sme5fi9Ursx2RW9eHhhhYRrysBS5u+tgi+o6EC1v5PzWfe0fvjUwapDBFsZO3/0qemCQFIe4uznWOg9A4/nIRsMCeBzao6AQQp4ogLUh8uCH3FL6rpSqxNasTDnI5ibTabvraEEppzMurs8MwIi8sAYyRgg/pSva0RfMWqF6G9CXImKmV0V7AfTGUVfe47u4TAZMeX0FyjDuoC1TcwGCB9mJqX79DXFg8QRzzckfpwQeg7flFNl9R0AUjKVWNbAzRW6GtLqNBc6+yRO+lKfW3RC6PR2UdaWpiFJq2NsPIFNZ/xG9e7Aow5FzCQXP4z5sYSX1knBCLa++L4i1WrsEAl3a7pUb5TXzs8IEJvA3yKzYrRZvHJ0s3NzT5Z1+/sWQnxuZAxCgzRECo/lw8wWv2btmc1mNQBiRC4+FE1XcTawpzIaEjIgbpilZ4el663RcHP+regtQ7SR6i62XAlsb8SAZQ68dBk3TxoqoSUwTDqF64/L7GfqiU/sJq04iUcHHKJz0wUAoiGctj5tZqPD9C0dI0QiIiHpiNusxHdXkcMzRgMBnzREXTPHt9FwPxKeybMeFw5FHv26G1NQJNi9c2hTlfYAJvNRhPR2GyZGMKpr20w4UexNklNF0gepBzxqsLexZaEnrFanVHCo28Mr97hhyO9xPWlogB2LYLa/UqhOmc85J8AkTGer21pgxX/VvPpt4LJzcv+4afDgdVkFC8WRzxc2PQ+WNtVGUPmSL2t6RlHRFwc8YAiur2OeEMr6RlZmKOjfeLExEdHen1NXSi3gDVGpT1qToXQJfXN/ouI22w2WpqbKS8ro6SkhJycHL/tLbiBFhFvrvHZFo7U9GiJiIc9qflQ9GNQC9MEDAWLVFmWOSnwoz6+RnqJ60N1EXz5B9j26ZH3xaSoFmIz7/BMu2Dt/1QGTWw6TLzC/ecPPw2++xuppSswtjdjjYjuuy1CcBDIvcMPp2Nqus0WlAeqoeeI26zE0Ex6RhaJySk+2yY6FBzx9lYwtoHRAAkpYAy9l4M3abX5t07GHK1Ow6urK8jMzMRkCuA6nXAlOkmNPnLEje2NmCxNgNSICzh7XAfx6X/AsPJ5NU6+KjBb8/gT6SXuf4p+gjcvUSnjBqMSUMsYpcqcdi9R0fHlT6i08tMfgXEXur9HayMsfkTNj/8dRMW6v0b2OJpjsohuKiWlbCUVObPcX0MIHsq2w8G1yh8Ye4He1vROap6yta1BvX8l9dfbIrcJOc/LaLNgMBgwR8upXa+01qsxMlac8ADFHB1NHdDW1iaOeCCiRSqaa3xyGqtFw63GSCwRcV5dWwhCtNP/su362hHslO+EXQsBA0y7Xm9r9EcTaxNH3D8Ur4c3zlPXYDkT4LwXIHOU836rRalWL7xPHbq9f51KXT/zMfcOjX58FupLIHkgTL22b7YaDJTnnMiA3W+TfvA7ccRDHU2kbegpEJ+hry2uYIqElDyo2Kn+V4LQEQ9JJSgDSE2tK2iOeFSYRwMCGHkdBzhaRNxmgdYGry8f1VGoTV4LQvoINVbsUjXOQt/46T9qHHGGiqiEOxIR9x8NFSoS3lqv2kJd+0VnJxyUSvXIs+Cm5TDrDypivv5N+M8sKNno2j4VBfD9Y2p+4p8hwtxnk8v7KSHD9OLF0joxlLFaYcN8NQ/U3uFdkWH/XAxS5fSQdMQFF2mxO+LhnpYnCH2lYzaJD9LTI5tVmypJSxcApXpsjIS2RpW6KrhPcw2se1PNj/6VvrYECppYW32JisYKvsFmg09uU4KLacPgkv9BVA+ZThFRcOLdcM2n6rCkYhe8eDKsfqVnh7itGT64Edqblejb+Is9Mrsy8xgsJjMxjQeJq5GymJClcKnSiYhOUiJ9wUKQK6eLIx6utLeCpUXNe/ogEAShewyGDnXi1V5fPqqlChChNsGOKQLShqh5kF506M66N1U0MmMk5EmaLQDxWWAwKaXkhjK9rQldtn2mhNmMkXDhy66LsA2eATctg2Gnqeu2T29X6er1XfytLG3w8c1wYLX6bDrnKY+zqawRMVRlHgPYo+JCaKKlpY85X7XLDBaCXDldHPEAoqSkhF//+tfk5+djNpvJzc3lnHPOYdGiRd7fLIzqwwsLC1UbO/tXWloap556KmvXrtXbNCEUiE5Wow8i4lEtKiLeZvad8KQQZGin/2XBedGhK1arMy396F9JuYeG0aSccRDldF/R1gxf/VHNZ9ymasPdITYVLnsbTrlfHZpseh/+PUWln1cVKge8aBW8PkfdZzDBha9AyiCvmF+ecwIgjnjI0tYEWxeo+fgga1PXUTk9CBFHPEAoLCxkypQpfPvttzz22GNs3LiRL7/8khNPPJFbbrnF+xt6oT68rc1/7bxcwWKxYO2hbnLhwoUUFxfz1VdfUV9fzxlnnEF1dbX/DOyBQPtdCm7gQ+X0yI414oIAzjrxID3915VdC6Fyt/qfDbaLTV8jvcR9yzp7G7GEHJh5Z9/WMBphxm/gum+UI99SA9/+DZ6cAA+kw8uzYe9yFWC57C0YerLXzNcc8eSKtUS0VHttXSFA2PGl8guSBkLu0Xpb4x5pQ9VYdxBa6vS1pQ+IIx4g3HzzzRgMBn766ScuuOAChg8fzpgxY7jzzjv58ccfHY/bt28fc+bMIT4+nsTERC6++GJKS0sd9993331MnDiR//73vwwcOJD4+HhuvvlmLBYLjz76KNnZ2WRmZvLg3/+hnmDvHW4wGHjuuec444wziImJIT8/n/fee8+xrhZVnj9/PrNmzSI6Opp58+YB8NJLLzFq1Ciio6MZOXIkzz77rON5ra2t3HrrreTk5BAdHc2gQYN4+OGHAdUr+7777mPgwIGYzWb69evHbbfd5nhuVVUVV199NSkpKcTGxnLGGWewc6fzxOvVV18lOTmZBQsWMHr0aMxmM/v27ev2d5yWlkZ2djZTp07lH//4B6WlpaxcuRKA999/nzFjxmA2mxk8eDCPP/6443lPP/00Y8eOdXz/6YKPSYqN4uUX/+O47Rdnnc4D993j+P6zTxZw3PSjyExJYPzoETzy4AO0t7c77k+KjeKl/7zApReeR056Mv/4+8Pd2i0EOD50xJ1ibVIjLtjJEEe8zzhall0tJVmH43DEi/W1IxSxtMGyJ9T8uN96rsszYArc8B2c9x8YOF2lugNEJcC4i+H/rVD9v71Ic1x/6hOHYbBZSStd5tW1hQBgo/16f9yF6sAnmIhJhrhMNa/YpaspfSG0c5Lt2Gw2mtq8K0ASYeo9pS0m0uSS6nVlZSVffvklDz74IHFxR14cJCcnA2C1Wh1O+JIlS2hvb+eWW27hkksuYfHixY7HFxQU8MUXX/Dll19SUFDAhRdeyO7duxk+fDhLlixhxdIl/PKGXzF7xjSOPnO843l/+ctfeOSRR3jyySd54403uPTSS9m4cSOjRjkVPf/whz/w+OOPM2nSJIczfs899/D0008zadIk1q5dyw033EBcXBzXXHMNTz31FAsWLOCdd95h4MCBFBUVUVRUBCjn91//+hdvv/02Y8aMoaSkhPXr1zv2mjt3Ljt37mTBggUkJibyf//3f5x55pls2bKFyEj1wdPY2Mjf//53XnrpJdLS0sjMzOz19w0QE6N6dLe2trJmzRouvvhi7rvvPi655BJWrFjBzTffTFpaGnPnzmXWrFncdtttlJeVkZ6RwfJlS0lLT2fZ0iVcd8ONtLW1sWrlj9zx298BsGL5Mm664Zf8/R//ZPqMmezZvZvf3Hqz+v396S8OGx556AHuu/9BHn7scSIiwuJfMTTR6vyaqr2+dFSzlpoujrhgx5GaLi3M3KJsBxQsUgrU027Q25rAw6GcLqnpXmfDfKgpUs7CpCu9s6bRBBMuUV9tzUrA0ZyodCR8RHnOCcTX7iT94GJKB57ts30EP9NUBTu/VvNxF+lrS19JzYeGQ1C5B/pN0tsatwiLq/+mNgvHPPyt3/fdcv9pxEb1/ivetWsXNpuNkSNH9vi4RYsWsXHjRvbs2UNubi4Ar7/+OmPGjGHVqlVMmzYNUA77f//7XxISEhg9ejQnnngi27dv5/PPP8doNDJiQCp/f+Rhvlu5nqPPvsqx/kUXXcT116ueqg888ADffPMN//73vztFuG+//XbOP/98x/f33nsvjz/+uOO2vLw8tmzZwgsvvMA111zDvn37GDZsGDNnzsRgMDBokLNead++fWRnZzN79mwiIyMZOHAgRx11FIDDAV++fDnHHnssAPPmzSM3N5ePPvqIiy5SbxZtbW08++yzTJjger1VdXU1DzzwAPHx8Rx11FHceeednHzyyfzlL8pJHj58OFu2bOGxxx5j7ty5jB07ltTUVJYt+55zz7uApd8v4dbbbuf5Z54GYM3qVbS1tXH0MdMBeOShv3H7b3/H5Vdebf+d5PPne+7lnj/9sZMjftHFl3Ll1de4bLcQoPgjNV3E2gSN9OGAARrLoa4UErL0tig4WPWiGkec6bW62ZBCeon7BpsNlj+p5sf+GiJjvL9HZLRfxLXK+53A4O0vklbyvVLXN5p8vqfgB7YsAEsrZI6BrNF6W9M3UvOh6EdVehRkBFn+QWhic7Ev49atW8nNzXU44QCjR48mOTmZrVu3Om4bPHgwCQkJju+zsrIYPXo0Ri3dpLmOrIxUDlV1rqWYPn36Ed93XBdg6tSpjnlDQwMFBQVcd911xMfHO77+9re/UVBQAKio9rp16xgxYgS33XYbX3/9teP5F110EU1NTeTn53PDDTfw4YcfOtK3t27dSkREBEcf7axVSUtLY8SIEZ1sioqKYvx4Z1S/J4499lji4+NJSUlh/fr1zJ8/n6ysLLZu3cqMGTM6PXbGjBns3LkTi8WCwWDg+OOPZ9n331NdXc32bVu5/sabaGltYcf2bSxb+j2Tp0wlNjYWgE0bN/Doww/SLyPF8XXbLf+PkpJiGhsbHXtMmjzZJbuFAEdS0wV/EhXnjIqXbNDXlmChpR7WvaXm067X15ZARXqJ+4a9y1UZSWQcTJmrtzUeUZM2ibbIRKJaq0mqXN/7E4TgYOO7ahx3ob52eEJqnhqr9uhrRx8Ii4h4TKSJH+8+yatrJsZEurSvKwwbNgyDwcC2bds8NQvAkbatYTAYnLfZrNBah8FgwGpw/8/fMXW+vl4Jvr344oudHGYAk0n97JMnT2bPnj188cUXLFy4kIsvvpjZs2fz3nvvkZuby/bt21m4cCHffPMNN998M4899hhLlixx2Z6YmBiX0v8B5s+fz+jRo0lLS3Ok+7vKCSecwPMvvMAPy5cxfsJEEhMTmTFjJku//57ly5YyY+Zxjsc21Ndz95/v4Zw55x6xTnS089Q6NlZqFEMCPzjikpoudCJngrq4L14Pw07R25rAZ+M70FqnRH3yT9DbmsDEUSMuqeleZfUrahx3IUQn6muLh9iMEVRkzyS76HPSi5dQky7BhKCnoVwdFgGMvUBfWzwhNV+NlcHniIdFRNxgMBAbFeH3L1cdxNTUVE477TSeeeYZGhoajrhfU/YeNWpUpxprgC1btlBdXc3o0S6mk7Q2KmccwxFtyzqKwmnfd6wPP5ysrCz69evH7t27GTp0aKevvLw8x+MSExO55JJLePHFF5k/fz7vv/8+lZXKwYiJieGcc87hqaeeYvHixfzwww+OuvT29naHmBpARUUF27dvd/1nPYzc3FyGDBlyhBM+atQoli9f3um25cuXM3z4cMeBwqxZs9i2dSsfffg+M48/HoCZx89i8XeLWPnDCmYe7+xHO2HiJHbu2MGQIUOP+DIGmwiG0DuO9mXVXl3W2N6IydIMSERcOIxsexZQsUSlesVmg1X/VfOpv5SWZd2hOeJ1xep3JnhOQ4WzJdTUa/W1xUtIG7MQY8eXyifIHh/cJTspdp8jCFPTwyIiHgw888wzzJgxg6OOOor777+f8ePH097ezjfffMNzzz3H1q1bmT17NuPGjeOKK67giSeeoL29nZtvvplZs2Z1ShnvEU3a32g64oLk3XffZerUqcycOZN58+bx008/8fLLL/e43F//+lduu+02kpKSOP3002lpaWH16tVUVVVx55138s9//pOcnBwmTZqE0Wjk3XffJTs7m+TkZF599VUsFgtHH300sbGx/O9//yMmJoZBgwaRlpbGnDlzuOGGG3jhhRdISEjgD3/4A/3792fOnDl9+RV3y29/+1umTZvGAw88wCWXXMIPP/zA008/3ak2fvz48SSnpPDu/Ld55/2PAJh53PH8+e7/w2AwcMz0Yx2P/f3df+KSC84lNzeXOeedj9FoZOPGDWzdvJm/3He/V20XAgAfRcQ1oTaLMQpLhGRPCB3IsTvikpreO/tXQelGiIiBiZfrbU3gkmCvEW9vVuJNsXL45zEb5qva25yJQScg1R0V2cdjw0BC9VbMjSW0xGbrbZLgCds+U+PIIBff01LT64pVwDEqVl973EDCcwFCfn4+P//8MyeeeCK//e1vGTt2LKeccgqLFi3iueeeA1Rk/+OPPyYlJYXjjz+e2bNnk5+fz/z5813fqKVWjYYj0+b/+te/8vbbbzN+/Hhef/113nrrrV6jz9dffz0vvfQSr7zyCuPGjWPWrFm8+uqrjoh4QkICjz76KFOnTmXatGkUFhY6ROOSk5N58cUXmTFjBuPHj2fhwoV88sknpKUpYapXXnmFKVOmcPbZZzN9+nRsNhuff/75Ean3njJ58mTeeecd3n77bcaOHcs999zD/fffz9y5cx2PMRgMHHvsDOV0H6vqyceOG09CYiKTJk/plLI/+5RTmf/+R3y7aCEnHncss084jmf//RS5A4P4tFHoHh9FxB1p6dFpEsUTOqNFxKsKldMkdM8q+2Hy2AsgJkVfWwKZCDPEpqu5pKd7B6321ltK6QFAW3Qqtanq/Set2PUyQiEAaW2AAruQ9ciz9LXFU2JTnUGRqkJdTXEXg81VpbAAora2lqSkJD5auZO4+IRO9xmtbaRYq8kdOIgos+9UJF2pEQ84LG1QuknNM8dARJTjLoPBwIcffsi5556rj21BQG1Tm9/3bG1ppqx4P3l5eZ3qy4UAomgVvDwbkgfC7Rs9Xm7hllIA0g9+x8Rlv6I2ZQw/nfKh2+vMHi1q2nqg/f0Ox+t/j6cmQ2UBXPGe1Il3R0s9/GOYau103ULInaa3RV6ju9dZR9x+zT1/nMqyuPwdr/eh7iuu/Jy9oct7YUUB/HuyCnr8djvEZ/jfBi9x+N8gb/MzDNn8JIf6ncyGmSpQJJ83QciWBfDOVZA8CH6zPvgP/P9zAhxcC5fMg1G+jfBrfmhNTQ2JiZ5pP0hEPJxotkfDI2M6OeGCIHiA1kfcy6npkaKYLvRErmr1SNFP+toRyGz9RDnhqUNggIvlW+GMKKd7j03vqzF/VlA74V1R3u8EAFIP/YDR0qKvMULf6ZiWHuxOODgF24JMOV0c8XBCcxS09A1BEDzHUSNeC1ar15YVxXShRxyO+MqeHxfObLCXbU24NDQuNH2N9BL3DjYbbHxPzccGcUuobqhLHk1zTBYR7Y2kHPqx9ycIgYelXQm1QfCnpWsEqWCbOOLhglW1LQPAfKQjbrPZJC1dEPqC42DL5tRg8AKaWFurOc1rawohRK69ZeSBNWC16GtLIFJbDHvsNazjLtLXlmDB0cJMHHGPKN8J5dvBFOXzFFldMBgo76daAmccWKSzMUKfOLBG6dpEJzs/S4IdRwszccSFQKS1TrUoMEaq1HRBELxDhFkpMoNX09MlNV3okYyRYE6E1npRT++Kje+qz7zcY5yKukLPOFLTRazNI7RI4+CZIZuBWNbvZADSi7+1t8QVgord36kxfxaYQqSBlvY+H2S9xMURDxc6pqVLip4geBcftDCLalERcUlNF7rEaFIX+gC7Rb34CDa8o8YJl+hrRzDRsZe40Hd2fKXG4afra4cPqcw8hvaIOKKbDpFQtVlvcwR3KbA74kNO0tcOb6JFxGuKoL1VX1vcQBzxcMBmcwq1hejprCDoisMRr/baklEtqi1Va7Q44kI35M1S4+7FupoRcFTuVr3DDSYYfa7e1gQPCZKa7jFNVbDvBzUfdqq+tvgQmymKimx1ECjp6UFGcw3sX6Xm+Sfqa4s3ic+CyFiVoVG9T29rXEYc8XCgtQGsbeqixByvtzWCEHr4ICIuqelCr+SfoMZ9P0Bbs66mBBRbP1Xj4Jmqv6zgGppYW0ut8/BecI9di8BmUaUjIV4SoaWnZxwURzyoKFymXqOp+ZAySG9rvIfBEJSCbeKIhwNNKrKm0tLlTy4IXscHLcxENV3olYwREJ8N7c2int6RbXZHfNQ5+toRbJgTnGKukp7eNxxp6YHRh92XVOTMwmYwklCzHar26m2O4CqhmJaukTJYjdXB83oUryzUsdmc6bIxKbqaIgghixYRb6r2ynLG9kZMFhXhlIi40C0GgzMqLunpiroSZ2/1UGnL408cyuki2OY2Vgvs+kbNQ7g+XKPNnEJ1+hT1zfYv9DVGcB2HUFsIpaVrJA9Uozjigh4sXrwYg8FAdXW188aWOrC2gzHC5bT0LtcJQebOndtry7YTTjiB22+/3fH9uJHDePbpp3xrmBB8aIdcWvaJh2jRcIsxCktEnFfWFEIUzREv+FZXMwKG7Z8DNug/xelUCq7j6CUuEXG32b9KfQZEJ8OAo/S2xi9o6enq/04IeKqLoGKXKlXNO05va7yPlmovNeKCu8ydOxeDwYDBYCAyMpK8vDx+//vf09zsYd1fL2nphzuaAMceeyzFxcUkJflO2K2wsBCDwcC6detcsskXPPnkk7z66qtuPee7pSuY+8vrHd8nxUbx6YKPvWyZEHR42xFv7qCYLl0OhJ7Q0guL10H9IV1NCQh22iOSI87Q145gRXqJ9x2tbdmwU0KnJVQvlNn7ibN3udcywgQfsne5GvtNCk3xZi0iHkSlEuKIBxCnn346xcXF7N69m3/961+88MIL3HvvvX1f0GrpkJbuenprVFQU2dnZGELcAUhKSiI5Odmt56RnZBAbG+sbg4TgxeGIV3plORFqE1wmIQtyJqj5rjAXTWpvhT3fq/nQ2fraEqxIL/G+EwZtyw6nKWEw9YlDVOblroV6myP0hqboP2i6vnb4imQtIi6OuNAHzGYz2dnZ5Obmcu655zJ79my++eYbx/1Wq5WHH36YvLw8YmJimDBhAu+9916361XsL+Cy//d/9J9yOrEpmYwbN4633nrLcf/cuXNZsmQJTz75pCMaX1hY2Ck1vba2lpiYGL74onP9z4cffkhCQgKNjY0AFBUVcfHFF5OcnExqaipz5syhsLDQK78Xg8HARx991Om25ORkRzRbi66/8847HHfcccTExDBt2jR27NjBqlWrmDp1KvHx8ZxxxhmUlZV1+vk7pqY3NDRw9dVXEx8fT05ODo8//vgRtnRMTR83chgAV1x6EUmxUYwbOYy9ewtJjjPz85o1nZ737NNPMXbEUKxWqxd+I0LAoR10eS01XWtdluaV9YQQR2uTtPNrfe3Qm/0/QWs9xKZD9gS9rQlOJCLeN6r2wqEtKuU3FEWwekDS04OIvXZHfGCoOuL2iHhTVdB0fggPR9xmUy28/P1ls/XZ5E2bNrFixQqioqIctz388MO8/vrrPP/882zevJk77riDK6+8kiVLlnS5RnN1KVPGj+Kz999k06ZN3HjjjVx11VX89JMSsnnyySeZPn06N9xwA8XFxRQXF5Obm9tpjcTERM4++2zefPPNTrfPmzePc889l9jYWNra2jjttNNISEhg6dKlLF++nPj4eE4//XRaW1v7/Dtwl3vvvZc///nP/Pzzz0RERHD55Zfz+9//nieffJKlS5eya9cu7rnnnm6f/7vf/Y4lS5bw8ccf8/XXX7N48WJ+/vnnbh//3dIVADz7wkvs2L2P75auYNCgwZxw0snMe+O1To+d98ZrXH7lVRiN4fEvF3b4qEa8zSwCi4ILDD1FjQXfgqVdX1v0RMsIGHIiyHtt39Ai4nXiiLuFdgg28Jiwa5lXrjniO79RWSlCYNJQAeXb1TxUHfHoROf1WJDUiYdHEUtbI4n/0qFX3h8PQpTrQkuffvop8fHxtLe309LSgtFo5OmnnwagpaWFhx56iIULFzJ9uvoHys/PZ9myZbzwwgvMmjWr82JtTfRPj+eum66GrLFgiuTXv/41X331Fe+88w5HHXUUSUlJREVFERsbS3Z2drd2XXHFFVx11VU0NjYSGxtLbW0tn332GR9++CEA8+fPx2q18tJLLznS2V955RWSk5NZvHgxp556ardrH3vssUc4p01NTUycONHl35vGXXfdxWmnqZYhv/nNb7jssstYtGgRM2bMAOC6667rtia8vr6el19+mf/973+cfLL6UHnttdcYMGBAt/ulZ2QAKsU9q8Pv7+q513LHbbfy0N8fw2w2s27tWjZv2sSb77zv9s8kBAnahVejdxxxSU0X3GLAVHXx0VQFB1YrZyAcKdAc8ZP1tSOYSdDE2sQRdwtHfXj31zuhSk3qeIjLgIYyVYM8JATVuEOBoh/VmDEytA+Lkgepz8LqfZA9Vm9rekWOjAOIE088kXXr1rFy5UquueYarr32Wi644AIAdu3aRWNjI6eccgrx8fGOr9dff52CgoIjF2sow2Kx8MDTrzNu4mRSU1OJj4/nq6++Yt8+906JzjzzTCIjI1mwYAEA77//PomJicyerWrw1q9fz65du0hISHDYlZqaSnNzc9e2dWD+/PmsW7eu09fUqVPdsk9j/PjxjnlWVhYA48aN63TboUNdixkVFBTQ2trK0Ucf7bgtNTWVESNGuG3H2efMwWQy8cmCjwB483+vc9ysExg0aLDbawlBgs8i4iH8YSl4D2OHdNhwTU+vL4Pi9WoeZqnBXkVLTW+sgDYPxWLDhZZ6pzZBGNWHOzCanD+3tDELXLT68FA/qA2yFmbhERGPjKX2Du/+QRJjIl3a1x3i4uIYOnQoAP/973+ZMGECL7/8Mtdddx319fUAfPbZZ/Tv37/T88xmc+eFLO3QUsVjz73Ok/+ZxxNPPMm4ceOIi4vj9ttvdztdPCoqigsvvJA333yTSy+9lDfffJNLLrmEiAj18qmvr2fKlCnMmzfviOdm2KPG3ZGbm+v4mTViYmI6fW8wGLAdlubf1tZ2xFqRkc6/iRaZP/w2f9RoR0VFcdnlVzLvjdf5xZzzePedt/n7Y0fWmwshhOaIt9ap1LyIqJ4f3wtRLUo1XSLigssMOxU2va/SQ0/uvgQnZNF642aNUwJ2Qt+ISYGIGGhvUunpqfl6WxT47FkCllYVictw//A+JBhxJqx9Q9WJn/F36fYRiDjqw4/V1w5fE2QtzMLDETcY3EoRd4koFxxxDzAajfzxj3/kzjvv5PLLL2f06NGYzWb27dt3ZBr64TRWgsnK8tUbmfOLOVx55ZWAEnvbsWMHo0ePdjw0KioKi8XSqz1XXHEFp5xyCps3b+bbb7/lb3/7m+O+yZMnM3/+fDIzM0lMTOzbD9wDGRkZFBc7e5ru3LnTIRLnLYYMGUJkZCQrV65k4EB1mlZVVcWOHTt6/H1HRkZisR75+7t67rUcM3USL/3neSzt7Zwz5zyv2isEGNFJgAGwqU4F8ZkeLedMTRexNsFFhpwMGKBkA9SVQEL35UYhidZHfaikpXuEwaCi4pUFKj1dHPHe0dLSh58evg5o/gnqAKemCEo3Qfa4Xp8i+JHWBtXiEsIgIm53xIOkhZmkpgcwF110ESaTiWeeeYaEhATuuusu7rjjDl577TUKCgr4+eef+fe//81rr3UWBqOxHIBhI0byzcKFrFixgq1bt/KrX/2K0tLSTg8dPHgwK1eupLCwkPLy8m4jxscffzzZ2dlcccUV5OXldUrhvuKKK0hPT2fOnDksXbqUPXv2sHjxYm677Tb279/v8e/hpJNO4umnn2bt2rWsXr2am266qVOk2xvEx8dz3XXX8bvf/Y5vv/2WTZs2MXfu3F7F1QYOGsSS776jtKSEqipnWvKIkaOYdtTR3PvnP3LBRZccEeUXQgyjydmTs9HzFmaaarqkpgsuE5+hesNCeLYRKrT3x807Xl87QoEke9Zdjeef3yGP1Qo77OUgw0/T1xY9iYp11oZLenrgcWCNajGX2N+Zuh2qBFkLM3HEA5iIiAhuvfVWHn30URoaGnjggQf4y1/+wsMPP8yoUaM4/fTT+eyzz8jLy+v8RGs7GCP5830PMHnyZE477TROOOEEsrOzO7XrAiVwZjKZGD16NBkZGd3WjxsMBi677DLWr1/PFVdc0em+2NhYvv/+ewYOHMj555/PqFGjuO6662hubvZKhPzxxx8nNzeX4447jssvv5y77rrLJ728H3vsMY477jjOOeccZs+ezcyZM5kyZUqPz3nw4Uf57ttFjB6ez/HTj+p031XXXEtraytXXj3X67YKAUis91qYiVib0CfCtY1Z9T6o2adaR+Ue3fvjhZ5x1FgGR2qnrpSsh/oSiIyDwTP1tkZfRpyhxm2f6WuHcCT7V6txwLTQz9romJruQfcqf2GwHV58GwTU1taSlJTERyt3Ehef0Ok+o7WNFGs1uQMHEWWO9pkNLtWI+xubFUq3gLUNkgYoFUvBa9Q2HVmX3hOPPvwgH334Pit+6r4FWm+0tjRTVryfvLw8oqN993oWvMCLJ6lT50vfgpFn9nmZbzcUctIHqgfyd+euwRKV0Mszumb2aKmT1YOFW0q7vN0vf4/9q+Glk8GcCL/fDaYA/JzyBevnw4c3Qv8pcMO3elvjF7p7nXWkz6+5JY/Cdw/CpCthzjN9W8NLuPJz9oZP//cW/x0WPwQjz4ZLj9TJCQVcfq3VH4J/DAdscMcWZ2aFoD/vXA1bPobZf4WZt+ttjW9pbYSH7N0ffr/HJwrxmh9aU1PjccBRIuKhRGOFcsKNkRAjtaV6UV9fz5bNm/jPC89x40236G2O4C9itIi4Z6npmmK61RiJJTLeU6uEcKLfJIhNg5ZaKPpJb2v8x95lahwU4iJE/iLIaix1pWN9eLgTn6kiruD8vQiBgdZRot9EXc3wC1GxEGfX6QmCrB5xxEMFq1WdRgLEZ0Evtc2C7/jdnb9h1oxjmHnc8Vx1zVy9zRH8hZdamHVKSw/1FDLBuxhNzh7a4ZSevneFGgeFeWqwt5DUdNeoK4GD9oy3MOwf3iVDVVtbCpfqa4fgpKkKqgrVPGeCrqb4jZTgqRMXby1UaChT7TOMkSoiIujGc/95mbLqel59401MJpPe5gj+QnPEPRRrkx7igkdoDkG4CLbVlULFLsAAA6U+3CtojnjtAdUOVegaLerbf6q0zNMYPEONhcuDoj43LNCi4SmDndcpoU4QHSaKIx4KWNqUWAiotiMSDRcE/+MlsbYoEWoTPGGovY1Z6SaoOaC3Nb5nnz0anjU2fC4yfU1CjjrUt7arXuJC12z7XI2aSJmgDiVMZmg4ZD8gE3Tn4Do15kzU0wr/EkTlNeKxhQJ1xUqoLTJWLkQEQS8cqemeRcRFMV3wiNhUGDBVzXd9o68t/sCRli714V7DaITkXDUPgoiSLrQ2wO7Faj6i7+KcIUdktPP9p3CZvrYICq1/eLikpUOHiLg44oKvaWtSIm2g+gNKTakg6EOMdyPikpou9BlHG7NwcMR/UOOg6fraEWokd2gBJBxJwXdgaVG/p8xRelsTWAyyp6fvXa6vHYJCi4iHg1CbRkrwvH+JIx7M2GxQs1/No5PALArLgqAbXhJri2qWiLjgIZpg0u7F0N6qqyk+pbURDm1R8wFH6WtLqKFFlIIgtVMXtn+hxhFnSgDkcKROPHBoqoaqPWoejqnpQdBLXBzxYKapClrrAYOKhguCoB+xmlibF1XTBaEv5EyEuAz1+VD0o97W+I7STWCzqFY1if30tia0CCKxI79jtTiF2qQ+/EgGHAXGCKUvIK8ffSnZoMbkgT7ppx2wJA0ADNDWCA3lelvTI+KIByuWdqVoCpCQDRFmfe0RhHDHWxFxLTU9Oow+NAXvYjQ6o+Kh3MbsgL11VP/JEpX0NimD1SiO1JHs+wEay8GcJNoEXREVq8QTAQ6s0deWcCcchdpA+UTa4WyA14mLIx6s1B1QiqYR0RCfqbc1giBojnhbA7S39HkZiYgLXkHrJ77ne33t8CUH16qx3yR97QhFgkjsyO9s+kCNo84GU6S+tgQqmmCbOOL6ogm1hVN9uEaQvIeJIx4AGAyGHr/uu+++zk9oqXf2Kk7KBUPw/RkHDx7ME088obcZguA9zElgsPeN1wQU+4CItQleQYvUlWyE5lp9bfEV4oj7jtR8NdbsV6KwgsLSDlsXqPmY8/W1JZDpP0WN4ojriyMiHkaK6RpB0sIs+Dy4EKS4uNjx9cQTT5CYmNjptrvuusv5YJsVauypYrFpASXQZrPZaG9v9+uera0hLEQkBBdGI8Slq3lfa5LamolobwCg1ZzmJcOEsCSpv4oI2Kyw/ye9rfE+LXVQvkPNxRH3PrFpSgQWG1QU6G1N4LB3GTSUqS4Z+bP0tiZw6W+PiB9cpw4vBP/TXAuV9v/dnDB8j5SIuOAq2dnZjq+kpCQMBkOn295++21GjRpFdHQ0I0cM59mX3lBCGIn9KCwsxGAw8M4773DccccRExPDtGnT2LFjB6tWrWLq1KnEx8dzxhlnUFZW5thz7ty5nHvuufz1r38lIyODxMREbrrppk6OrdVq5eGHHyYvL4+YmBgmTJjAe++957h/8eLFGAwGvvjiC6ZMmYLZbGbZsmUUFBQwZ84csrKyiI+PZ9q0aSxcuNDxvBNOOIG9e/dyxx13OKL+APfddx8TJ07s9Lt54oknGDx48BF2P/jgg/Tr148RI0YAUFRUxMUXX0xycjKpqanMmTOHwsJCL/6VBMEF4jLU2FDW8+O6o1E58FZjJO2RCV4ySghbBtqj4vtCULCteD1gg8QBUp7lCwwGSBum5hU79bUlkHCkpZ8jaek9kTZUZYm1Nzk7Gwj+RRNqS8qFuDA82E8Jjoh4hN4G+AObzUazpdmra0a0tfX6mJiIGIeT2VfmzZvHPffcw9NPP82kcaNZu+QzbvjdA8SlD+CaG8c5HnfvvffyxBNPMHDgQH75y19y+eWXk5CQwJNPPklsbCwXX3wx99xzD88995zjOYsWLSI6OprFixdTWFjItddeS1paGg8++CAADz/8MP/73/94/vnnGTZsGN9//z1XXnklGRkZzJrlPAn+wx/+wD/+8Q/y8/NJSUmhqKiIM888kwcffBCz2czrr7/OOeecw/bt2xk4cCAffPABEyZM4MYbb+SGG25w+3eyaNEiEhMT+eYb1SO3ra2N0047jenTp7N06VIiIiL429/+xumnn86GDRuIiorq669fENwj1v5h19eIuP15bVEpIj4leM6g6bDhbWev7VDCkZY+UVczQpr0YXBgNZTv0tuSwKC1ETZ/qOZjL9DXlkDHaIT+k1QLxQNrIGe83haFH+Gclg6dW5gFMGHhiDdbmpn9wQy/77vy8pXERsZ6tMa9997L448/zvnnnQcVBeSdeRJbCvbzwqvzuObGWxyPu+uuuzjttNMA+M1vfsNll13GokWLmDFD/dzXXXcdr776aqe1o6Ki+O9//0tsbCxjxozh/vvv53e/+x0PPPAAbW1tPPTQQyxcuJDp06cDkJ+fz7Jly3jhhRc6OeL3338/p5xyiuP71NRUJkxw/uM/8MADfPjhhyxYsIBbb72V1NRUTCYTCQkJZGdnu/07iYuL46WXXnI42P/73/+wWq289NJLjoOPV155heTkZBYvXsypp57q9h6C0Ce8FBFvNad4ySAhrNEi4gdWKwHBUOqu0VExXfANaUPVKBFxxbZPoaVWpbwOPk5vawKf/lPsjvhqmHqt3taEH+Es1AbOiHhNEVit6nAoAAkLRzxYaWhooKCggOuuu05Fjm1WANotVpKSkjo9dvx452ljVlYWAOPGjet026FDhzo9Z8KECcTGOg8Kpk+fTn19PUVFRdTX19PY2NjJwQZVkz1pUudak6lTp3b6vr6+nvvuu4/PPvuM4uJi2tvbaWpqYt8+75xKjRs3rlOUe/369ezatYuEhM6pvM3NzRQUSG2b4Ec8dcTtEfHW6DBMIxO8T/owiE1XBzwH18HAo/W2yHuIUJvvSddS0yUiDsDaN9Q48cqAvagPKLT/zeIN+toRrjgi4mH6HpnQTwnoWlqhrljppgQgYeGIR5uiWXj+cq+umRDd+68uJiLGoz3q6+sBePGF5zl6aJpqVxaXCfEZmEymTo+NjHTWKmlR4cNvs1qtbu/92Wef0b9/5xev2dw5qhIXF9fp+7vuuotvvvmGf/zjHwwdOpSYmBguvPDCXoXVjEYjNput021tXZQAHL5ffX09U6ZMYd68eUc8NiMjo8c9BcGraGJtjX1MTa8vBaA1Ot1LBglhjcEAA49Rkbx9K0LHEW+qgqo9ah5u/XH9iVYjXr4LbLbwLpepKrS3AjTAxMv0tiY4yLYHg8q2QXsrREiZoN9oqXMeoIVraropApIGKLG26r3iiOuJwWDw2Ck+nNhI34t0ZGVl0a9fP3ZvW88VJ1+peoZnjPBau7L169fT1NRETIz63fz444/Ex8eTm5tLamoqZrOZffv2dUpDd4Xly5czd+5czjvvPEA5yocLp0VFRWGxWDrdlpGRQUlJCTabzXGYsG7dul73mzx5MvPnzyczM5PExES3bBUEr+KIiPfVEVdZKy3RcoAkeIlBxypHfO8PMPMOva3xDlo0PCUPYqXNn89IzQcM0FKjsnzCWRRv1ctqzD/BqcYs9EzyIDAnqnT+8h2QPVZvi8KHko0oMcv+EB/G1xMpg5QTXrXX2dIzwJDcmgDnr3++m4f/+SxPvfwWOw41s3HTZl555RX++c9/erx2a2sr1113HVu2bOHzzz/n3nvv5dZbb8VoNJKQkMBdd93FHXfcwWuvvUZBQQE///wz//73v3nttdd6XHfYsGF88MEHrFu3jvXr13P55ZcfEY0fPHgw33//PQcOHKC8XDktJ5xwAmVlZTz66KMUFBTwzDPP8MUXX/T6c1xxxRWkp6czZ84cli5dyp49e1i8eDG33XYb+/fv7/svSBDcxdG+rI+p6RIRF7zNQKXxQdGPqk4uFJC0dP8QGe10OsvDuE68pR5+tl/3HP0rfW0JJgwGZ1S8dJO+toQbjrT0iXpaoT9BINgmjnggY7Ny/QUn8dI//sIr737GuCnHMGvWLF599VXy8vI8Xv7kk09m2LBhHH/88VxyySX84he/4L777nPc/8ADD/CXv/yFhx9+mFGjRnH66afz2Wef9br3P//5T1JSUjj22GM555xzOO2005g8ubOgzv33309hYSFDhgxxpI+PGjWKZ599lmeeeYYJEybw008/de6h3g2xsbF8//33DBw4kPPPP59Ro0Zx3XXX0dzcLBFywb94WiNuj4i3SkRc8BbZ4yAyFpproHy73tZ4B3HE/Ue6tDBj/Vvq/yclD4adprc1wUWWPQpeslFfO8KNcBdq09AE2wK4l7jBdnhRbhBQW1tLUlISH63cSVx8Z4Euo7WNFGs1uQMHEWWO9pkNiTF+6B9ZVwx1JapneOYoNXqJuXPnUl1dzUcffeS1NUOd2qbeW9Z5m9aWZsqK95OXl0d0tO9ez4KXqNwNT01Sjs+fit1//jPHQNlW1sx6laosz9KoZo/O8uj5Qt9YuKW0y9t1/Xu8ejYULoWznwgN9eJ/joHa/TD3Mxg8U29rdKG711lHvPKa+/Ju+PFZOOZmOP1hz9dzE1d+zt7w6PdgtcAzR6l62zMeDcuIuEevtZ/fgAW3Qt7xcM0nXrZM6Janj1IHr5e/C8PDuHPQhnfggxtg0Ey49jOvLav5oTU1NR4H/CQiHqi0NUOd/c0vsb9XnXBBEHyEFhFva4TWBvef70hNl4i44EUGHqPGopX62uEN6g8pJxxD+IoQ+ZOsMWoM14jmpg+UEx6dDBMv19ua4ENLTS/ZpAT/BN/TUq9q8kEi4smBHxEXRzwQsdlU3ztsYE6AGOkpLAhBQVS8ElUE9wXb2luhqRKQGnHBy+TaHfF9P+prhzfQah/Th6vPR8G3dKzxDTdHytIOSx5R82NvlddbX8gYqQJJTZVQe1Bva8IDTagtoV94CyyCMzW99gBY/J/V6griiAciTZXQWg8YISnXJy1DXn31VUlLFwRvYzD0XTndXlduNUbSFpXkZcOEsCZ3GmBQLb/sOgRBy8Gf1Sj14f7B4UhVqYvZcGLTeyoaHpMCR4VfSrpXiIxWh2YQvlkV/qZ4vRolYwjis1RwxGaFmsAUbxZHPNCwtEGN/cMuMRsizD0/XhCEwCI2TY3uCrZpaenmNK+1KBQEAKKTIHO0mgd7VFyE2vxLhBnSR6h5ODlSlnZY8nc1P/bXEC3Cr31Ge+8p26qvHeGCCLU5MRhUQBMCNj1drvYCjdoDYLNARIwzsiYIQvDQV+V0Rw9xSUsXfMDAo9UYzHXiNpvTEe8/uefHCt6jY51vuLDxHSW+GZMKR92otzXBTcZINZaFSNeGQEdal3VGS0+vEkfcb9hsEIRi8NBSp9K/AJJzJSomBOfrONzRHPFGN1PTRahN8CWhUCdee1D9nxhMzrZIgu/JGa/GA2v0tcNfWNphyaNqPuM2qQ33lEy7I35IIuI+p7XB2aZSIuKKABdsCzkpbqshAosNykpLSElLJyIi0hcl1jQbLN5d0GaDyiKw2CA6BawmaG727h6CR7S2+E/owWaD9vY2KivKiTAaiYqK8tvegofE2SPa7taIO3qIp3nZIEHAGREvXg9tTRAZo689fUGLhmeOgqhYfW0JJwYcpcb9P6kPJ19cVAUSG99RegqxaTDtBr2tCX4yRqmxfAdYrWCUIJPPKNmk6qHjsyEhW29rAoMAj4iHnCOOwUBtZCrtzbU0HTyIwQC++MiIjjR5d0EtGm4wQkIUVOzx7vqCxzS3efnwpQdsqOudFiKYOiofo3xwBQ9aRNxdUSyJiAu+JHmQujirL4EDP8PgGXpb5D5SH64POePBZIbGCpWunTZEb4t8h6Udvv+Hmh97G5jj9bUnFEgZrF4/bY0qKpmap7dFoYvUhx+JIyK+T187uiH0HHHAZjDREJlMI1YMNqtP9jg2z4t1nE3V8MZ10FoLx/8ehhznvbUFr7Fil5sRTg+xGYzYkGh40KG1C2nomyMuNeKCTzAYVFR8y8dQ9GOQOuKimK4LEWb1Oy/6EYp+Cm1HfNP7UFmgasOnXa+3NaGBKQLSh6kWeGXbxBH3JaKYfiTJA9Uoqel+xmDAhgmbwcuRazvR0dHeW2zRP6ByM2SOgSmXqzctIeCwGiP1NkEIBrR0sLoS955nF3eTiLjgM3KPUY74viAUbOso1CaOuP/JnWZ3xH+EiZfpbY1vsFrg+8fU/NhbJRruTTJGOh3xEWfobU3oIkJtR5IyWI31pQFZliX5rnZWF1by+DfbeWd1EW0W30TRu6RyN6x5Rc3PeESccEEIdhJy1FhX7N7zJCIu+JqOyulWP37OeYPqvap8yxQFWWP0tib8GGTPoNi9RF87fMnWBVCx0943XJTSvYpDsG2bvnaEMm1N6qADJDW9IzEpEGUXXAzA9HRxxIFNB2p44fvdbC2u4+stpby72o9N3xc/AtZ2GHIy5B3vv30FQfANWkS8uQZaG117js0GdVIjLviY7PEQGQvN1Uo4KZg4YE9LzxqjUqUF/zJ4JhgjlIhZRYHe1gBQ2dDKxgM13ususvIFNU67QZTSvY0m2Ca9xH1HySbV/jgu0xkQEFRZVgALtoW9I26x2pi3ch82ICdJpZt/v7OM6sZW329eugU2vKPmJ//F9/sJguB7zInK2QEljOUKzTXQ1gBAS0yWjwwTwh5TJPSfouZFQdbGTNLS9cWc4GyBV/CtvrYApbXN3LtgM08u2sn81UWeL1i8Hvb9oA4bpv7S8/WEzmRqjviO4MvGCRY6CrWFemcDdwngOvGwd8Q3H6yhrL6FeHMEfzpzFPnpcbRbbazZW+X7zb97ELDBqF/IxYUghAoGg/t14loae0wK1ggv6k8IwuHk2tPTg61O3OGIT9bXjnBm6Elq3PmNvnYA320/RJO9k8l328uoa/awvejK/6hx9BxIlGii19GU09uboLpQb2tCE6kP754A7iUe9o748l0VAByTn0p0pIkpg1IAWLe/2rcbH9oK2z4FDHDSn327lyAI/sXdOvHaA2pM7O8bewRBY6A9qhlMEXGr1akGLIfW+jHcLrK1+zvV7UUnbDYbqwudwRKL1cbaIg/saa6BTe+p+VG/8sw4oWuMJkgfruZl2/W1JVQRxfTukdR0H+FhXVBdc5vD4Z4xRAkkjeufBEDBoQbafZk+s+Lfahx1NmSM8N0+giD4H3cj4rUH1ZjYzzf2CILGgGmAQQmFutvrXi8qC6ClFiJilPqyoA9Zo1Wtr6UVtn2mmxll9S1UN7URYTRwyihVyrO7rKHvC275GNqbIX0E5B7lJSuFI3AItkmduNdpa3bW34tQ25FIRNw3xNXt9uj5P+2pxGK1MTA1ltxUVdOZnRRNbJSJVouVosomb5h5JDUHnLXhM273zR6CIOiH2xHxg52fJwi+IibZWa9ZFCTp6Vpaes546SyiN2MvUOPGd3UzYdehegAGpcUyIluJqhWU1fd9wfXz1TjhEqmt9SVa0CnYhCKDgdLNSvg5Nl0y67pCIuK+If3AQo+ev7xApaXPGJLmuM1oMJCfEQdAYbkHJ6w9sfI5sLapdiADpvpmD0EQ9MPtiLikpgt+xFEnHiTp6ZpiuqSl68+4C9W4+zvd1NO1IEleehyD01QQpbS2uW+tZ6v3wd5laj7uYm+ZKHRFut0RL5MWZl6nWNPQmCiHSV2hibU1V6tSlAAiqB3xjIN9V+4sqmxkX2UjEUYDR+eldbovN0W9se+v9kFEvKUOVr+q5jN+4/31BUHQHy2yXetqRNz+OElNF/yBo048yCLi4ojrT2oeDD1FzVe9pIsJ+6tVW8j+yTEkxUQSHWnEaoNDdS3uL6ZF9gcfB8m5XrRSOAKtrKRsh8elpcJhiFBbz5gTICZVzQOsl3hQO+IJtTuJrdvTp+cuLygHYEJuMvHRnVPdBiTHALC/ysUewO6w4R1orYO0Yc4PM0EQQgstsl3jYlsdR424pKYLfkCLiB9cB20+KsHyFpZ2KNmg5qKYHhgcbRc0+/kNaKz0+/YHqtRrtn9KDAaDgZwkdc1WXNOH1/LWT9SoRfoF35GaB8ZI1aqzZr/e1oQWHVuXCV3jSE8v1NWMwwlqRxwgc/9Xbj+n3WLlx93qw6NjWrpGvxTtTb3ZM+MOx2aD1a+o+dRrwRj0v35BELpCi6zUHgCrpffHS2q64E9SBkN8liqR0qLNgUr5dmhrhKh4SBuqtzUCwJCTIWucCiqseMqvWze2tlPb3A5ATqK6VstOVC0fS2vdjIjXHLC//g0w4kxvmil0hSkS0oaouSine4+2ZqcAniimd09qvhp1KqnpDp97go888ggGg4Hbb7/dcVtzczO33HILaWlpxMfHc8EFF1BaWtqn9fviiK/fX0N9SztJMZGM6Zd05JrxZgAaWy00tLT3ya4uObAGSjeqXooTLvPeuoIgBBYJOWCMUOIpvdWJt9SruiWQ1HTBPxgMwVMn7hBqmyiH14GC0Qgn3q3mK1+A+jK/bV1mTz9PiI4gJsoEQHp8FAAV9W464ts/V2PuURCf6TUbhR5wCLaJI+41Sjc5hdqSpLyiW1Lth0CVYeSIr1q1ihdeeIHx48d3uv2OO+7gk08+4d1332XJkiUcPHiQ888/3+31bRhJrNpMTL17+f5aWvr0/DRMxiNFDcyRJhLt6erl7r6x98Tq/6px7PkQm+q9dQVBCCyMJqdT3Vt6ulavFJ2kvgTBH2h14sHiiPeX+vCAYsSZqma/rRGWPu63bTVHPDPB7Lgt3R48Ka9vdW8xzRGXaLj/EME27+N4j5wsQm09oWVUVXjWccvb+MwRr6+v54orruDFF18kJSXFcXtNTQ0vv/wy//znPznppJOYMmUKr7zyCitWrODHH927IKhKnwJA1j7X+1lW1Lew8YBSzJs5NL3bx2XY3+TLvOWIN1XDpvfVfOovvbOmIAiBi3YyXe2iI671ueyF+uZ21u6roqnVhZR3QeiOwTPVuHc5tLvpwPgTUUwPTAwGOOkvar7qJb/VXR5yOOLRjtvS+hIRb66BPUvVfORZXrNP6AUtIl4mLcy8hrxHukZamEXEb7nlFs466yxmz57d6fY1a9bQ1tbW6faRI0cycOBAfvjhhy7Xamlpoba2ttMXQOlA9eaZU/ihywqMS3aWYbPByOwEspOiu32cdsJa1hcVzq7Y/AG0N0PmaBgwzTtrCoIQuGiOeE0vGTvV9r6WKb074u0WK49/s51nFhfw0Bdb+9auRxBA1fjGZUBrfeCqp7e3qrRLkIvMQGTISZA3S2kNfPeQX7asaFCHRprzDc7rtYqGVmyuqnHvXqLsThsK6cO8bqfQDRkdIuKinO4dDmqOuIhZ9ohWI15XDK0+ak/dB3ziiL/99tv8/PPPPPzww0fcV1JSQlRUFMnJyZ1uz8rKoqSk61rKhx9+mKSkJMdXbq66wD2UcyLtphji6gtJqljXq13NbRa+36HS0k8YkdHjY7WIuNupTt2xfr4aJ1wqqSOCEA4kuxgRr7I74i5ExNcVVVNkVwwurmnmh4IKTywUwhmjEfJPVPOCvrcC9SmHtoClFaKTISVPb2uEwzEYYPZ9ar7hHSjZ6PMtqxrVNVlKrNMRT4qJBKDdaqPR1Uyh3d+pccjJXrVP6IW0oWAwKl2UBv9pC4QsLfVO4Ts5rOyZ2FSIsWdoVwZOerrXHfGioiJ+85vfMG/ePKKju484u8Pdd99NTU2N46uoSF3Y/nbBbj5uVenpB75/ha+3lNDS3v2b8MKtpdS3tJOVYGZSbkq3jwPI8GZEvHIPFP0IGGDcRZ6vJwhC4OOIiPeWmu66I762qLrT9+v3V3f5OEFwiaF2J6Rgkb52dIcj0jNRDrADlf6TYcz5gA0W/tXn21XZI+KpcU5HPNJkJNYu3FbT1ObaQtrh05CTvGqf0AuRMc7POqkT95zi9YBNdVxJyNLbmsBHE2wLIOV0rzvia9as4dChQ0yePJmIiAgiIiJYsmQJTz31FBEREWRlZdHa2kp1dXWn55WWlpKdnd3lmmazmcTExE5fAM1tVt63HA/AiW3f8/Hq3fzxw00s21WO9bCUl0N1zXy5WUXcfzGxX5cibR1x1Ih7wxHf8I4a82eJKrIghAuOiLj3UtN3lNYBcOk0tfbWkjosVknvE/qI5oQUr/er8rXLHFijxv5T9LVD6JmT/qy6ROz6BvZ879OtKjVHvENEHJxRcZcc8crdqqbdGOnUShD8R8ZINUoLM885KPXhbhGAdeJed8RPPvlkNm7cyLp16xxfU6dO5YorrnDMIyMjWbTIeQK/fft29u3bx/Tp093a685ThnHFxZfTGJ1FkqGR82I2UNPUxqsrCnnki23sKVc1AHXNbTy/ZDfNbVaGZcYzbXDviuVazVFlQ+sRTr1b2Gyw4W01l5ZlghA+OFpl7Om5l3iVJtY2sMflapraqGpswwDMGJJOTKSJ1nYrB2uavGOvEH7EZ0L2ODUPxKi4JkLUf6q+dgg9kzYEplyr5t8+6LNtWtotNNhTz1PiIjvdpznita444lo0PPcoMMd71UbBBRx14uKIe4zjPVLqw13CEREPnNT0CG8vmJCQwNixYzvdFhcXR1pamuP26667jjvvvJPU1FQSExP59a9/zfTp0znmmGPc2isvPR5zVBSleeeTt/U57kr/AUvmuSxYf5Dd5Q08+PlW0uKiqG9pp6XdSrw5ghuOy8foQopbYkwEBsBis1Hf3E5iTGSvz+mS/avV6WtkLIw8u29rCIIQfCQNAJMZLC0q6q0JhXSkqQpaVBeH3hzxvRXqYDEnKZqYKBOD0mLZVlLH3vJGclNivW29EC4MP13V9m79RGmYBAotdXBoq5pLRDzwOf4uWPOqKsPbvxoGeP/wpKpROdnmCCMxkaZO9yVG2yPiza444lp9+IletU9wkQxpYeY1tNZlEhF3jXCIiLvCv/71L84++2wuuOACjj/+eLKzs/nggw/6vN6B/IuxYSC97AfOG9jEg+eOVT3CDQYqGlppabfSPzmG3502olNdUU9EGI3E23uJu1xz1BVaNHzUOXLyKgjhhNHkfNMv39X1Y7TbE3IgKq7H5Q5WNwMwwO50D0xV477KRs9tFcKXUb9Q466FAaUky8F1gE1pLUjtY+CTkO3UwPnhaZ9s0bE+3HBYQMXl1HSrFQqXqXm+OOK6oDni5dLCzCMaK6Fqj5qLI+4aWkAkgGrEvR4R74rFixd3+j46OppnnnmGZ555xivrN8f1pzznBDKKv6N/wVs0Tvwj183M49JpuRyobiIm0kT/lBiXIuEdSY6JpK65nZqmNnL7YpilDTbZDxjGX9KXFYQgY2txLR+uPUCbxcqJIzI5blj6ERcMQhiRNlQpP1fsAk498v5ye2pe+vBelyqpVY54VqIqm+mXFANAsaSmC56QPQ5SBqua2Z3fwJhzdTbIzoHVapSUy+Bh+s2w/k3Y8rHqBuGC7oU7VHahmK6RGKMuZ2ub2nte5NAWpdgdGQc5E7xqn+Ai2uddfanKCovpWTxZ6Ib99vfI1CHyO3QVLTjScAiaayE6UV970Cki7gv2D1Epdf0KP8TYri5Y48wRDM9KIDc11m0nHJwnrNV9jYgXfAdNlRCXqXptCiFNUWUjTy7aye7yBoqqmnj9x73MW7nPM40BIbhJG6rGip1d36/VyGkRgh4oqVHva9lJqhtFTrIai+23C0KfMBicUfGtC/S1pSMOoTapDw8assepax2bFX5+3evLd6WYruFyRHzvCjXmHgWmPpYcCp5hToDEAWpeJlHxPlO0Uo0D3SvrDWuikyA2Xc0DpIVZyDjiFdnH0xTbn8jWGrL2f+6VNR2OeGMfe4lvek+NY84Dk1+SDwQdeXfNftqtNsbkJDJnYj8MwOIdZbz10z5s4oyHJ+nD1FjRXWq6/SLEhYj4oTotIm53xO0OeXVTG02u9s4VhK4YPUeNO74KnPR0hwiR1IcHFVPtom3r3uxZpLIPaDXiybFHOtCuO+LL1Th4hldtE9wkw/6ZJ3XifUdzxHOP0teOYCPA6sRDxhHHaOLAEJX+nbvjdaVW7iFJsW60wzic1kbY+qmaS+/wkKektpktxbUYDHDV9EGcM74f183MwwB8t72Mj9cd1NtEQQ+0iHi5g2IsQwAAoE9JREFUZxHxNouV2maVcpkep1LTY6MiiLP3zq1o8EKbRSF86T9F1c611sPmj/S2BmqLofYAGIySPhxsjDgTYlKh7qBTndxL1NqF2JK6EM91yRG32ZwR8UHiiOuK1sJM6sT7hqXNmTWUKxFxt3Bcl3UTIPEzoeOIAwfyL8FiiiaxegspZSs9Xi85RqU/9ckR3/EFtDVA8iCfqIcKgcWavVUAjM5JdLS+OyY/jSuOVkrYn24s5rONxRIZDzcyRwEGqCs+sk9zW7Ozh3h6z4641js3KsJInNmpFpxmf62V1/cxa0cQQKWnT7pKzX2QUuw22gVm5mgROQ02IsxOTRwvv5a01mSaQnpHNEe8vqWddqu16wUqdqnaUJMZ+on2gK6IcrpnlG6CtkaVau1CRp3QgQB77YWUI95mTuHg4PMBGLj9vx6v53KqU1dsfF+N4y5UFzlCSLNhfzUAkwd2Fsw4YUQm50/qD8CHaw/w0rI9tLRJGnHYYE5wpqcXr+t8X/kOVUsZnaT6OfdAhd3RTjtMLTgtXh0Wao66IPSZiZeDwaTaT+nd31eE2oKbSVeqcfsXSozLS2hCbF1FxOPMquUsQENLN5+xWlr6gGkQGe01u4Q+kC69xD2i6Cc1DjgKjCHlyvmejFFqFEfcN+wbPhcbBjKKFxNb61naQZ8d8aYq2Pm1mo+90CMbhMCnpc1CYblqITWm35EKjGeOy+HSabkYDbByTyX3fbqFnaV1/jZT0IuciWrU+n1q7F+lxn6Tez2s0xzttMNEirTvy+slNV3wkIRsGH6amq9+RV9b9v2oxgFS+xiUZI+FzDFgbXOW6HkBrUe4ppDeEaPBQKy9VKehpRvldEda+rFes0noI1pUsqYIWur1tSUY0d4jc4/W145gxNE+bydYeumy4AdCzhFvShhMWb+TABi441WP1tIEQaob29xLKd76ifoAyhwDWaM9skEIfHaXN2Cx2UiNi3KkpR/O7FFZ3HXqCFJjoyira+HRr7bz+cZiP1sq6EK/iWo8uK7z7VrrkQHTel2iukk54smHte3RXm8VEhEXvMG069X482vQUK6PDW3NztR0cZiCl7HnqXHzB15ZrrnNQmu7SjnvKjUdVFQcVHp6l4gjHjjEpkJchppLnbj7aBFxEWpzn6Rc1b7Q2hYQyukh54gD7BvxSwByCj8isrmiz+toEfF2q40md9KJN76rxnEX9HlvIXgorFAqw/npcT0+bnhWAvf9YjQzhqRhAz5Ye4AvNokzHvJoEfHDU9P3a6llvTviWlbO4SmZWkS8QiLigjcYcpJ6vbY1wo/P6mPDwbVgaVVtP1Pz9bFB8JwxqkyQ3UuO1MfoA9p7oDnCSHSkqcvHxNsd8S4j4lV7VfTVGCHOS6Aggm19o2Y/1O5XpUTSVcJ9jMaAUu0PSUe8On0qNanjMVlbGbSj77XikSYj5gj1K6prdjF9oa4E9ixV87HiiIcD+ypVWvrA1NheHxsbFcG1M/K4YLKqG/9o7UH2VTT61D5BZ3ImqIu/2gNQVahua6x0tjRzQcyxu9rINImIC97EYIDjf6fmK/+jXqf+Zp89ajnwGNFXCWbShqhDHZsFtn7s8XKaYnp30XCAWLOWmt5F4ESLhvebBFE9H5oLfiI9cJyhoEJLS88eK2KWfSWA6sRD0hHHYGDP6JsBGLBrHpEtfb+YSIjuJdXpcDZ9ANhUbVvK4D7vKwQP+6uaANcccY3Tx2QzZWAKFpuNN1buFTX1UMYc74x6F3ynRk00KG2oStHrBS0adHhtZLpdrK2uuZ2WdhEBFLzAiDMhayy01sG3D/h//70/qFHSh4Ofsfao+KYPPV5KO4zsqj5cI76n1HTtPVdeV4GDFhEvk4i4W+xZosbBx+lrRzCj1Ykf2qqvHYSqIw6U55xIbcoYItobPVJQ7/GNvSvWv6XGcSLSFg5YrDYO1am04Jwk11VYDQYDlx89kEiTgT3lDew8JGIlIc2Qk9W4zS5ctO1zNQ471aWnayJFSYdFg2KjIoiOVG/jVQ196O4gCIdjNMIZf1fz1a8467X9gdUCRfbWowOn+29fwTeMsdeJ712uesN7gKN1WReK6RqO1PTWrhxx6R8ecARQenBQoWXd5h2vrx3BTKYWEddftT9kHXEVFb8FgNxd84hs6VsLDYcj7kpqevF6KNkApigYd1Gf9hOCi4qGFixWGxFGAymHKVr3RlJMJNPz0wD4enOpL8wTAoUx56px92Io3QJb7KmaI89y6enaRWhS7JEXockx6nWnCboJgscMnmnvBW2DBbdBW5N/9i3dBC21EBWvovJCcJM80K58b4OtCzxaqrvDyI7ERXVTI15XApUFgEFUpgMJLSJetUeJNAq9U12kfl8GkxxWeoIWEa/QXzk9dB1xoKzfydQljyKivYGBO/rWjiXendT0tf9T48izXEo3FYKf0loVDc9KjMbYh3rG2aOyANhwoNr1rAsh+EgfptLIrO3w3HRoa1AXIS5EZ5rbLLT0oBbsaLPYKBFxwYuc+jeITVfO8Zd/8M+eWunG4Jlg6j4FWQgitEPIzZ6lp7sSEY9ziLUdVqajpaVnj4OYZI/sELxIfBZEJ4HNaj8oEXql0B4N7zcJoo9slyu4SNJAdeBraVXOuI6EtCOOwcDuMbcCkLvzDaKa3Ffu1CLivYq1tTXDhnfUfNKVbu8jBCclNeoUNzvR9bT0jvRLjmFASgxWG6zfX+1Fy4SA45T7VbYMAAY47SGXxKh6Uwt2tFlsEkdc8CLxmXDBi4AB1rwKq/te4uUyBd+qcchJvt9L8A+j56hx348epadr12Cabk9XdFtKWKjVh0taekBhMEC6PTIp6emused7NUpaumcYjc6sq+IN+pqi6+5+oKzfbGpSxxHR3kD+5ifdfn6CPQLVa7Ry26fQXA2JAyD/xD5YKgQjpbXKEc9K7Lp/uCtMHpgCwNq91d4wSQhU+k+GuZ/DjN/AVR/C0JNdelp3rcs0HBFxccQFbzPkJDjhbjX/9E6Po5o90toI+35w7iuEBkkDvJKe7oojHmdXTT/iek2rDx8sjnjAoaUIi2Bb79hsHRxxEWrzmJzxaixer6sZIe+IYzCwY4K6kOi/5z3iq907dXO5Rvzn19U48XIwdt3jUgg9HI64G0JthzNpYDIAm4traLNYvWGWEKjkTlOR8SGuH9bVuuiIV0tquuALZv0epswFbPD+9bDhXd/ss3eFShNMylXdBITQwQvp6ZpznWDuPTW9sYNYW2RLJZTZlZEHimJ6wJEhEXGXKd2s2qBGxEh9uDfItjviJRIR9zk1GVMpHXAGBpuVYesfUadKLuJITW/p4SK3dLNqJ2AwSlp6mFFqV0zPSui7Iz4gOYaE6AjaLDYKyxu8ZZoQItT0UhuppaZLRFzwCQYDnPVPGHex0jj44HpY+YL393GkpZ8o/cNDDS+kp9fZxdrie4qIRx2Zmp5ctlpNMkZBXFqf9hZ8iKOFmTjivbLzazXmHQ+RMfraEgrkdHDEdWwhHBaOOMCu8b/FaowkrXQFmfu/cPl5LvUR/+EZNY76BaQM8sRMIYiwWm1UNyql6rR49xTTO2IwGBiemQAgbcyEI6i1Z+MkdnMBKqnpgs8xmuC8F+CoX6nvv/g9LLzPexcvNpvzIlPS0kMPD9PTLVYbja1KgC3B3HuNeJvFRqtd4DKlbJW6U9LSA5OsMWos3+m/7gzBys5v1DjsFH3tCBUyRoExEpproHqvbmaEjSPeFD+QwpHqImLEzw+43M6s19T0uhKnSNv0Wz22UwgeapvbsNrAaOi5pYorDMuKB2BHaZ03TBNCCO0QML6bC1BpXyb4Ba2/+Il/Vt8v+xd8+Cto98LrrmybUq41RcEQ17QThCDDg/T0hpZ2bIABZ/p5V0RHGjHZsym0981kzREfJGnpAUlCjurOYLOo1p5C1zRVQdFKNR9+mr62hAoRUZBpz8jQUbAtbBxxgD2jbqI+cSjmlgqGr/2bS6f58Y6aIwsWaxePX/4UWNvUaW/uNG+bLAQwlQ3qAjQ5Jgqj0bNUSi0ivqusHmtXrzMhbNF64nZ3Aaqlpje3WWlps3T5GEHwCgYDzPodzHlG9bHdMB/evAiaaz1bd4s9Spp/orTkCVU8SE+vs78HxkaZMPXwWWswGIiJUho9Ta0WIlprSai214eLYnpgYjBAzgQ1L9FXNCugKfhWHVZkjILkgXpbEzpka689ccT9gs0UxZZpD2E1mMjZ9wn99rzf63O0i18bzgtiB1V7YdWLan7C/3nZWiHQqbKLY6XEeRYNBxiQEoM5wkhzm5USuwCcIEDvjnh0pAlzhHorlxZmgl+YdCVc/g5ExsHuxfDKmSo7rC/YbLDlYzUfdY7XTBQCDA/S0+sdium9f9bG2h3xxtZ2ksrXYMAGqUMgIdttkwU/4VCv1lc0K6DZYS/dkbR076IdAh1cq5sJYeWIA9SmTWT32N8AMGLtX0mo6jkVxmQ0ON7YG1oPc8S/e1CpvObNknS6MKTKXh+eEtv3+nANo9HAgBQlvlFU2ejxekLo0FtqOkiduKADw2bDtZ9BXAaUboRXz4a6UvfXKV4PhzartPSRZ3nfTiFw6GN6uiaW29N7oIZ2vdbUZpH68GAhOzDaSAUsVgvsWqjmkpbuXQZMVeP+VWDVp2tR2DniAIUjb6Q8+zhMlhYmLr2e6PqiHh/vPGHtkPa5Z6lKywM45a+i8hqGaKnpKXGeO+IAA1NjAdgnjrjQgYYW9b6j9cjtCk1Usq63NouC4E36TYLrvobEAarG+7VzoP6Qe2usm6fGkWdDbKr3bRQCh9HnAgbVL75yj8tPq3ehh7hGTKTzei3l0I/qRklLD2y0qOShLWCRz7Aj2PcjNJZDdBLkHq23NaFF9jjVDq65Rn2G6UBYOuIYjGw85gnqkkZgbi5n8pK5xNTv6/bhsfaWGFqKaERrDXx8i7pzylx1MSKEHc6IuOep6QC54ogLXaBl4vQUDdJSNrUWP4LgN1LzYe4nkNAPyrfDa7+AhnLXnttS5zzQltafoU9Sf8g/Qc3Xv+Xy0+pcyArS0K7XaKwgsWqzmmt7CoFJSh5EJUB7M5Tv0NuawEPLIBl5Npi8c70p2DFFQv8paq6J4fmZ8HTEAUtUAmuPf4nGuFxiG4qYuugSksq7rhGI6xARN1haGffDHUrqPnkgnPKAP80WAoiqBuX0pPogIm7TsaehEDi0Way02NvwaD1yu0JrbVbXU5tFQfAVqfkw91OlgFy2FV4/Fxore3/emldVJCJ1iDhL4YJ24LLuLZdTQevciYjbr9dya1ZhwEZd0gipDw90jEbIHqvmkp7eGavFqakw5jx9bQlVco9Sozji/qc1JovVJ71NXfIozC0VTPnucvI3PoGpraHT42Ltp7DWpmomLL+ZtNJlEBkLl8wThdcwptKLNeIA/ZNjMBkMNLRaHEJwQnijZeEYDM4LzK5wRMSbxBEXdCJtCFzzCcRlqprxN86DpuruH99SDyueVvOZt6te5ULoM/IsMCdBzT4o/N6lp2ip6fFuOOJDatVFdUX2zD4aKvgVLbP0wBp97Qg09v0I9aUqLT1vlt7WhCYOR/wnXbYPa0ccoDUmg9UnzqN44C8w2izkb32WGZ+fxNANj5FctgpzYwnDDUVcZ/qc27ZfRXrJ91hM0XDJG06lRyHssNlsDmEsbznikSYjmYlmAA5WN3llTSG40YTa4qIiMPagQ6FFimolNV3Qk/RhcM0CiE2D4nUw70IV8e6KxQ9DfQkkD4Lxl/rVTEFHImNg3AVqvvq/Lj1FE2tLMLuqmm5jdONqACqzxBEPCgbY2//u18cZClg6pqVHeOdaUziMAXZHvHyHa5lcXibsHXEAS2Q8m4/5BxumP0Vj/CCiWqoYvO1Fpn53Bcd9ejwPl9zIXyL/R3J7OQ3xg1lzwhswdLbeZgs60tChr7wr6XKukpMUDUBxjbQwE1xTTAcRaxMCiMxRcPXHEJ2slGhfOgUqCjo/Ztvn8OOzan7W43KBGW5Mu0GNWz+B6u71eTTcEWuLjTQx1HCAVEs5FpOZ6vQpHpkq+AlNhKxkk8qWESQt3V/EpUHaUDXXIT1dHPEOHMo9nR9O/4IN05+kZODZNMdkYTWYaDbGsNI6kpeTf83KUxdQmzZBb1MFndFEsWKjTESavPdvlJOkWpgV10hEXHBNMR0gUUtNb5GIuBAAZI9TaeqagNsLx8N3D8Ge7+H7x+DduWCzKrFT6YsbfmSNVpoANiv89J9eH+7qgSSo1PSTjUrvpzp9GtaIaI9MFfxEUn/VfcFmgYM/621NYCBp6f5jsD1zZvcSv2/tvVBeiGAzRnAo9wwO5Z7huG3JjjLe+HEvEyOTuVXe1AWg1l6LqzlA3iJbIuJCBxpcvACNl4i4EGjkjIcbv1NO974fYMnf1ZfG6Dlw5uO6mSfozDE3w+7FsOZ1OP733ert2Gw2t8TaYqMiONmk+ocf6i+HPEFF7jTYvF/V6uYdr7c1+iNp6f4j/0QlHrp7sd+3loi4Czj7iMtFrqDQanG9mZYOkpoudMZRI96LI64dCNU3t2O1iuK+ECAkZMPcz+GCl2HoKSr9b+B0OO8FuOg1MEksIGwZegqkj4CWGvjhmW4f1tJupd3+nuZKRDzDVs4k4y6sGCjrLyWEQYWWnq6TaFZA0TEtffS5upoSFuQdDxhU14/aYr9uLY64C2iOuJYmKgjaCX1ijHcj4jmJyhGvb2mXntCCIyLemyOuXaDacDrvghAQGI0w7kK48j349Rr45Zcw4VLVCkAIX4xGOPGPav7D0932ntc+a6NMRsyRvSvrj6hUqaXrGEFrTIZ3bBX8w4AObaRcbG0XsnRMS5fWjr4nNhX6TVTzPf5NTxdH3AW0/r0SERc0au2K6YlejoibI02OvuQltRIVD3caW+014j20LgMwGQ2Ox0gvcUEQgoLRcyBnIrTWw5JHu3yIpnvhSusygLzybwH4wjLNKyYKfiR7nGoN3FwNh7bobY2+SFq6/9EOPAq+8+u24oi7QKxdKKmhVSLigkJLTfd2jThAZoJqYVZe1+r1tYXgorFNvefERvV+EZpgz86QTApBEIICgwFO+auar3oR9h/ZQ9rRQ9yFtHRzw0EyK1Xbsi/ap9JmCfOoarAREeUUzSpYpK8temK1qo4CIGnp/iT/RDUWfOvXjAxxxF1AuwhubbfSLm/sAlDro9R0gIx45YgfqpOIeLijZeHE9hIRB2d2hiYkKAiCEPDknwDjL1EK6h/fAu0tne7WSm0SXHDE+xV+gAEbKyyj2W/LcGQUCUHEkJPUWPCtvnboyf5VUF8C5kTIF7V0vzFwuvqdNxyCA6v9tq044i4Q26EuSaLiAjhT070t1gaQoUXE6yUiHu40tWoR8d4d8QRNsE1S0wVBCCZOexhi05VQ0pd3d7rL0bqst89aq4V+e94H4EODcuaa2uR6LegYcrIa9/4ArY362qIXmkjb8NMhwqyvLeFERBQMO1XNtYwEPyCOuAsYjQZiIkU5XXDiy9R0zRGXiLigRXRiXHHE7RGjWklNFwQhmIhLg3OfBQyw+mXVRsiOq6npWfu/JKbxAK1RySyLmA7I9VpQkj5M9RO3tMDe5Xpb439sNqcjPuocfW0JR0adrcZtn6q/hR8QR9xF4syaIy4nrEJH1XTfRcTL6lp6eaQQ6jS2ulEjLr3EBUEIVoafBif9Sc0/vRM2fwS4GBG32Ri87T8AFA27CmNULAAtbVJKGHQYDDDUnp6+KwzrxEs2QPU+iIiBodJ+z+8MnQ0mM1TuhkNb/bKlOOIuokXEmyXVKexpabfQ0q4+4BPMvqsRr21up0Veb2GLzWZzKzVdy86QiLggCEHJcXfBxCvAZoH3fgkb3nV0gegpIp6z9yMSqrfSHhHL/qFXEh2pLm0lNT1IGXqKGrd95reoZMCwxR4NHzYb7AdKgh8xJzjV07XMBB8jjriLaKmhTRIRD3u0fvImo8Hxge9N4swRDserrF6i4uFKa7sVi/0iJNaF/rlaRLxeIuKCIAQjBgP84t8w/lLljH9wPedXv44Ra7dibZHNlQxdr1qf7Rl1M23mFKIlcBLcDJ2t2pjV7IODP+ttjX/RapNHzdHXjnBmzHlq3PCOXw6CxBF3Ee2NvVHe2MOe+g4n9AaDwSd7ZEp6etijvdeYDAaiInp/q06QiLggCMGO0aTqxY/9NQBXtb7NW1F/o7+t+MiHtjczfsWtmFsqqE8cwr7hc4GOGYySmh6URMWqUgVw9tMOByr3QPl2MEbA8FP1tiZ8GXWOOgiqLIADR7ZU9DbiiLuIpKYLGlrEUdMN8AXp9vR0iYiHL40tTqE2Vw58pEZcEMKXplYLj3+9nUe/2hb8B7hGE5z6Nzj3eRqI5mjjNq5YfRGjVv2JpPI1RDUdIrVkOVO/u4yU8tW0R8az4dh/YzNFAc7AiaSmBzFjzlfjxvfBEiafabsWqjH3GIhO0teWcMYcDyPtom3r3/L5duKIu0ispKYLdupdqFnzFImIC+70EAfn67Gx1UK7VSJBghBOfLz+AFtL6thRWs+8n/bqbY5XsI6/lNNbHmGxZQJGWzv997zLtG8v4/hPZjL5+2tJrNpMqzmFdTNfoDFxqON5WsmYBE6CmOGnQWwa1B10Oqihzs6v1TjsFH3tEGDCJWrc9D60+7aVsDjiLiInrIJGQ4sWEfedI+5sYSaOeLiipaa744hrcXNNx0AQhNDHYrXx4+5Kx/ebDtRSEQLZVLXNbRTZMpnb9n/8OGseJbln0WpOBaAlOoOiIZez8pSPqM6Y1ul5ksEYAkSYYcJlat6hnV3I0tYMe5aquTji+pN/IiTkQFMVbPNtT3HfeRIhhvbGLhFxod4eqexOPMYbaI54eQhcTAl9w53WZQBGo4E4cwT1Le3USZ24IIQNhRUN1Le0ExdlIisxmt3lDWw8UMMlehvmIZUNKhIVHWmkPmsym7LsDrfVotLXu0ECJ77nh90VtFmszBiSjsnoG60cJl8DPzwNO76Esh2QMdw3+wQCe5dBexMk9IPM0XpbIxhN6vW35BFY9TKMvcB3W/ls5RDDoZoub+xhjz8i4mlxyhGvamjDFm7tOwQAt1qXaWi9drXyCUEQQp+CsnoAhmUmMH6Aqi3dVlKnp0leoapROeJHlIH14IQDHVTTpUTHF/y0p5KXl+3h9R/28uHaA77bKGM4jDgLsMHyJ3y3TyCg9UwfNlt1DxD0Z8o1YDDB3uVQusVn24gj7iISERc0/FEjnhwbiQFotVgdUQEhvHC3RhycWRoi2CYI4cPusgYA8jPiyE+PB2BvRaOeJnmFygaV2ePuZ63UiPuWr7eUOOaLtpU6Pqt8wnF3qnHDfKgu8t0+erPnezXmn6ivHYKTxH4w8kw1X/2yz7YRR9xFJCIuaNT7ISIeaTKSGKPaUR2sbvbZPkLgoqWmx7jjiItyuiCEHcU16jMiNzWWQWmxgOq4UdMY3CUqjoh4tHuftVIj7jsq6lsorGjEYIC4KBNtFhtbDtb6bsMBU2HwcWBth8WP+G4fPWmshNJNaj74OH1tEToz7Xo1rp8PLb7JMhJH3EVipOZIsKMJYfkyIg6QFqdasRyobvLpPkJg4m6NODh7iUuNuCCEB1arjdJa5YjnJEUTZ44g1f7ZsfNQcKenV9mzwRLMkW49T2rEfcfOQ6oMYnBaHDOHpgOwyZeOOMDJ96px3Tw4uNa3e+lB4TI1ZoyE+Ax9bRE6kzcL0oZBax2sneeTLcQRdxFJTRc0nBFx3/URBxwXUwfFEQ9LtItI7b3HFbTDIakRF4TwoKy+hXarjUiTwfGZkZ0YDcDu8gY9TfOYyu5qxHtBasR9h1YGMSQjjmFZCQDs8fXrLHcajLsYsMEXf4BQ080ptKulSzQ88DAY4Jj/p+Y/PuOTnvbiiLuIpKYLGg1+qBEHccTDneZW9x1xSU0XhPCizN7iMjMhGqNd5CkrUYl9+txB8jFaRFxS0wOHoiqlPZCXFsdgexnEwZom39aJA8y+DyJjoehHWP+Wb/fyN1pEfPBMfe0Qumbi5RCbDtX7YMtHXl9eHHEX0d7Y2yw22i1yyhquWKw2R8qw3xzxGnHEwxHt0E8THnKFBImIC0JYoYl5aqVM4IyI7ykLbkfcU7G2lnYrVmuIRU91RtMjyEmOITk2iqSYSGw22O5rlf6k/jDr/9T86z+ruupQoKEcDtkVucURD0wiY+CoG9V8xVNez8gQR9xFojtEpSQqHr50PPV1p3a3LzhrxEWsLRzRojnuiLXFS0RcEMIKLX07pYMjnqU54sEeEfcwNR2guV2u17xFXXMb9S3tGHBmXeQk2csg/HHoM/0W1WO7sQK+ucf3+/mDopVqzBgJcen62iJ0z7TrISIGitc7Fe69hDjiLmIyGjBHqF+XOOLhS0OHdGGT0be9HiU1PbzR6huj3UpNF7E2QQgntIh4aleOeEUDliCOCDtS0910xCNNRiLsn89SJ+49SuyigKlxUZgj1OdSlkOPoN73Bpgi4ewn1HztG7B3he/39DVFP6lxwDR97RB6Ji4NJl2p5iue8urS4oi7gaPuqFXe2MOVpj7U7fYV7cKqrK5Fat3CkL6ItWk14vUt7ZKSKQhhQFeOeFpcFBFGA63t1qA+yK3sY/syEOV0X1BZr/4e6fFmx20OYUB/lUEMPBomX6Pmn94J7a3+2ddX7F+txtyj9LVD6J3pt4DBCLsWQslGry0rjrgbRNtTRBvbJO0zXGnqQ2/nvhJvjiDKpP5FS2okPT2csNlsjsMXdyLiWuTIaoNaiYoLQsijRY1TY52OuNFoICNBOUt7Kxp1sctT2i1Wapr6ViMOzjpxOcT2HtrBSMdDn2x/pqZrzL5PiWeVbYUfnvbfvt7G0g4Hf1ZziYgHPql5MPYCNV/xb68tK464G8RKC7Owpy9Ryr5iMBhIjZf09HCkpd2KFs9257UWaTI6LkArGoI8UiAIQo/YbLYunaOO3wer2GdNU5tDE6kvrUKjRTnd63SVfZGtRxlEbCqc9qCaL3kUqgr9s6+3ObQF2hrBnAjpI/S2RnCFmXeqcfsXXltSHHE3iJHelGGPPyPiAGmxmmBbcF5MCX1Du3g0GiDS5J4WQYJZ1YlXiiMuCCFNfUs7bRYbBiA5NrLTfWlBrjGiCbXFRpmIMLp/qRojqelep6KXMogDVX58rY2/BPKOh/Ym+Px3wdlbfP8qNfafAn14jQs6kDUaRp4NeO/1Jn95N5Be4oJWlhDrJ0fcKdgmqenhRFOHtHSDwU1H3F5PKY64IIQ2mmOUGBNJpKnz5Vywi332tXWZRrQETrxOVReOuNFoINOuoF5Y4cf0dIMBzvonmKJg59ew7TP/7e0tNEdc0tKDi+N+69XlxBF3A+2NvWMLKyG88KdYGyCp6WGKJyUQ8eKIC0JYoDlGKYdFw8HZzqw4SPVFKvuomK4hNeLep6uIOEBanHLE/X6dkj4Mjr1Nzb/9G1iD7G8tjnhw0n8y5M3y2nLiiLuBFhGXE9bwpakPvZ09Idjr/IS+oXVmcEeoTSPBLI64IIQDdc0qKJAUc6QjrqWmB2tZU7UHiunQsZQwyJyzAKW5zUKjPRDRURgQdM6+OPbXEJ2shNs2feD//ftKYyVU7FLzAVP1tUVwn/P/47WlxBF3g1ipOQp7Gv0cEQ/2iymhb3gSEdd6iVfUiyMuCKGM1hlB+5/vSEfnyBaE9bOO1mV9jIib5XrNq2gHuzGRpiMCEdp1yn49rlNikpUzDrD4YaVEHgwcWKPGtKFKfE4ILqLivLaUOOJuEC2q6WGPXhHxA1XBeTEl9A1H67Io99+inTXiLV61SRCEwEKLiCd0ETVOsUctm9usVDUGXytDLe0+oY+OuIjrepeuFNM1dBcGPPomiE2DygLY8LY+NrjLwbVq7DdZXzsE3RFH3A1ErE3QDmH8JdamXUy1tAfnxZTQN7xRIy7tywQhtOnJEY80GUmP16l21ws4xNr6mJouNeLepcaefZHcRRlEqt6Ze+Z4mHG7mi9/EqxBcPhSvF6N/SbqaoagP+KIu0GMRMTDHn+npquLKRFsCzeaPUlNt0eQtPY/giCEJlpqemIXqekA/ZJVj+dgLG2q8jA1PVpS071KXZM69EnsSo/AfuBTUtPsv17ihzP1WjAnQfkOpaIe6BRvUGPOBH3tEHRHHHE3kL6Ugr9T0wFykmKA4FW/FdynY/syd3GopkuNuCCEND1FxAGyEpUjfqgu+MpUPFVNF7E271Ln0CM48u+RFBOJyWigzWKjTK/XmjkBplyj5j88rY8NrtJYCTX71Dx7nL62CLojjrgbaPWa8sYevjhS0yP7dnHQF3KS1MVUsSinhw1aXWPfIuJ2sbaGVtEVEIQQpq4HsTaALHt/50O1wXeI67WIuGQweoXaHg59TEYD2YkBkH1x9E1gjIDCpXDgZ/3s6A0tLT01H6KT9LVF0B1xxN1AIuLhjc1m0yUi3i9ZRcQPVgffxZTQN5o9iIhrF0ot7VZHKYUgCKGF1WajrsWeLtxdRDxBOUelQeiIaxHxuL464hH2wEl7ENQLBwF1LpZB6FpCl9Qfxl6g5oEcFdcccUlLFxBH3C06pjpJpCn8aLPYHPVP/qoRB4mIhyOeiLWZI4xEmgyA9BIXhFCloaUd7TKku6hxphYRD7LU9JZ2iyPtvquaZFeIltR0r9JTRBycZRC6H/pMv0WNWxZA/SF9bekOccSFDogj7gbaG7vVpqJNQnjR2Ko+iAwGMEf671/HGREXRzxc8KR9mcFg6JSeLghC6KE5qrFRJiJMXb9PZDqco+ByxCvs+hYRRkOfO5Ro12st0r7MK/QWEc8OFD2CnAnQfypY2+Dn1/W1pTvEERc6II64G5gjjBjsc+1DUAgfOkYpjQZDL4/2Hs6Ur+BLLxT6RpOH6vzx0ktcEEIaR8S4G8cInKnpwVYjrjniafFRff6s1dqXtVqs+il5hwg2m81lYcCSQBCVnXadGte8BtYAy4horlX9zgGyxREXxBF3C4PB4DhlrW8RRzzc8NQ56iuaanpprY6tQQS/oom19aVGHJwtzLRevIIghBY9qVhraGJtFQ2ttFmCJzJcXq8OENPizH1eo+N7Z0OrXK95QlObhXb7tUd3woBaGYTuqekAY86D6GSlTL5rod7WdKZkoxqTciEuTV9bhIBAHHE30U5Z6yUiHnboIdQGkJlgxmiAdqvNcYEihDaetC8DiYgHEiU1zRyqC4CLUyGk0ITa4ntwxFNio4gwqoiybm2l+oD2OZee0HdHPMJowGSPpjdI4MQjtPrw6EgjURFduw3ZgVIjDhAZA5OuVPNVL+try+FIWrpwGOKIu4kWDa1rkUhTuKFXRDzCZHSkfUmdeHjQ7IFYGzijZFIjri8/7ankLws28aePNvHphoN6myOEEJpzGR/VvSNuNBrITAigSKWLlNtT09Pjo/q8hsFgcGi5iCPuGXVNPbfJg45ibS2BIWY89Zdq3Pk1VO3V15aOiCMuHIY44m6iRagaWgKs7kTwOVorqL6Kx3iCUzk9eC6mhL7RZrE60gCj+ygKqF0wVdaLI64XbRYr76wuwmYDmw3uW7BZFJwFr6Fdg/TW3isYBdscEfH4vkfEgQ6lhPJ/5wm1zT23yQOnI97UZnFka+hK2hDIPxGwwc+v6W2NE3HEhcMQR9xNnG/sEhEPN/RKTQfIEeX0sKGjsxYd4WmNuDjierG1uJbqpjbizREkRkdQXt/Kwq2lepslhAha3XOcuef3CC0iXhZE5REVDke87xFxcB5kSkTcMzRNJK0bR1fERJkcjnppoAQMpl6rxrX/A0sAXLO3NkL5djUXR1ywI464m2ipolIjHn7olZoO0E8i4mGDduBjjjBiNPZNMVhS0/Vn/f4aAKYNTmHmsHQAvthYoqdJQgihOZdxPaSmQ+eU4WBBS033RKwNnAeZIq7rGY7XWi+HPgH3WhtxJsRlQn0p7PhSb2ugdDPYrBCfBQnZelsjBAjiiLuJdsIaEKk3gl9p1DMibldOL66RiHio09yq1I09OfDRBJyqGsUR14udh+oAGNMviXH9kwD4YXcFVul8IHgBV1PTswJJzdpFvCHWBh1LCeV6zRPqHY54z6+1bHvAoCRQXmumSJh0hZqveVVXUwAoXqdGiYYLHRBH3E3kjT180TUiLr3EwwaHYroHBz5aCqHUiOtDc5uFYvv/al56HHnpccRGmahsaGVXWb3O1gmhgMup6fYo5aGgUk33XKwNJDXdWziEAXvTI0gIIOV0jclXq3HXIv1F27T68Ozx+tohBBTiiLuJpKaHL5qDFNtLKqAvkIh4+NDkoWI6OCPidS3ttLSLUJG/2VfZiA1IjY0iKSaSCKORsf1UVHyDPWVdEDzB1dT0YFNNt1ptjraLItYWGDS0upZ9kZ0UgK+11HzIPwGwwdo39LVFc8T7TdTVDCGwEEfcTaId7cvEEQ83Gu0RCH0i4soRP1TXQmu71e/7C/6j2dFDvO9vz7FRJkz2+vKqhgAQqQkzDlSpA7MBKTGO28ba09M3HRBHXPAMm83msnOUFWQR8arGVrTqjdQ4DyPiEZLB6A2chz6u1ogHkCMOMGWuGn9+Ayw6vRbaW+DQVjWX1HShA+KIu4lWHywR8fCjScf2ZWlxUUSZjNhsAfghJ3gVT3uIAxgNBlJi1UVsRUNwXICHEgftmSvaARrAuAGJAGwUR1zwkMZWCxa7t+qqc1TZ0BoUh7iawGRybCSRJs8uUbXDTBFr84wGF2vEnanpAfaZM+IsiE2H+hLY+ZU+NhzaAtY2/n979x0eR32tD/yd7ZJWvTdLlnvBFVewMc30FggESAKEEEjsJGCSeyENSHIvv1S4IRAIAdNCCTWUUIxNx8a9d1m2rN61q7J9fn/Mzqxkq2yTdmf2/TyPsZHWq7E1npnzPed7DpKygPTS2BwDxSUG4iFS9hy5eGFPNLEcX6bTCUojFHZO1zZlj3iElRfZ/mwSR5iNPvnfaKG/twMApWHb3jobPN74D4gofnX0SlUuBp0Ak2Hox7jMZCOMeqk6prkrzgKkAbTYo1OWDrCnT7QEX5oepxlxgyn2Tdv6zg8XwpuGQtrEQDxEFu4RT1ixbNYGAIVKIM594lrmcEfeNR0IlHUyEB99chlwfmogEB+bY0WySY9etxeVzd2xOjTSgHb/v+kUswHCMA/1giDEZxOtQbR0y6PLIitLB/oE4kychE0UxUDX9GGrL6TFkya7M/6mQ8y5Qfr50Bqg4/jof/267dLPLEunEzAQD1ES94gnJFEUY5oRBwJlruycrm3RaNYGAFlWBuKx4PH5lLFxfbs+63UCJhWkAgiMNiMKR6c/Iz5cYCTLkwMkNQTi9uiMLgMAs1KazmZt4eq3DWKYjHiu1QxBALw+ES3xtiUqexwwdili1rStb0acqA8G4iFiRjwx9bi8SgOZZGbEaQQ5olSanpXMQDwW2rvdEEWpbDgtydjvc+NyrQCAyiZmxCl8HT3+QHyYwEiWH697dwcgzxDPjUZpOpu1RazvNgjzMNsgDHqdsqWgKR7PtVg1bfO6gcY90q/ZMZ1OwEA8RMr4Ml7YE4rdv/CiEzDsnryRUsiMeEKIVuVFtj8b28JZ4qNKDiRyrGboTigblgPxIy2cJU7h6+j1l6YHOUpTLhlWQ2l6s7JHPBql6ZwjHqlQtkEAQIG/OWBDPPaymXwxkJwN2OuAw2tG7+s27we8TsCcDmSOHb2vS6rAQDxE8oW9b7kOaZ/dIa0KJxn1Qd2MRkIRM+IJweHvRWCJcMEn11/a2WyPwwciDWv1L3xkDxBIjMtNAQBUNjMQp/DJGfFkc7Cl6erJiDf4Fwvkbu+RsDBxErFQt0Eoiz7xeN8xmIFZ10m/Hs2mbUpZ+gw2aqOTMBAPUd9yUTYASRw2f0Y8VvvDAaAwXcqIs2u6tskZcXOEpelyOapa5gdrhbw3cqCuz+PyAqXpcdfMiFRDrtAKdpRmYJZ4/N875JJmuQN3JNg1PXKhboNQFn3i9Tllzo3Sz4c+ADprRudrcn84DYGBeIiMeh0MOmlFi/vEE0ffjHisFGUE5sHK+4hJe+Su6ZHOqw80aGIgPpoCpeknZ8THZCXDoBPQ6/YqmT+iUNn896PkIEvTC9LU0zU9qhlxg1yazvtluOTGk8EG4kpperyeaznjgfIlgOgDtj03Ol9TCcRnjc7XI1VhIB4GljslnkAGIrib0UhITzIqCwF1HSxP1yqlWZshwkDcnxFv7nJyG80oUkrTU07OiBv1OpRlJwNgeTqFz9YrB+KhlQvH5b7dPhxur1IKHY1AXK4qcnl9cHl8Eb9fIuoM8VwLBOJxvACsNG17BvCN8CKNzws07JJ+zYw4DYCBeBgsykgMBuKJQs5AxLI0XRAEJSvO8nTtkkvTLabILs85VpMySoad00dPa/fge8SBvp3TGYhTeELdKiWXC9scHvS64jc7LGfsLUYd0iyRL3rLz2oAy9PDJT/7BN0YMD3OS9MBqWlbUhZgqwUOfziyX6vlEODuAYwp0gg1ohMwEA9DEkeYJRw5Ix7L0nSg7yxxZsS1yOcT4fRnbiLNiBv0OiUrq4aSVC0QRVHJIGWcMLpMpuwTb+YIMwqPkhEP8n6UZjEo96543icuN5MrSLNEpSmqQddnKyED8bDYekPrRxD3pekAYLSMXtO22i3Sz4UzAF1snx8pPjEQDwNL0xOPPQ4y4kDfWeJxfJOjsPVtABnpHHEAyFM6p8dxmaCGtPe4lW0A6YMF4nJGnKXpFKZQ70eCIPQZYRa/1wI5eMuLQlm6TGnYxua6YQm1GlBustfZ647vXjZzbpB+PvgeYKsbua9Ts0n6uWTeyH0NUjUG4mFgRjzxKHvEY5wRD3ROZ0Zci+SmQnpBgFEfeUZIfviO5yyYlsh/z1azAQb9wLfXCv8IsyPMiFOYbGH0LMlTQaZSLmcuiGogzlnikQi1H0Hf6ou47kmQOxEoO23km7bVbJZ+ZiBOg4h6IH7//fdj3rx5SE1NRV5eHi6//HIcOHCg32scDgdWrFiB7OxsWK1WXHnllWhsbIz2oYwYZsQTjz0OxpcBgc7pdR1xfIOjsMnXFLNRF5XSTLlhWzxnwbRE7lA/WDYcACpypEC8weZAD7N0FIZQgyOgzwizeA7ElY7pJzc6DFfgeS2Os7NxLNRFH0EQlKx4PC/6ABj5pm3OLqBpj/RrBuI0iKgH4p988glWrFiBDRs2YM2aNXC73Vi+fDm6uwOr/3fccQfeeustvPzyy/jkk09QV1eHr33ta9E+lBHDZm2JR37wiXUgzoy4tsnXlGj1ImBGfHTJM9sH2x8OABnJJmQmS58/2tIzKsdF2uH0eJU+EqEE4gVp8d8voj6Ko8tkcq8NZsTDYw9r0Sf+zzUAwJRLAUsG0HkcqFwX/fev2yZl3NNLgbTC6L8/aULUZzG99957/f7/qaeeQl5eHrZs2YKlS5eis7MTTzzxBJ5//nmcddZZAIDVq1djypQp2LBhAxYuXBjtQ4q6JGbEE068lKYrXdOZEdck+WExGvvDASBXyYIxIz4a5AfP9OTBA3EAKM9JQXt1B462dmNqUdpoHBpphL3PlrhQGjrmp8V/dUxtu7TAXJKZHLX3ZOIkMoGZ9aEs+vgz4vFcmg4EmrZteERq2jbh3Oi+v7I//NTovi9pyojvEe/s7AQAZGVlAQC2bNkCt9uNc845R3nN5MmTMWbMGKxfv36kDycqLP4Lkp17xBNGPIwvAwIZcbvTozTsIe2Qryl9x+5EQm7W1shmbaNCboo3VGk6AIz1l6dXtXCfOIVGqc4y6qHTBb99RQ17xGuUQDwpau+pNGtjIB4yURT7dE0PPm+Xr5bSdCDQtO3Au4CtPrrvzUZtFIQRDcR9Ph9uv/12nHbaaZg+fToAoKGhASaTCRkZGf1em5+fj4aGhgHfx+l0wmaz9fsRS0m8sCeceBlflmI2KPNV2Tlde6KdEZezYM1qeCDSAHkLwFCl6UBgnzgbtlGoQp0hLiuI8z3iDrcXLV3SQlZpVDPifF4Ll9Pjg8sbzjYIufoiPs+1fvImA2MWAaI3uk3bfD7g+FfSrxmI0xBGNBBfsWIFdu/ejRdffDGi97n//vuRnp6u/CgtLY3SEYZHLgdjqVPiiJfxZQBniWtZtPeIK+PLupzw+cdq0chRmrUFUZoOAEdbGYhTaMJp1Aag3/gyUYy/a4GcDU81G5CWFL1dk4HSdDZrC5V8rgkCYDYEHy6opjRdNvcm6edNjwOeKFWPNe8DeloBYwpQOCs670maNGKB+MqVK/H222/jo48+QklJifLxgoICuFwudHR09Ht9Y2MjCgoKBnyvu+++G52dncqP48ePj9RhB8Vi8l/YWZqeEHw+UQmQQinPGinyLHF2TteerihnxHOs0sO32yuivccVlfekwTX6M+IsTaeREs6eXSBQHdPr9ipZ9XhS0y41LizOTIrKxAgZm7WFTznXjPqQvidyaXo89yPoZ9oVQGoR0NUI7HwpOu9Z9an0c9kiwGCKznuSJkU9EBdFEStXrsTrr7+OdevWYezYsf0+P3fuXBiNRqxdu1b52IEDB1BdXY1FixYN+J5msxlpaWn9fsSSnK2y88KeELpdHsjJxFiXpgNAYQY7p2tVIBCPzqXZZNAhO0V6CFDNQ5GKtXZJix1plmEy4tlSIN7W7UJnD3s9UPACjUNDWxS2GPVKt/54vHfUjECjNkAaBQkwEA9HZxj7w4H+pemqqMQymIBFP5B+/cVfpLLySMmB+Nilkb8XaVrUA/EVK1bgueeew/PPP4/U1FQ0NDSgoaEBvb3SRTY9PR0333wzVq1ahY8++ghbtmzBTTfdhEWLFqmiYzrQdy4lH6ASgfzgo9cJMOqjt1IfrmKlNJ0Zca2J9h5xACiUO+3H4cO3ljjcXvS4pPLXVMvQD64pZoNSKlzF8nQKQSSjNON5W9NINGoD+uwRdzEQD1W4TWrzUs3QCYDHJyr7/uPenBsAczrQegg4+G5k7+X1AEc/l37NQJyGEfVA/G9/+xs6OzuxbNkyFBYWKj9eeilQ7vHAAw/g4osvxpVXXomlS5eioKAAr732WrQPZcQEmn9wz1Ei6NuoLZolc+GSS9MZWGmPkhEPYSzRcOSFG/lBl0ZGhz+zrROCq5wJlKd3jehxkbZEMsFDDsRr43ARVy5NH7FAnM9rIQu3H4FBr1O2QtTG4aLPgCxpwLzvSL/+7M9AJH0UGnYAThtgSQcKZkTn+EizRqQ0faAfN954o/Iai8WChx9+GG1tbeju7sZrr7026P7weKTMEY/DfVYUffHUqA0IjDBj13Tt6QqzI/JQijOkUk/VPBCplLwHP8VsCGrBLhCI94zocZG2BMZJhX6NKI7jjLjcL2FMVnRL0y0GzhEPl9xLIJJzTVULwAu+DxiSgNrNwKEPwn+fIx9LP5cvAXTx8dxI8WvE54hrkbx/0+X1wenhKqvW2SO4GY2Eogy5WVtvXHa/pfDJ5ZOWEDrUDkfOMNWq6YFIhdq7pUDcag5uP6WWGrY53F787r39WPaHj3DxQ5/h/T0DjyKlyNnDbNYGBIKjeLsW+HyiMspvfJ41qu/N8WXhC2TEQ29SWyzfd+Jw0WdQqfnA/FukX6/7Tfh7xQ/4S9vHnRWd4yJNYyAehr5lo8yKa59SChgHjdoAoMBfmu70+NDORk+aIl9PLNHMiGfKmQlmXkeS/G8x+EBcCjjUXppuc7jxrSe+wt8+rsTR1h7srrXh1me3MBgfIbYwm7UB8btHvK6zF71uL4x6IfoZcQbiYYukH4FqF4BPux0wpQINu4B9b4b+++0NQM1m6deTLozqoZE2MRAPg04nIMXEfUeJwjYC5cKRMBv0yLFKnbDj7YGKIjOSe8RVlZlQIbk0PfhAXAo4jrb0qLayxesTseKfW7HpaDtSLQb85drZ+PpcaVzpz1/fpWRvKXoia9YWqKaKJ4ebpMWo8uwUGPTRfSwNzBFnIB6qcEflASreEpWSHeig/tH/YFd1Cx75+DBe21oDhzuI5/0D7wIQgeJTgbTCET1U0gYG4mFK8T9s2dk5XfPscZYRBwL7xOPtgYoiIz8sRvNcK/WPA2rpcgX3IEFhkUvTU4IMxEuzkqETpO95s1o6C5/gjx8cwGeHWpBk1OOFWxbi0plF+J8rTsHYnBS0dLnwwsbqWB+i5kQWHEn3jQabAx5vFEY0RUnlCJWlA327pntVu+AVK0o/gjDuR8VqzYgDwKIVEJOygJaDeO2xe/H79w5g1b924OrH1iv//ga1+1Xp58kXjfxxkiYwEA+T1T+ehqXp2hdve8SB+G66Q+GTK2zMUZojDgBpSQYlS6uqxjkqE2pputmgV2YmH1Vhw7Z3d9Xjbx9XAgB+d9UMTC9OByDNrr91aQUA4Pmvqhn8RJk9ggqtHKsZRr0AnygF4+ESRRH76m144vMq/Obtvbj/P/vw/FfVON4W3nksZ8RHJBD3Vxd5fSKcnvhZfFCDwKJPGHvE+1Riqe0aIJrT8Eb2zQCAOwyv4oqJRmQkG7GzphP3/nvP4L+xrQo4+hkAAZhx9egcLKkeA/EwpfoftljupH3xmBGX918dZ2ClGT6fOCIZcUEQ+pwv6gv41KIjxNJ0AChX6QizffU2/OTlHQCAW5aMxaUzi/p9/pKZRTAbdDja2oMDjfZYHKJmhTtSCpC21cmLP9VhBs37G2y45u8bcMH/fYbfvL0XT3xehcc+PYKfvb4LS37/EW5avRGHQvyeV/oD8XG50Q/E+y5q8nktNJFsg5AD8S6nR8msq8WTXxzFnYdnYpevHGlCDx5IewlP3jgPggC8tq0Wu2s7B/6NO16Qfq5YBqSXjNrxkroxEA+TkhHnhV3zIslAjJRSf0MbNuDSjp4+ZeOWKC/6KB26m4Pv0O3x+ljKHoK2MALxCv/35UgI35dYq+voxY2rN6Lb5cWiimz89/mTT3pNitmAJRNyAAAf7Gkc7UPULI/Xh26X9G8ynGZtAFCWLd07jrWGfu9Ys7cRVzz8JTZWtcGk1+GsyXn43tIK3HRaORaMzYJOAD460IyLH/ocr26pCeo9vT4Ru+ukwGZqUVrIxzQcnSAoixZs2BaaSMaXJZkCvWzCWfSxO9x48vMq/PTlHbj3zT14e2fdqNyPPtrfhP95Zy980KFywW8BQQ/sfgVzbB/hkhnSguM/vxpgy42rG9j4uPTr2d8c8eMk7QjvSk5IMTEQTxRKBiLMB5+RUJKpwhmdNCR5m4tOAIz64edQh0LONFU2B5d5fWdnPX72+i50Oz24+fSxuOuCyUHNxk5kSmm6JfjrxIR86fsSq6yxw+1FZXMXmu1O6HUCslPMGJ9nhWmQ8XlHW7px01Ob0GhzYkKeFY9+c+6gzbWWTy3Ah/ua8P6eBvzo7Akj+cdIGPY+W+EspvDyKOXZKQCacbQ1tMWfzUfbsOKfW+Hy+rBkQg5+d+UMpQu77GhLN3715h58erAZd768Aw6PF9cvKBvyfQ822tHj8sJqNoxIRhyQFoZ6XF4+r4UokuoLAEqviKrWbpxSkh7079tyrA23PrsFLV0u5WNPfXkU6UlGfH1uCW5YXK4kI6JpT10nfvjCNvhE4BvzSnHZhacASXcCn/4eePsO3HD+G3hzB/D2jjrcc8nU/gvmW54CetuAzHJg6uVRPzbSrviJLFSGe8QTRzxnxMPdk0fxR+mYbtRHPegdlydlXoMJxLdVt+PHL26Dxyft63vs0yMoz0nBtfPHRPWYtEYuTU8xB3+dmJSfCgA42BB+IO7ziajt6IXN4UZuqhm5VvOQ509dRy/W7W/CR/ub8EVlCxzu/vtmTQYdphelYW5ZJuaWZaI8JwU9Li8+2t+EJz6vQo/Li+KMJDz1nflITzYO+nXOmpIHANhTZ0N7twuZKaaw/4wk6duvxKALNxCX+xIEH4h39rjxfX8QvnxqPh65fs6ACzDlOSl46sZ5+J//7MMTn1fhl2/sxpisZCyZkDvoe28/3gEAmFGSDr1uZBb7rGYDmu1OTrkJgSiKEe0RB6RAfNPR9pAqsfbUdeKGJzehy+nB2JwUXD6rGJ29bry7ux71nQ784/MqPPlFFZZNysOZk/MwpSAVGclGONw+9Li86HZ6YHd64PH6kJlsQnlOCsqzk4e9p1a1dOOGJzeiy+nBoops/Pqy6dLvOeO/gMNrgLptmPP5rZic/gvs75SqQy6Rt+TY6oGPfyf9+vRVgJ6h1Uhwerx47JMj+PxwC0oykvDdJRUjUkXTlyiKaO12oaa9FzXtPahp78Xxth5UN7RE7WvwbAkT94gnDiUQj6M94vL+K5vDg85eN9KTBn8gJnXo7hOIR1sgIz70A5Eoivj123vh8Ym4YHoBpham4U9rDuKBNQdx5ZySQTOlFOiaHkpp+sQCKRCv63SE/O/Y5xPxzPqj+PunR1DXGWi8lZFsxKT8VEwuSMWkgjTkp5nR3uPG7tpObDjSiv0nBP2ZyUYUpCfB5xPRYJOOY2t1B7ZWd+Dxz6pO+rrzy7Pw1+tnIy/VMuTx5VjNqMhNwZHmbmytbsfZU/KD/rPRwOTAKDWEqosTlfm3Q4RSmn7/u/vQbHeiIjcFD35j1pAjxnQ6Ab+4aApsvW68vKUGP3phG95cefqgGczt1R0AgFmlGUEfT6jkxTGWpgfP4fbB7ZUWY8PNiIfaA8Pp8WLVSzvQ5fRgYUUWVt84X0mA/PyiKfjkYBNWf3EUnx1qwbr9TVi3vymo981MNuKsyfm4aEYBTh+fe9J9bMuxdnz/OSkDP7UwDY99e27gNXoj8I3ngcfPhtByAE9Yf4dLsBKfHGyWAnGPE3jjNsDZCRTNAWZdH+TfDoXC6xNxyzNb8OnBZgDARgBv76zH/1wxHV8/tTQq73+w0Y5dtZ042tKNKv+PY6096B1gS4TPGb0kGAPxMMkZcTsz4pqnNGuLo4x4itmArBQT2rpdqG3vZSCuASPRqE1W4Q/Em+3OIQO+D/c1YVt1B5KMetx36TSkJxvxzIZjaLI7sWZvIy6awbmoA/F4fcp+ylAC8TSLEUXpFtR1OnCo0Y5Ty7OC+n1urw8rn9+K9/37r00GHdIsRrR1O9HR48ZXVW34qqptwN+rE4DZYzJx1uQ8nDkpD1MKU5VskSiKONbag63V7dha3Y5t1R1o6HTAbNBhcmEarphdjItnFAZdsXFqWSaONHdjyzEG4tEQCMTDv96PzZaCo6Ot3RBFcdjv5d46G17cdBwA8LsrZwSVHRUEAb+5fDoONNqxs6YTP35xG/5166IBA/it1e0ARjgQ51bCkMnnmk4AzGEuwFYogXhwGfF/fFaFA412ZKeY8Mj1c/s9c+l1As6anI+zJufjcJMd7+1uwPojrTje1ouOHhcsRj1SzNKEEKvZAL1OQFu3C4ebu9De48arW2vw6tYapJoNWDIxB7NKM6DX6bCpqg3v722AKAIT8614+jvzkXbiv6+0IuD6fwFPXYTirt14z3wXXth/BcQ9yyBs+ofUKd2QBFz2V2bDR8gz64/i04PNSDLqcdcFk/HpwWas3d+En76yE3qdgK/NCb05nsfrw4f7mvDmjlp8drAF9kGuD4IA5KdaUJKZhJLMJJRmJSPD4MF3H4zwD+XHMyZM8qxYrrBqXzyOLwOA0swktHW7cLy9Z8TLc2jkBUrTo591tpoNyE8zo9HmxJHmLswekzng6x7/7AgA4MbTypGXJmU8r5pbgr99XIm3d9YxEB9Eh38vpSAEHvqDNakgFXWdDuxvCC4QF0URd7+2C+/vaYTJoMPPLpiMb8wfA4tRD4fbi8NNXTjQYMeBRjv21dvQ3uNCRpIJ43JTMLc8C6ePz0HWIGXigiBIpZw5KWE92Jxoblkm/rW5BluOtUf8XhS4F0WSES/OTIJeJ8Dh9qHJ7kR+2tCVDX/64AAAqRP+vCAXigCpsufh6+bgwv/7DFurO/DXjw7j9nMm9ntNbUcvDjV1QScgpPcOlZXPayGTExBpScawt0qNzZEWgKtahl/06ex147FPpHGIv7h4yqDXKAAYn5eKlWelYuVZw/eecHl82Fbdjv/sqse7uxvQZHfiP7sa8J9dDf1ed8XsYvzm8umDL6QWnALcvAa+F65DXtth/Ni7Gnh5tfQ5QxJw3UtA/rRhj4dC5/R48aj/3PjZRVPwrYVl+NbCMvz67b146suj+OkrO2E1G7B8WkHQ7/nZoWb89u19/fqzpJj0mFGSgXF5KSjPTkFFrvRzcWYSzIb+z/82mw3fjc4fj4F4uFianhi8PlFZJYun0nQAKMlMxo6aTjZs0wi538RIlKYD0ozeRpsTBxrsAwbih5vs2FjVBr1OwA2LypWPX3RKIf72cSU+OdgMt9cH4xBlqYlK3h+eZjFCF+I+14kFqfjoQDP2N9iCev2bO+rwypYa6HUCHvvmXJw5OU/5nMWox/TidGWmd6zNLZPOsx01HTx3oiAQiIefETfqdSjNTMLR1h5UNnUNGYjvrbNh7f4m6ATgjnNCb7hXmpWM31w+Hbe/tB0PrTuMpRNzMafPtWfNHikYmjMmc0R7CKTweS1knb2RL/rIHfptDg/aul3ItpoHfe3qL6pgc3gwMd+Ky2YWh/01T2Qy6LCgIhsLKrJxzyXTsKOmA58ebEFlcxd8ooixOSk4f3oBphUFcc3MnQTdD77E0w/dg4q2zzAtw42sKWcAC24DssdF7Zipv9e31qLR5kRhugXX+MvQdToBv7p4KuwOD17dWoOVz2/D6pvm4bTxOUO+V2VzF/73nX1Y69/WkJ5kxDfmleLCUwoxrShtyG03I4WBeJg4viwx9P3+xlNpOgCUZPlnQ7NhmyZ0u0Y2EJ9RkoEvDrdiR00HvjFA4zV5JMvZk/NQkB54OJ9amIaMZCM6/PuMB8umJ7K2bil7lDlE87LBTPc/AO6sGWQ2bR8dPS7c++YeAMCPzprQLwiPRxU5VljNBnQ5Pahq6cZEf3M6Co+SpYwgOAKkKoyjrT3YW2/D4iEeXJ/+8igA4IJTCpXtLaG6fHYxPjrQhH9vr8PtL27Hf368BFazAaIo4tWttQCAC08Z2UqbQAUjm7UFSz7XUs3hL/pYjHoUZyShtqMXh5u6Bg3EXR4fntsg3X9WnjUh5MXMYOl0AmaPyYzsHmYwo+OUm/GtD5fg8uIiPHjh7OgdIA3oje3SdeLGxeX99vfrdAJ+d+Up6HK68f6eRtzyzGY88535A1aWdfS48H9rD+HZ9cfg8Ykw6AR8c2EZbj9nAjKSY9tIlMvTYbL6L07cI65t8s3IZNDFXTanJFOeJc6MuBaMdFNAeQ/mNn9zpL4cbq8y9/e6Bf2DdJ1OwHz/jW3DkYH3HSe6dn9GPJysnvx92VdvG3ZO7t8/PYL2Hjcm5afiB2fGfwZGpxMwyd+Qbl99cBl/Glw0MuIAMKVQ2sq0r37wbv1t3S7lAfimxeURfb1fXzYdxRlJqG7rwX+/uhMerw+fHmrBrtpOmA06XDarKKL3H45Vbtbm4vNasORzLS0pskWfKYXSv/+9Q/z7f39PA1q6nMhLNeOC6cGXF8fKjFL/4mnt8IunFJnWLic2+vudDLRgZ9Dr8JdrZ2PJhBz0uLy47vGv8PdPK5V7aVu3C39ZewjL/vgxVn9xFB6fiLMm5+G925fi3kunxTwIBxiIh417jhKDcjOKMAMxEgKzxJkR14LuEdwjDgCz/QHfgUa7ssAke3tnPWwOD0oyk7B0gFFDCyuyAQAbjrSOyLGpnVyanhnGTb0kMwk5VhPcXhF76gZ/WG3tcuIpf4byzuUT425hcDDyg/hQQR8FR57rHOn9KBCID36+vbipGk6PD9OL05QtBuFKTzLigWtmQa8T8M7Oelzz9w2446XtAIDrF5QNWbIcDcls1hayaDQGBKCUfO+uHfxce3b9MQDAtfPHqOK6NsO/9edIc7fy90Qj48N9jfCJwPTitEEnL5gNejz2rblYPjUfLq8P//uf/Zh53wdYfP9azP3tGvx5zUF09LgxMd+KZ74zH0/eOA/j88Kr8BkJ8X/Gxykr9xwlhEAgHn9dyUv7ZMRFUYzx0VCkukZwfBkA5KVZUJyRBFE8uQz62Q2BB6GBygIXVEgZ8S3H2uHz8Vw7kVyanhFGabogCEpWXJ6pPJDHPj2CHpcXpxSn49yp6ulAPrlACvqC3QNPg4tGszZA2m4CAIea7HB5fCd93uP1KcHRjYvHht2sq6/5Y7PwyPVzYNLrsOVYO9q6pVFRdy6fOPxvjhATJ6GL1rOP3K9iT93A2eP9DTZsPCr1Jrl2gC1T8SjbalZGyO5mVnxEfbRfGle2fOrQlRLJJgMe/eZc/O7KU1CckQSnx4e6TgdEETilOB1/uXY2/vOjJVg68eREQ6zFX5pPJZQ94ixN1zR7FOa2jhQ5I97llGaJx0OJDYVPCcQNI9eLYE5ZJmo7erHhSKvS1GRbdTt2HO+ASa/DNfMGnsc5KT8VZoMOXU4PjrX1YKx/LA1J5Ix4Vpj/BmeVZuDDfU3YeqwdN58+9qTPN9kdeGb9UQDAqnMnRiUwGi2BjDgD8UjZndHJUpZkJiHVbIDd6UFlc5eSIZd9sLcR9Z0OZKeYcHEUJyWcN60A792+BG/tqEd6kgFXzysNahxapDjlJnRy9UWkzz7Ti+VFny443N6TFpqf8y8CL5+a3683SbybUZKO2o5e7KzpxOJxQzcIo/CIoohNR6Wy9NPGZw/7ep1OwDXzxuDqU0tR1dINu8ODwgwL8lLj+7xiRjxMSkbc5WE2UsOiVZ41EixGPXJTpZI+7hNXv0DX9JG7LC/zrwav2duofOyJz6sASOOJcgYpETXopTnSgNRJmfqLZI84ACwaJz1kfHaoGR7vyRnKv31cCYfbh1mlGVg2Kf5W9IcyyZ8Rb7Q50dbtivHRqFu0MuKCIGCaP0DaPMBoOXkLxLX+sXjRVJFrxY/PmYAbTxs7KkE4AKT494izgjF4gT3ikT37FKRZkJVigtcnnrQYZ3O48Zq/Yd+3FpZF9HVGm5zp5/1w5FQ2d6O12wWzQYdTijOC/n2CIKAi14qZpRlxH4QDDMTDJt8IRRHocbETp1ZF68FnpMhZcXZOVz+5kdBIjsk7a3IejHoB+xvs2FXTiZ01HXh7Zz0A4KbTyof8vXI562AlhoksktJ0AJhVmonMZCNsDs9JM7cbOh1KR/s7l6srGw5Ii9ZyGWdlc1eMj0bdbFHcKnW6vyLms4PN/T6+r96mjDG8fqE6SoWHY2XX9JDZotShXxAEzCyRgtbNR/tf217ZXIMelxcT863KYqRaTPJPgDjYyN4XI0XOhs8qzejXLV1rtPsnG2Fmgw56/15KrrJqV7wH4qXsnK4ZXf6HRPMIBuKZKSZc5O88+rPXd+G/XtkJAPja7OJhZ09PLfJnxFlifJJIS9P1OgHLJkmjyNb555vK/m/tQbg8Pswrz1SCJ7WpyJW2MhxhIB4Re5TKhQFgib8p4/rKVrj7VGHIWyDOn1aAwvSkiL9OPGBpeuii2R9H3gb12eEW5WM+n6ica99eVK66BUZ5FOOR5u4Bq5gocnIgPn/syePItISBeJgEQVBWWTnCTLviuTQdYOd0Lenyn2sjmREHgDvOnQiLUYddtZ3Y32BHRrIR/3X+5GF/31SWpg9KLk2PpE/D2VOkQPztnfXw+hviHW6y46VNxwEA/33+ZNU9rMrG+WdQH2nujvGRqJstSuPLAKm0NjPZCLvTo4w0rGnvwatbpFLhGyIcWRZP2Fw3dNHaIw5AaZC1obJVeaZat78JR1t7kGox4IrZxRF/jdFWkpmEJKMeLq8Px1iROCJ2+ZvKzh6TEdsDGWEMxCPAi7v2xXPXdCAwS/w4M+KqJ5dNjuQecQAoy07BkzfMw5wxGVgyIQfPf3dhUE1yJvvnQTfZudf3RO090sNlZkr414lzpuQjI9mI2o5e/GdXPdxeH+781w74RODcqfk4tVy9WQE5I17JQDwi0Wwe2rcK4/VtNQCA//vwEFxeHxaPy9ZUFooZ8dBFa2Y9AEzIs2J8nhUurw/v7KyHx+vD797bDwC4bv4Y5fujJjqdoIzAOsTy9KjrdXmVrUzyCDytYiAegVR2Tte8aK4Kj4TSLGbEtWKkx5f1tXh8Dl77wWl49uYFSsn5cFL67PVliXGAzydGXJoOSN/3mxZLHdPveXMPvvPUJuyo6USaxYD7Lp0WlWONlYocf0a8hedNuFweH5z+UWPRWhj+hn9KwqtbanH/u/vw8hYpIL9z+aSovH+8kJu1dbu8HL8YJGWPeFLkzz6CICjn2iMfH8a9b+3BoaYuZCYb8YNl4yN+/1iZkC9d1w428roWbQca7fCJQI7VhLzUgZvIagUD8QikMCOuefG+R1zJiLdxlria+Xyi0qxtNALxcAUym3zwkNkdHsjP9pGOELz1jApML05DW7cLnx1qgV4n4I9fn4miDHXv1ZXPm+rWnn77kSl4cjYcCIxPjdT8sVk4a3IeXF4fHvvkCADghkVlmFuWGZX3jxfWPhnXHjcbtgUjmhlxAPjG/DEoSrfgeFsvntsgNZ+8+4IpSA+zwWU8kPeJH2ri/TDa5KawU4vSVbslK1gMxCPA0nTts8f5HvGiDAsEAeh1e9HKcmHV6nF7Ia+jjPQe8UjIe31ZYhzQ5s+Gp5j0EXd2tRj1+Od3F+JHZ43HdQvG4NXvL8byaQXROMyYKkizIMmoh8cncsJDmOT94VazQWkUGylBEPDANbNwycwilGYl4fvLxuFXl6i7+mIgSUY95L8ylqcPz+sTlefaSLumy6xmA564cR5mlqQjP82MX1w0BVf7s+RqVZEjLTAea+X9MNr2+HvRyL1ptCw+03wqYVVK093DvJLUKrBH3BCXY+rMBj2K0pNQ29GLY609g86BpvgmPxzqdQKM+vhd/R0nZ8SZAVBEOkP8ROlJRqzSWGmwTiegLDsZ+xvsONbWgwr/gg4FL5r7w/tKTzLioWtnR/U9440gCEgxGWB3etDl9CA/1gcU5/put4xmEmJKYRr+vfL0qL1frJX7A/Gqlm6Ioqj5zO1okmfOTwty65yaMSMegVRmxDVPCcST4jMjDgBjsqTydK7Kqpd8nqWY9HF9M1e6X7fwXJPJ+8MzIyxL1zr5OsWMeHjifZtUvGPDtuDJ+8MtRp2m5zdHSr6m2R0epWEnRU4URWWxXy7/1zL+C4tAYI94/GVKKTpGKgsRTWXZciDOB1y1kh8O43ULhGycv0tsdVsPnB5e9wCgrVu6RmSoeK/jaChlIB6ReN8mFe/khm1MnAwv3se2xguLUY9C/8SRo0yERE1Llws2hwc6IfB8q2UMxCMQ2CPOlTAt8nh96PaXo8fzDWmM/0JVzQdc1ZIDcflhMV7lpZqRYtLD6xNxvI0j84BARjwrSqXpWiVnj3idCo/NEd09u4lGfl7rYeJkWHaea0ELJEIYiEeL3Ay2NCs5rpvXRgsD8QhwfJm29V05j+uMeBYbhqid3RloxBTPBEEIZDY5Mg9Anz3iLE0fkjxqsZoLOGEJjNKM30XheKaUprv4vDYcnmvBK8+Wnr+OtvB+GC2H/WXp4xKklwgD8Qiwa7q2yavCFqMORn38/lMpY0Zc9QIZ8fgOxAHu9T0RS9ODI583NW09HLUYBu4RjwzHzQZPDb1x4kVZNhMh0SZnxOXmsFoXv9GFCihd03lh1yR5n1RanK8Ky6XpLV0unosq1eVUz0O2UmLMngQAWJoerJJMf2MjpwcdbGwUsmjPdU40VjZrC5pNBb1x4kW5//nrKO+HUSOPR2VGnIbFFVZtU0sGIs1iRKY/G8fgSJ3ka0iKKb7PNYA9CU4kl6ZnsDR9SBajHnmp0nhFbmsInRoah8azQLM27hEfDveIB08eYcZmbdEjd0yXm8NqHQPxCCjjy7hHXJPUtE9qjL88qrqNNwM1UlO2q5RNt/pp95emZ7I0fVhs2BY+lgtHhuPLgmdXSTVgPJC3Bnb0uJXqKApfr8uL2g6pjwgz4jQslqZrm1oy4kCgPIojzNRJTdmu0szAHnHu9WWztlAERpixYVuo7E45OIr/a0Q8spoYiAfL1queZ59YSzYZlEoflqdH7kiLlA3PTDYmzHYvBuIRkPcc2ZkR1yQ1rQqX+R9wjzHTpEpqWvQpyZS6X3e7vGhP8L2+oigq+50zE+ShIRKspggfg6PIcCth8JRFH1ZfBEXOirOBaeQSbX84wEA8InIg7vT44Pb6Ynw0FG1qCo7GsHOnqsnbINSw6GMx6lGQZgHAgKrb5YXLf+1nafrwSv2LOHxgDV2gaobnWTjYrC14XPQJTXGGdF2TS6opfNX+Z1h5730iYCAegb6jhnhx1x65c2i6ClaFy1iarmpqWvQBuNdX1t4tlaWbDDokGfUxPpr4N4Yz6MOmtmtEvAnsEWeztuGoqRowHsgTIWp4XYuY/Ewh3ysSAQPxCBj1OliM0l8hy9O1R14VVkN5llyaXtfRC5eH1Rlqo6ZmbUDfvb6J/eAhl6VnJZsgCEKMjyb+Ffsz4vUdDvh87C8QCrVdI+JNoGs6n9WGY+O5FhJ5u1ZNOzPikZID8dKspBgfyehhIB4hq1m6UPHirj2BOeLxn4HITTUjyaiHT2R5lBqpqVkbELhJJvq4vDZldBkfWINRkGaBXifA5fWhucsZ68NRDYc7sAVCDfejeKSUprv4rDYcJSOexHMtGHJGvJaBeMTkRp7MiFPQrP5VVpama09nr3oalgiCoFy4uE9cfdQ2moil6ZIOdkwPiUGvU/oLMHsUPHlRWBCAFBODo3BwfFnwAnvE1XE/irXiPhlxThIJn8vjQ32ndF8oZSBOwZJHmNl5cdccJSOuluAom8GRGvl8Irpc6tr/qWQAErz6Qt4jnihjVqIh8NDK61Sw5IU6q9kAnY5bIMJhZdf0oLD6InRFGdLiYq/bi7ZuzhIPV11HL3wiYDHqkGs1x/pwRg0D8QgpF3fuEdccZY+4SlaFlRFmCV4urDZ2pwfyIrp6AnEpmKrr6IU3gff6tvn3iLM0PXgl7DAcMqViRiX3ongkZ8Qdbh88nHIzKFZfhM5s0CM/TQocWekTPrmJZ2lmckL1XGEgHiHuEdeuQNd0ddyM2DldneT9eCaDDmaDOjpv56dZYNAJ8PhENNkdsT6cmGFpeujkjDj3UwZPbT0k4pHcrA2Qxg7SwFh9ER5WiUUu0KgtccrSAQbiEZNvjNx3pC2iKKpqtjMQmCVe3cY94moSyHap5yFbrxNQmMG9vu3+jHgmS9ODxpm7oWNGPHJmgx5GvRRY8nltcDzXwiNf17jlJnyJ2KgNYCAeMXmVlePLtKXL6YFccauWPeJlfRpocTSQeqh1LFFJBmenynvEM1maHrTAzF0G4sGSF4WZEY+MfI3l89rgeK6FhyPMInecGXEKB0vTtUmeo2ky6GAxqqNcuDgzCXqdAIfbhyY7RwOphVrLTpUHj7bEffBoZ2l6yPqWprPDcHACi3XqukbEG7nqSN52RidT2wSPeMERZpFTStMzE2eGOMBAPGLyjZHN2rRFbWXpAGDU65TunRxhph5qLQXknjigg6XpIStMD3QYlkv7aWiBxTp1XSPijRxcyvd3OpkyLYaLPiEpZkY8YnKzNnkCUKJgIB4hjsTQJiUQV0mjNlm5f5/4UQbiqqHWjDgfPKCMqmFpevAsRj3yUqUOw8weBcfGjHhUpLE0fVh2h/qSEPGgpM9YRlb6hM7mcCsL26WZDMQpBCkMxDXJptIsZUWOFIhXtSTuvl21UetDdkmCz4N2uL3odUvdlzNYmh4SzhIPDcuFoyOVpenDkse2qu1+FGtys7ZulxedrLgImbw/PDvFpMRViYKBeISYEdemTiUjrq4Hn3IlEO+K8ZFQsGwqLTsNzBJ3JGRzQHn1Xq8TWMYZInZOD41NpVUz8UZeWGdp+uCUjLjKnn1izWLUIzeVs8TDlaiN2gAG4hHjHnFtCuwRV9eDz1h/IH6UGXHVUGsjpoI0C/Q6AS6vD81didccsG9ZuiBw3m4ouK0hNNwjHh3yVjMbn9cGpdYKrXjAEWbhS9QZ4gAD8YgxI65NcgYiXWWrwkog3tqdkFlKNVLr+DKDXoeCNHmWeOI9eHT4O6azLD10HGEWGrlcWG0Lw/GGGfHhcdEnfBxhFr7ADPHE6pgOMBCPGPeIa5Py4KOyQLw4IwlGvQCnx4d6myPWh0NBUGuzNiCxHzzkjt9ZDMRDVsLS9JDIW6W46BMZpWs694gPinvEw8cFxvAFRpcxI04hUkrTnR52StQQm0o7hxr0OqW0p6qZndPVQK3jy4DEfvBoUzLi6vu+xVpglnjiVVKEQw7E1VahFW/k0nR2TR+csuiTxEWfUHHLTfiU0WUsTadQyaXpXp8Ih9sX46OhaOlU6fgyoE/ndI4wUwW19iMAEvvBo0PZI84H1lDJeyltDg+zk8Nwe31KxR0D8cikmlmaPpxA9QXPtVAl+iSRcPl8Imr8pencI04hSzbpIffpsTt5cdeKQHCkvpuRPEucGXF1UOsecSCxHzzk0vSMFPV932ItxWxQZq9zlvjQ+gaNalysiyeB0nRmxAfT0SstMHLRJ3SlmdxyE45GuwMurw96nYDCdEusD2fUMRCPkCAISla82+mN8dFQtMg3ajXejMbmBhq2UfzTwh7xRHzwaPeXpnOPeHgC5emJd+6EQs5QppoNMOj5yBYJpWs6M+IDcri9SmVnOjPiISvyV/rYHR7OEg+B3KitOCMpIa9xifcnHgGpZnnfEf/haYVNpXPEAWCsnBFvYSAe77w+Ed0uaQFPlYF4hlRGVtvem3A9MuRAnKXp4eEs8eB0qvheFG+UrukOd8Jdr4Ihn2t6naA811Lwkk0GZKdI94NErBILV2B0WeJ1TAcYiEeFfIPkCph2BJq1qe9mJGfEj7f1wO1l34J41tWnRFKNpekF6RboBMDpSbxZ4u3dbNYWCbnRHwPxoXVwz27UyM9qbi97+gykb1NAQd5zSSEpYaVPyI63JW6jNoCBeFQwENcWr08MdLJWYRYiP9UCi1EHj09MyCZaaiIv+FiMOpgM6rscmwyBWeKJ9uDR6g/Es63MiIdDzogzczQ0GzumR02KSQ+d3NOHFYwn6ejhuRapRG5gGi45EC9JwNFlAAPxqMjwX7TkixipW98spRqbtel0gtKw7SjL0+OafM1Q86iYRB1h1uYPxLNSzDE+EnXiHvHgMDiKHkEQOEt8CB09bNQWqUS9H0ZCLk0vy2YgTmFKZ0ZcU+SuoUlGvSqzlAAw1j/C7AgD8bgmn2tqLjtNxAyAw+1Fj39vf1aKehdRYimRG/2FguOkokvuxdHZy87pJ+I2iMgFel+w0idYyh5xZsQpXHIgzk6c2iBnIDJVfDOSA3FmxOObFrJdiTjCTM6GG/WCKvtIxAO50V9LlwsONyeODIbN2qKrb8M26k9+hs3guRa2kgRcmI5Er8uLJrvUX4Z7xClszIhri9wNOUPF3ZDLc9g5XQ20kO1KxMymHIhnJpvY1ChMaUkGZfQnH1oHp4XtK/FECcT5vHYSLSwMxxpL00MjL+Cnmg2qfg6KBAPxKJDnLTIQ1wYlI56i3otCBQNxVVACcRU/ZBdnJN6DR6uyP1y937dYEwSBI8yC0MlmbVGlzBJ3sDT9RPJWqXQVJyFiTd6q1dnrZkPAIBxvl0eXJSfsojYD8ShIZ7M2TVEy4ioOjuTS9LrOXvS6WPYZr5TmOCpeCe5bmp4os3nbuqVSOnZMjwxH/Qyvs5cNtKJJzogzSDpZoPqC51q4rH0yu1xgHF51a2KPLgMYiEcFS9O1pb1H/eXC2VYzslJMEEWgsrkr1odDg9BCKWBhhgWCADjcPqVkW+tau9gxPRqKE7C/QKi0sH0lnihd09ms7SSsvogOZXG6jYH4cKr9f0djErRjOsBAPCoYiGuLnKXMVHl51vhcKwDgcBMD8XilhS61ZoMe+anSLPFEKU+XFxyyWZoeEZamD4/BUXSxWdvguOgTHbyuBU/pmM6MOEWCXdO1pUMDGXEAGJ8vBeKHmuwxPhIajBb2iAOJN8KsjXvEo4KzxIenhaqZeCKPL+Pz2sm08uwTa4GGbaz0Gc7xNpamMxCPAvkGaXd64PH6Ynw0FCktdE0HgAl5zIjHu06NPGQn2ggzpWs6A/GIyA+szBwNzOH2wumRninU3Eciniil6WzWdhKlZ4nKF4ZjTc6IJ8rCdLhEUVQy4gzEKSJ953vy4q5+WpgjDgDj8+SMOAPxeCV3qVV7BiLRRpixND065AfWBpsDLg8XsU8kZ211AmA1cV59NMiNyDp7EqOfRbC8PhF2p/T8qvaF4VhLtPthuFq6XOh1eyEIgXtBImIgHgVGvU6Zh8p94uqnnYx4KgDgWGsPH3LjlFbKThNtdipL06Mjx2qC2aCDKAINnY5YH07c6eizP1ynS8zRPtEmjyVtYyDej93hhjz0Qu33o1hLtPthuORseFF6EkyGxA1HE/dPHmVs2KYdWsmI56eZkWo2wOsTcbSV88TjTd+yU7VnxAOleIlRmt7KjHhUCIIQ6C/QkRjnTijYqC365CasHd18VutLfu5JMekTOiiKBvma1tbtQo+LVbKDOa40akvcbDjAQDxq0pRZ4lxlVTO314cuf3mW2rumC4KAcXJ5eiPL0+ON/JCt1wlKRY1a9Z0HrfVZ4m6vT/neMSMeOaXDMLNHJ9FKxUw8ke/rdqeHlWJ9BCZ48JoWqfQkI9L8TQHlrC+dTAnEMxN3fzjAQDxqsvzlTu0MxFVNfvARhP57/9WKDdviV7vSGMcIQVB32WmRP5jqdnmVf0NaJX/fBIEPrdFQkmAd90MhL/ho4V4UL9KSjJCr/OUeHcRzLdrKc1IAAEdbGIgPho3aJAzEoyQrxQwAaGO5k6rJFQ1pFiP0GtiTN4EjzOJWW5d29hlbjHrkpkrXQK0HVErH9GSTJq4RscaZu4Nr63YC0MY1Il7odYJSYaD1RcNQyM8+GQzEo6I82x+Ic1vgoI5xhjgABuJRk+Xf4ynfOEmdWvzBUbZVGw8+45kRj1utGmv4lSgjzLS0gBIPlBFmGl/ACYfWrhHxQh47KC+qEdCujGRkIB4N5dnSde0YA/FBHWmW/m7G+qsHEhUD8ShhRlwbWv0LKTn+76fayZ3Tj7R0c8Z9nNHaCKxEmQktd1tmcBQdbNY2OHnRJ8eqjftRvFAatnEroSLQgJLnWjTIpelVLQzEB2JzuNHSJT1vV+QyEKcokPeIMyOubi126funlYx4cUYSkox6uDw+HG3lg248ae3S1rkmZ8S13pxGvkbkaOT7FmtyaXp9hwNen7Yb/YWKY/JGhhyIM3ESwOqL6JID8WN87hqQnA3PSzUj1ZLYVRgMxKNEzoi388KuavLNSCsZCJ1OwORCKSu+t94W46OhvgIPPto418YmSAagyR+I56VaYnwk2pCfZoFBJ8DjE9Fk5yzxvhgcjQx5NCmb6wbIC8NcYIwOeY94facDvS5vjI8m/hxplrZLJno2HGAgHjXyvppWZsRVTWt7xAFgamEaAGBvHQPxeKK10vRxuVI/gkqN9yOQA3G5OR1FRq8TlK771cwe9aO1a0S8kPeIszQ9oE1jC8OxlpnMEWZDqVQCcWuMjyT2GIhHibyvpp1dOFWtRVkV1s7NaFpROgBgT11njI+E+mrV2KLPOP/Kdl2nA91OT4yPZuQEMuLauUbEmlxNcUTj1RShYmn6yGBp+sm0dj+KNUEQEqZKLBxyafo4BuIMxKNFvlG297i4z03FtFieNbUokBEXRZ6b8aJVY6OJMpJNyr8bLT94NNmk8um8NJamR4tcniiXKxLg9HjR5V/QYgOt6JJL05kRDwhsy9PG/SgelHGE2aDkQJyl6QzEoybDf2EXRV7c1axFg11qJxekQidIN1o5m0ex16bBLrVymVmlhgOqZmbEo04+b+SHMwpcHww6AWlJhhgfjbYo48v4rAYAcHl86OyVqgNYmh49gYZtvK715fWJqPL/nYzLYUacgXiUGPU6pCexAYjaBTpZa+dmZDHqlfIflqfHB4/Xp2xj0VIpoNb3ibu9PiVzxEA8esaxNP0kcqlwZooJgiDE+Gi0Rd5zL/8dJzr5mVUnABlJid3BOprG5kgjPSu5wNhPbXsvXB4fTAadMr4ykTEQj6IsXtxVrdflRbe/u6WWgiMAmFbEhm3xRA7CBSGwX1EL5H3iWn3wkHtIGHSCpr5vsSZnxKvbeuDy+GJ8NPGBjdpGjtxosdnu5HYtBJ5Zs1LM0Om46BMtE/KkiTWHGu08z/qobJEW6sdmp0DP842BeDTJgbh8AyV1kR+yTQYdUs3aKgWU94nvYSAeF+RrRGaySVM3onF52i5Nb7IFOqbzgTV68tPMSDHp4fWJqG7T5iJOqNiobeTIgXivO7D4nsjkfiVc9Imu8XlWCIK08N7CBJ3iUKMdADAuj/vDAQbiUSU3uZADOlIXpVmJBksBZ5RkAAC2H++I6XGQRL5GaO0he7y817elW5NNK9kxfWQIgqBkxQ81anMRJ1RavUbEg2STAVb/YrvcfDGRKdUXGqsEjDWLUa/MEz/oDz4pUJkpj9ZNdAzEoyjf30W30cZAXI0a/TdkLc4HnlGSDr1OQH2nA3UdvbE+nITX0Cmda/lp2jrXijKSYDbo4PL4UNOuvdmpTXb5GsGO6dE2uUAq49zfwAdWAGjukhd9eK6NhL7l6YmupYvVFyNlYr60wHiA1zXFvnrp70Ku1Ex0DMSjKBCIc4VVjeTgqDBde80jkk0GZfVxa3V7jI+GGmxyIK6th2y9TsAE/4PHvnrtbYPQ6gJKPJjsvz5p8bwJRyPPtRGlBOKsYAyMZOSiT9RNypcWGJkRlzjcXhz2b12bwow4AAbiUSVf2Bu5wqpK9f4Hn4J0bd6M5ozJAABsOcZAPNbkxboCjQXiADC9KB0AsLtWewFVbbtUTcJOr9E3pZAZ8b7kyjqt3o9iTX5ea2IFo7IwXJDORZ9om8hKn34ONXbB6xORmWzU5PNPOBiIR5Gc3eKeI3Wq75QesosytHlxmFOWCYCBeDxo0PCiz7RifyCuwVF5Nf5tHcUZDMSjbUqBlB2pbuuB3eGO8dHEXiOzlCMq18qMuCxQ6cNzLdqm+Rem99Xb4PZyIoRc8TS1KE1zvZjCpa3W0DEml5A1hZERP9Rox782H0eX04OFFdm4eEaRpropjwaP14fqth54fSLG5VpD7mocyIhr8yF7YUU2AGBXbSc6elzI4PilsFW1dGNjVSuSTAYsm5SLNEtos1cbNVqaDgDT/fu+dtd2QhTFuLvZur0+GHRCWMclZ8RLmBGPuswUEwrSLGiwOXCw0Y65ZVmxPqSwebw+vLOrHpuPtiMj2Yivzy3FmOzkkN4jcI1glnIkRLJHfPPRNry3uwHJJj2WTMzFvPLYnas+n4hPDzXjk4PNSDbpccXsEoz3T68IlpYrtGKtPDsZaRYDbA4PDjTYMd2/UJ2oth2XEkFy5RwxEI+qfP/KdVu3C06PF2aDPqjf9+aOOtz5r+1we6Uuwy9sPI5HPqrEX6+bjQn+/SU0OFEU8eKm4/i/Dw8pJVYT8qx44JpZIV30AnvEtXkzyk+zYFJ+Kg402vHF4VZcNKMw1oekOnaHG798Yzf+vaMO8ljQzGQjHrp2Dk6fkBP0+8jnqRbPtSmFadDrBLR0udBoc8ZN1v/9PQ14+KPD2FnTifQkI65bMAa3nzMh6Ou0x+tTvm/FGaEFVRScqUVpaLA5sLOmU7WBeGVzF37w3FYc6LMn9PHPjuCR6+fgrMn5Qb1Hl9OjjNXS4mJdPMgLIxAXRRF/WXsYD3x4UPnYX9YdxrlT8/GHq2aM+uJ2e7cLK1/Yii8Otyofe/zTKvzh6zNw2azioN5DFEUlCaHF/jixJggCZpZm4LNDLdhR05HwgbhckTnXX6FJMS5Nf/jhh1FeXg6LxYIFCxZg48aNsTyciGUkG2HSS3+lwV7c99bZ8JOXd8DtFbFsUi5uO2McMpKNONBox2UPf4EP9jSM5CGrXrfTgx++sA13v7YLDTYHLEYdLEYdDjV14Rt/3xB0p0pRFAPlwhp+8JGDxc8ONcf4SNSnsrkLlz/8Bd7YLgXhCyuyMDYnBe09btz89Cbsrg2uFNvj9SnXBy2eaxajHhP8GZltcdAY0OH24pdv7Matz27Bzhrpe9TZ68bfPq7Ed5/eHHS5YJPdCa9PhFEvcHzZCJH7WGxW6faZLw634IqHv8CBRjsyko343tIKzB+bBYfbhx/8cyuONAc3mk2+F6WaDUgxM18yEpQ94iEE4i9uOq4E4ZfMLMLls4pg0AlYs7cRl/71i1FtyHWgQXpG/OJwK5JNely3YAyWTMiBy+vDqn/tCPp+1NnrhtMjXQPzWH0xImb6x8fuSPDxsZ09bhz0j6ecw0BcEbMr/EsvvYRVq1bh0UcfxYIFC/Dggw/ivPPOw4EDB5CXlxerw4qIIAjISzOjpr0XjTYnSjKHzpr4fCLufHkHXB4fzpyUiydumAedTsB3l4zFj17Yhi8rW3Hrc1vwX+dNxm1nVMRdiWesVTZ34bZnt+BQUxcMOgE/PW8SbjytHA6XD7c8uxkbq9pw58vb8foPToNRP/SaU1u3Cy6vD4Kg7QzEkgk5eOLzKnx8oBk+nxh0+b7XJ2LT0Tbsq7fB6fGhIM2C6cXpGJebkhDn5Zq9jVj10nbYnR4UpFnw8PVzMLcsE06PF7c+uwUfH2jGf7+6E/9ecRoMw5xrLV0u+ESpw3i2VZsPPvPKs7C/wY6vqtpwwSnBVV6IoogP9jbita012FNng8crYkxWMk6fkIMLpheEVR1U2dyFlc9vU/al3bq0At9eXI6dxztw58s78NmhFvzt40r86OwJw75XrX9/eEG6JeRtLxQcOQu+NYRAXBRFrNvfhGc3HMPWY+1wenwozUrG6eNzcP70AswvzxqV79cLG6vxyzd2w+MTMbcsE499ay5yrGZ4vD58+8mN+LKyFfe8uQfPfGf+sNdMpYs1A6MRI++9D3bKTW1HL3779l4AwE/Pm4QVZ44HAHxv6Th879nNqG7rwZWPfImHr5+DpRNzR+ag/d7f04BVL21Ht8uL0qwk/OPb8zCpIBU+n4jv/3ML3t/TiJ+9vguv/+C0Ybc4ylU+mclGWIzBVQdRaGaWZgAAtocYiK+vbMXzG6ux43gHXB4fSjKTsHhcNpZPK8C0Udxj7fOJ2HysHe/vacCeuk70uLzIS7XgjEm5uGpOCZJMwZ038sSesTkpyNHos084YhaI//nPf8Ytt9yCm266CQDw6KOP4p133sGTTz6Ju+66K1aHFbG8VCkQD6Zh239212NfvQ2pZgP+dPUs5WEhx2rG09+Zj1+/tRfPbjiG3723H4ebuvC/X5sedBmllomiiFe21ODeN/eg2+VFXqoZj1w/B6f692mZDXr89drZOPeBT7G71oZn1x/Dd04fO+R7yqVZOVYzTAbt9jBcWJGNVLMBDTYHNh9rx/yxQ5d/iqKI17fV4o/vH0Bd58nndG6qGUvG52DpxFycPiFHcxdXp8eL//vwEB75uBIAMK88Ew9fP0d5iDMb9PjDVTNxzp8/wZ46G17YWI1vLSof8j3lpoB5qWbN9oFYNC4bz244hvWVrcO/GFIF0Y9flBYf+2qwObDxaBv+vOYgZpVm4Jp5pbh4RiFSh9mTL18j7nlzD3pcXmSnmPDna2bhDP8DcnFGElxeH3784nb8Ze0hXHhKAcbnDR3oKx3T2ahtxMwqzYBeJ6C+04Hajt5h/657XV785OUdeGdXfb+PH27qwuGmLjz15VEUZyTha3OKccXsYlTkhrZ3Nhi9Li9+/fZevLCxGgBw+awi/L8rZyhBjUGvw/9ecQqWP/gpPjvUgk8PtSjn4WAa7dpt5hgvSrKkc6ut24Vup2fYyoO/rjuMbpcXp5Zl4rYzxikfn1qUhrdWno5bn9uCjVVtuOmpTfj5hVNw4+LyqC8AuTw+/HnNQTz6iXQ/WjwuGw9fNweZ/vnfOp2A31w+HV9WtmJnTSfe3lk3bIk6G7WNPLnS52BjF5rsjmEbMPa6vLj7tZ14Y3tdv4/Lz21/WXcYFbkpuHxWMS6fVRxy/4lgeLw+bDzahvd3N+Dd3Q0DVI504sN9jfjrukN44JpZWDxu+K15X1W1AQDmjGE2vK+YBOIulwtbtmzB3XffrXxMp9PhnHPOwfr16096vdPphNMZOAlstvgdiyNfzOoHCFr6EkURf113GABw85KxyErpv7fIqNfhN5dPx4R8K+57ay9e3VqDg4123H3BZCwal91vJazb6cHBRjv21duxr96Gg412tHQ50d7jhq1X6j4rCIAAAYIA6AQBel3g1zoB/v8XIJzwWun/A19LEAb/vOD/j/wx+b2kDwuBX/f9On0+b9QLKMtOwbjcFIzLtWJ8nhVl2SlKYOz1ifiqqhV/+7gSnx1qAQAsGJuFh66bfdKFLS/Ngv8+fzJ+9vouPPpJJa5bMGbI1d46Odul8ZuRxajH8mkFeHVrDd7cUTtkIO7x+vDLf+/GCxuPAwDSk4xYWJGFFLMBx1p7sLu2E812J17bVovXttUCAKYVpWFmaQZyrGZYzXq4vSKcbi+6nF7YHW50OT3ocnpgd3iU/+/x74Xsdy4NcG4J8gnW7/PSuaMTAq/V6fp/LHCuSb/WCQKyUkyoyE1BRa4VE/OtmJSfitxUs/IeTo8XH+1vwgNrDil7PW9YVIafXzT1pIWa3FQzVp07Efe8uQePfnIE35g/ZsgKjER48FngP68ONNrR2uUcMvNf096Dax7bgNqOXiQZ9fj24jKcPTkfJoMO++tt+GBvIz492Iztxzuw/XgHfv3WXlw0oxDXzCvFqWWZJ2UFjjR34ddv78XHB6TtF4vHZePBa2Yh74S/70tnFuGtHXX4cF8T/rL2MP5y7ewh/0y1Ssd07g8fKUkmPaYVpWFnTSc2H21D8RBBhMvjww2rN2JjVRuMegE3nTYWl80qgtVswIEGOz7Y24j3dzegtqMXD607jIfWHcak/FTMKs1AcWYSkk16uLw+OFxedPa60dHrRqf/h8crIi3JgKwUM8bnWjEh34oJJ9yPHG4vPtjbiAfXHMSRlm4IAnDHORPxw7PGn3ROluek4JsLyvDkF1V44vOqYQPxhk7peSefHdNHTJrFiPQkIzp73ahp78WkgsEX4uo7e/HKFuk++N8XTD5pATUzxYRnb56Pu1/bhde21uLXb+/Fe3sa8JPlk3BqWaYSkMv7sSubpYWiyuYuHGuVGsymmA0Yk5WM8uxkjMuzYkJeKnKsJgiCAKfHi08ONOPBDw9hr7+658bF5fj5RVNOutfkpVpwy5IK/HnNQTz+2RFcOrNoyMyp0qiNiz4jJttqxvTiNOyuteHzQy342pySQV/rcHvxrSe+wuZj7dDrBHxjXikumlGIFJMBBxrtWLevCR8daMKR5m78ec1B/HnNQUwuSMWMknQUZSTBajbA6xPh8vhgd0rPWdLzlvTs5fb6YPVveUk1G5BqMSDVYkSK2QCnxwtbrweVzV3YfrwDnb2B6RWpFgOWTy3A4nHZyEg24lBTF57bcAw17b345j++wp+unokrZg/+5wKAdfsbAQBLJwbfTycRxCQQb2lpgdfrRX5+/8Yl+fn52L9//0mvv//++3HfffeN1uFFpDRLekirbusZ8nV76mzY32CHyaDDTacNnq399qJylGenYMXzW7GrthPX/eMr5FjNKPevgNV19A6YqRyYGOTrYmdrdUe//9frBBSmW2DQCWiyO5WgzagXcMe5E3Hr0nGDZhWvmluChz86jNqOXry8pQbfWlg26Nc91ip9v0ZiZTHeXDqrCK9urcHbO+vxswunINl08mXA4fbiRy9swwd7G6HzP2DesrSi32KG0+PFlqPt+PRQCz492Iy99TbsqZN+qMH6I/2zrxnJRuRYzdAJ0r9fh1vaN5edYsJvL58+ZIn1NfNK8dC6Q6jt6MU7O+tx+ezBA4hj/mvDmCztnmvZVrPSGPDzwy2DZmXau124/h9fobajF+XZyfjHDfP6dfydVZqBb8wfIy34bK3BS5uP40hzN17ZUoNXttSgIicFc8oyUZRuQbfLi501Hdh8rB2iCJj0Ovz4nAm47YyBrxGCIGDVuZPw4b4mvLWzDj86e8KQ3YarWroBaPv7Fg8WVWRjZ00n1u1vGjKbd99be7Cxqg2pZgOeuHFev0XFsuwULJ9WgN9ePh1r/NsdPj3UggON9n5N1EKl1wnItUqVLI02Bzw+6Z6am2rGA1fPGrJh402nleOpL6vw6cFmHGq0D7nVQl4YzmdwNKJKs5LQWevG8baeIQPxf26ohtsrYv7YrEE7pJsNevzp6zMxsyQDv3tvPzZWteHqx9YjI9mIovQk9Lq9aLQ5lGeYYKRZpICp2e5UzrU0iwG/v2oGzp8++P3omwvL8MjHh7G71oZNR4eufJMXfbSehIi1pRNysbvWhk8PNg8aiIuiiJ+9tgubj7UjzWLA3799qjLtBpBK3K8+tRR2hxvv72nEv7fX4ovDLdjfYB+ROeWZyUacPSUfF55SgNPG5/SryD17Sj5uWFSuZO5X/WsHkk0GnDetYMD3qm7twcHGLuh1ApZNVOf245Giii4gd999N1atWqX8v81mQ2lpaQyPaHBjggzE39whlZycMyUP6UlDl1kunZiLtXeegYfWHsbr22rR0uVEywmzL3OsZkwpTMXUwjRMLkxFYXoSslJMSLUYIECACBGiCPjEwM8++Wdfn1/7Pw8Aogjl9wFSGC+Kov9n6SP9P9f/8yJEJfYXT3g/+b3kz0EEet1eVLV0o7K5C5XN3ahs6kKX04Maf0koIN2ELppRiFuXjkN5TsqQf28mgw7fXTIW9721F//ccAzfXDBm0JXhIy1SA4lxw7ynFpw2LhtjspJR3daDFzYex80nlO3bHG7c8vRmfFXVBpNeh79cO2vAm77ZoMfi8TlYPD4Hd10wGc12J7443IIjLd1o6XKi1+WFSa+DyaCD1WKA1b/6Kv1sVP6/7/4i+bySfy32+Xi/c3GA//cp5550PgPSz/J56evzexo6HTjSImUlDjV24WhrNzp63OjoCawA56aacfWpJbj59IqTKlZOZDHqccOicvxpzUE8v7F6yED8qD+gG+78VbtzpubhQKMdb++sHzCgcnulBlbHWntQkpmEF7+3aNCsTG6qGbeeMQ7fW1qBLcfa8dKm43h7Zz2OtHTjiP/vs9/XnpKHuy6YPGy5+dSiNJwzJR8f7mvEcxuO4d5Lpw362sNN0jViQn70y5spYPm0fDz26RGs298El8c34FahFzdW459fVUMQgL9cO3vQQMNi1OOSmUW4ZGYRWruc2HysHXtqO5VFXbNBB4tRj/Qko/IjLckIo16AzeFGo83pv0bYUdncjS6nR9lTC0jbFK6aW4Kbl4wddoRhaVYyzp6SjzV7G/Hq1lrcdcHkQV8rL9aVJ8DCcCyVZiZjd60Nx9sHf17z+kS8urUGAHDDMNuOBEHADYvLcdbkPPx13WG8uaPupPuKQSegLDsZ43KtGJdnRUWOVGVhc3hwrKUbVS3dONzcheq2HtgcHtgcHgDSGLvLZxXjlqUVw24By0ox4bKZxXhp83G8suX4kIG4/KzKLTcja8mEXDzycSU+PdQCt9c3YNXco58cwWvbaqHXCfjbN+f2C8L7SrUYcdXcElw1twQtXU5sOdaOPXU2NNsd6HZ6YdALMBt0/Z61rBYD0iwGGHQ6dLuk7HhXn0y53eGB2ahDqtmA0qxkTC9Ox/SitCF73iSZ9Pjz1bNgMerx4qbjuP3F7Xj5tkUDdob/cJ+UDZ9fnoX05NDGvWpdTALxnJwc6PV6NDY29vt4Y2MjCgpOXk0xm80wm9Wx97Q8W3q4PtZ68sOhzOsT8aZ/78elM4MbMZGXasFvLp+On180BXvqbH2auVgwLjdFkzOhRVFEo82J2o5eiKKIjGQTyrOTh22G1dfXZpfg/nf3Y3+DHbtqOzHD373yRJXN0vdrJPYQxhuDXofbzhiHn72+C499Uokr5xQr50+TzYEbVm/CvnobrGYD/v7tuUHt/QGkYGmoADSeOdxeVDZ3obPXDZ8PKMywYGx2Skh7/K46tQQPfHgQG6vacKy1G2XZAwfacmZ1bI62H7IvnVmMhz+qxMcHmtDZ4z7p5vvbt/di/ZFWpJj0eOKGeUGVRgqCgFPLs3BqeRbuuXSaP7vYhZYuJ8wGHcblWbFkQs6wjTL7+taiMny4T8qa3nXB5AG3sIiiqATioc7opdDMKs1EjtWMli4nvqpqxZIJ/cu4t1a341f/3gMAuPPciThzcnDZlWyrGedNKxg0YzMc+X7UbHfCK4rITTWjKN0SUsOkK2YXY83eRry1ow7/dd6kQa8v8vPDYNcQig65gvF4W++gr/mysgX1nQ6kJxlx9pTgzrXSrGT87qoZ+M3l03Gw0Y7mLieSjXrkpppRmpU8bPNYQLonHWvtgcPtRU6qGYVpoTWJvHJuCV7afBz/2dWA+y6dPmhDraOtibEwHGunlgeua2v3NeH86f2vQ2v2NuL370sVwfdeMhWnjQ/uuSsnwutapHQ6Ab+9fDpqO3rx2aEW3PLMZryx4rR+W+9EUcRr26TFrHOnBjfCMZHEpCuVyWTC3LlzsXbtWuVjPp8Pa9euxaJFi2JxSFFT5l/BPt7eC59v4FLwjVVtaLA5kGox4MzJoXXXtBj1mFuWiQtOKcQFpxRiblmmJoNwQHroLki3YG5ZJk4tz8L4PGtIQTgApCcbcYH/gvfipuODvi4QHCXGzejKucUoz05Gk92JH76wDTaHGx/ubcTFD32OffU25FjNePF7C4MOwtXOYtRjWlE6Fo/LwekTcjAu1xpyo53C9CSc7g8aXtlSM+jr5AefsTnaDugmFaRickEq3F4Rb2yv7fe5Z9YfxdPrjwEAHrhm1pBloYOxmg248JRC/PicCfjN5dPxi4un4tr5Y0IKwgFgyfgclGQmwebw4J2d9QO+ptHmRJfTA71OUBZbaWTodYLysCY3QJM12Ry47dktcHl9OH9agdK5ejTI96NTStKlfeYZSSF3LT5rch6sZgNqO3qxZZDRfm6vT2kMyHNtZJVmSlngoTLiL2+WruWXziwKuau4yaDD9OJ0nDkpDwsqslGRaw0qCAeke9KkglTM9J9rod6PTi3LRGlWErqcHnywd/AxuEcT7NknVox6Hb5+qlSSfuJ1bX+DDbe/uA2iCHxz4ZhhG77GG4Neh79eNwfjclNQ3+nATas3we4IVIF8VdWG3bU2mAw6XKHSZM1Iill76FWrVuHxxx/H008/jX379uH73/8+uru7lS7qaiXvZ3Z5fP1K2Pr6t/+h9MLpheyCPgquOVXaxvDm9jr0uDwnfd7ucCtzncfmJsbNyGzQ42/fnAuLUYfPDrVgxr0f4LvPbEaT3YnxeVa8+v2By4toaF+fK91oX91SM+BCXI/Lg0ab/1xLgIfs6xaMAQA88vFh2Pw35g/2NODeN6WM5k/Pm4TlMVrJl+l0Aq6dLx3n8yc8IMkONUn778qykzU9VSFe3Li4HADw7u4GHPLv6e5xeXCL/xo1Ic+KP149U3WjEy1GvZK5+vcJi1Oyuo5eeHwizAYd59WPsBIlIz5wIC7txZWCWDmIUgudTsBl/orLt3YMvMBoc7jR2u0CwIz4aPjGPOlZ9JODzcpM8Zr2Htz45CZ0u7xYPC4b91wy+PaoeJaeZMSTN85DjtWEvfU2fO+ZLf4Z9V78xj/275pTS5UO/xQQsyeKa665Bn/84x/xq1/9CrNmzcL27dvx3nvvndTATW0Meh1K/KuscgOwvpweL/7jH7Vy2eyiUT22RLWwQtoT3eX0KDfVvuRseI7VPOw+Py2ZUpiGp2+ajwr/4oPVbMD3llbg3ytOY0lkmM6dmo80iwF1nY6TmsEBwNEW6ZqQmWxMiH1SV59airLsZDTanLjl6c347dt7cdtzW+ATpZvyD5aNG/5NRsHXTy2BXidgy7F2JfDr61Cjf384y9JHxaSCVJw/rQCiCNz92i5sq27Ht5/YiB01nchMNuLv3z4V1mHGTcWry2ZJ9/13dtbD4/Wd9Pmj/ueGsuxkzqsfYaWZgUBc7lnT1wd7GuH0+FCRm4JTVLgwfclM6Vz75KC0PehEx/z3I2nKiTr/PalJWXaKkhFe8fxW/OOzI7j84S/RYHNgQp4Vj1w/J+iKiXhUlp2C1TfOR7JJj/VHWnHBg5/i0oe+wJ46G9KTjPjh2aNXwaQmMf2Or1y5EseOHYPT6cRXX32FBQsWxPJwomaMP4ipbjt5n/jHB5phc3iQn2bGgrEDN2Kg6NLpBHxtjnTxG6hk+IiyPzzxgs8FFdlYu+oMbPvludj2q3PxswunDDtPlQZnMepx0Qzp4ee1rSdnvKoSpFGbzGLU48FrZiHJqMdXVW34x+dV8InSRIPfXjE9bjKaeakWnOXfa/zSAFtY5Iw494ePnv++YDKsZgM2H2vHFY98ic3H2mE1G/CPG+apuox28bhsZKWY0N7jHnCxjvvDR8+YrGQYdAK6Xd4BKxjf2in38hl6BFi8mlSQion5Vri9It4foDy9qjUx+pXEk19ePBVjspJR096L376zDy1dTkzKT8UzN8/XxDbTU0rS8dL3FqEkMwl1nQ4caLTDajbgb9fPGXZ+eqJS79JLHBvr3ycuNwDrSy5Hu3Rm0aBjtyj6rvSPi/iyslWZByzbXdsJAJg0xDgZLRMEAZkpJlWvxMYTedHnvd316D1hVM2BBmm02/gEaAoomz0mE/9eeRqunT8GF88oxN+un4M/XDUj7s43uWzwtW21cHn6Zyq3H5euEWrMiqnV2JwUPPfdBZhRkg6TQYfTx+fg7R+ejrllmbE+tIgY9DqlPF2ujutLrqRjx/SRZzLolEWdAyeMf2rrduHzQy0AApllNbrEvzD89gD9L+T94Vz0GT1ZKSa8/oPFuHFxOU4fn4M7zpmIf688DYXp2ulaf0pJOtbccQYeunY27v/aKVj3kzOwOMjmc4mIqa8RMLkwDQCw94R5ynaHGx/uawKAIeejUvSVZiVjYUUWNhxpw+tba7DyrAnK53bUdACQZjQSRUpuknO8rRcf7G3o9299l3/R55SSxAroJuan4v6vnRLrwxjSGRNzkZ9mRqPNiQ/3NeJC/9z4bqdHWUCZPUbdQaDazCrNwJsrT4/1YUTdxTMK8cLGary3uwG/vmx6v0UpOSAcl0CLdbE0MT8Vh5q6cKDBjmWTAl3R391dD49PxLSiNFV/Ly6eWYQ/rTmILw63oLXLiew+o8/kSRBqrjBRo2yrechRmVqQZNKregFrNMVXSkIjphVJgfieus5++47e290Al8eHcbkpymto9MhZ8Ve31irfF6fHqwRHs0oTKziikSEIAq6YHTjXZKIoYmeNdK6xEV78Meh1uMrfbK/vhIUNR1rhE4GSzKR+I1mIwrVgbBay/eXpG/qUp4uiiN110jViWhGvEaNhqv9ZTL42ywIjZtUdTIzNScH04jR4fSLe3d2/PF2uBuTzKFHsMBAfARPzU2HUC2jvcfdr2CbvGb1sVrEq9xup3YWnFCLZpEdVSze+qmoDAGw51g6H24fcVLOqV70pvsgNWT4/1Iwm/97Dg41daO12wWLU8cEnTl3tn7Dw2aFmHPbvC//ogFTFdMbE0EZNEg3GoNcpc4T7jsyr7ehFR48bBp2AiQW8H42GOf4ql219xsnVd/Zi41HpGeFilQfiQN/y9DrlY3aHG0f8pencckMUOwzER4DFqMfMkgwAUC7mR1u6sf5IKwQBuHKuusZgaEWK2aCUCT/80WEAwId7pYfs08fncHGEomZsTgrmlmXCJwJPrz8KQAruAGBeeRbHFsapsuwULJ+aD1EE/vTBQTg9XiVQOmequid6UHy5yL/14f09DUpPgo3+BeJpRWm8RoySmaXpMOgE1HU6lD3Tz39VDVGUKheKM9S/d/eiGdK59lVVGxr9C8Obj0kLD6VZSf3K1YlodDEQHyELKrIASPMCAeClzVKp49IJuZq4sKvVD5aNg0En4LNDLfhwbyPe8DfPu2RmYYyPjLTme0srAABPf3kMnT1uvLlDykbI3bkpPt25fBIEQZphfe3fN6C9x438NDOWsNkMRdH8sVnISzWjvcetNG1bXymVqS+s4ESV0ZJsMmD+WOl5be3+JjjcXjz/VTUA4Ab/PHu1K8lMxpwxGRDFQNO2Lw9LjegWV/C6RhRLDMRHiNwVdd2+Jhxv68FzG44BAK6dXxrLw0p4pVnJuNrfHfm7z2xGW7cLZdnJWDqBZacUXedOycek/FR0OT04//8+xc6aThj1AhuYxLlJBam4afFYAMDW6g4AwE+WT4Ihzrq8k7oZ9Dp8a2EZAOCJz6vg9vrw4b5GAMAS3o9G1XJ/tcu/Nh3HM+uPorXbhcJ0i/JxLZCrAZ/bcAwer0/ZL75kIgNxoljik8UIOaU4HRPyrOh1e7Hk9x/B7vBgUn4qlk8tiPWhJbyfXzgFs/wd0q1mA/5w1Uw+ZFPU6XQCfn3ZNOh1Auo7pXLA7y6pQA7LAOPezy6cjFXnTsSCsVn4zeXTlSZuRNF0/cIymA067KrtxNWPrUd7jxs5VjMW+ivqaHRcMacEKSY9DjTa8b//2Q8A+PHZEzT1XHDV3BJkJBtR1dKNS/76BWrae2E1G3D2ZO0sNhCpkXauMnFGEAT84uKpkEeFmww6/O6qGdBxdnjMpZgNeOW2RXj9B4vx6X+dqZSlEUXbgopsPPOd+bjwlAL89/mTcee5E2N9SBQEg16HH509AS/dugjfWljG/hE0IrJSTLjtjHEAgG3+6otbl1ZoKgBUg/QkI357xXTlee3yWUVK40atSDEb8F/nTQYA7KuXxjHedFo5kkzsRUAUS5wjPoLOmJiLl25dhM8OteCC6QWYUshOyfHCoNdxJjCNitPG5+A07i8mogH88KzxsDnceG93A86bVoCbTiuP9SElpCtml2BeeRbsDg8mF6RqcvHt2vmlaO9x4bWtNVg8Lgcrzxof60MiSngMxEfYvPIszCtnxpWIiIj6M+h1uOeSabjnkmmxPpSEV5KZHOtDGFGCIGDFmeOx4kwG4ETxgvVPRERERERERKOIgTgRERERERHRKGIgTkRERERERDSKGIgTERERERERjSIG4kRERERERESjiIE4ERERERER0ShiIE5EREREREQ0ihiIExEREREREY0iBuJEREREREREo4iBOBEREREREdEoYiBORERERERENIoYiBMRERERERGNIgbiRERERERERKOIgTgRERERERHRKGIgTkRERERERDSKGIgTERERERERjSIG4kRERERERESjiIE4ERERERER0ShiIE5EREREREQ0ihiIExEREREREY0iBuJEREREREREo4iBOBEREREREdEoYiBORERERERENIoYiBMRERERERGNIgbiRERERERERKPIEOsDCIcoigCAni57zI7BZkuK2dem2OiO0fnGcy2xROs843kTG4N9//j9oGgK5jqhhXMuGtdDLfw9xFKinGtEwbLZbAAC8WgkVBmIt7a2AgCuO3tOjI+EiIiIiIiIEklrayvS09Mjeg9VBuJZWVkAgOrq6oj/AoiGM2/ePGzatCnWh0EJgOcajRaeazRaeK7RaOG5RqOhs7MTY8aMUeLRSKgyENfppK3t6enpSEtLi/HRkNbp9XqeZzQqeK7RaOG5RqOF5xqNFp5rNJrkeDSi94jCcRBp2ooVK2J9CJQgeK7RaOG5RqOF5xqNFp5rpDaCGI2d5qPMZrMhPT0dnZ2dXPkiIiIiIiKiERfNOFSVGXGz2Yx77rkHZrM51odCRERERERECSCacagqM+JEREREREREaqXKjDgRERERERGRWjEQJ/J7+OGHUV5eDovFggULFmDjxo0AgLa2Nvzwhz/EpEmTkJSUhDFjxuBHP/oROjs7Y3zEpFaDnWsAcOutt2LcuHFISkpCbm4uLrvsMuzfvz+GR0tqNtS5JhNFERdccAEEQcAbb7wx+gdJmjDUubZs2TIIgtDvx2233RbDoyU1G+66tn79epx11llISUlBWloali5dit7e3hgdLdHgGIgTAXjppZewatUq3HPPPdi6dStmzpyJ8847D01NTairq0NdXR3++Mc/Yvfu3Xjqqafw3nvv4eabb471YZMKDXWuAcDcuXOxevVq7Nu3D++//z5EUcTy5cvh9XpjfOSkNsOda7IHH3wQgiDE6ChJC4I512655RbU19crP37/+9/H8IhJrYY719avX4/zzz8fy5cvx8aNG7Fp0yasXLkyKqOmiKJOJCJx/vz54ooVK5T/93q9YlFRkXj//fcP+Pp//etfoslkEt1u92gdImlEqOfajh07RADi4cOHR+sQSSOCOde2bdsmFhcXi/X19SIA8fXXX4/BkZLaDXeunXHGGeKPf/zjGB0daclw59qCBQvEX/ziF7E6PKKQxP3y0FDlJ3//+9+xbNkypKWlQRAEdHR0xO5ASbVcLhe2bNmCc845R/mYTqfDOeecg/Xr1w/4e+SRBQaDYbQOkzQg1HOtu7sbq1evxtixY1FaWjqah0oqF8y51tPTg+uuuw4PP/wwCgoKYnWopHLBXtf++c9/IicnB9OnT8fdd9+Nnp6eWBwuqdhw51pTUxO++uor5OXlYfHixcjPz8cZZ5yBzz//PIZHTWo2WBx69OjRk7bbyD9efvnloN8/rgPx4cpPenp6cP755+NnP/tZjI+U1KylpQVerxf5+fn9Pp6fn4+GhoYBX/+b3/wG3/ve90brEEkjgj3XHnnkEVitVlitVrz77rtYs2YNTCbTaB8uqVgw59odd9yBxYsX47LLLovFIZJGBHOuXXfddXjuuefw0Ucf4e6778azzz6Lb37zm7E4XFKx4c61I0eOAADuvfde3HLLLXjvvfcwZ84cnH322Th06FAsDplUbKg4tLS0tN9Wm/r6etx3332wWq244IILgv4acZ3O+/Of/4xbbrkFN910EwDg0UcfxTvvvIMnn3wSd911F26//XYAwMcffxy7g6SEYrPZcNFFF2Hq1Km49957Y304pFHXX389zj33XNTX1+OPf/wjrr76anzxxRewWCyxPjTSiDfffBPr1q3Dtm3bYn0olAD6LlyfcsopKCwsxNlnn43KykqMGzcuhkdGWuLz+QBITU/l2GH27NlYu3YtnnzySdx///2xPDxSmeHi0BMryV5//XVcffXVsFqtQX+NuM2Ih1MuTBSOnJwc6PV6NDY29vt4Y2Njv39kdrsd559/PlJTU/H666/DaDSO9qGSygV7rqWnp2PChAlYunQpXnnlFezfvx+vv/76aB8uqdhw59q6detQWVmJjIwMGAwGZZvNlVdeiWXLlsXgiEmtgr2u9bVgwQIAwOHDh0f8+Eg7hjvXCgsLAQBTp07t9/kpU6agurp61I6T1C/UOHTLli3Yvn17yI2c4zYQD7VcmChcJpMJc+fOxdq1a5WP+Xw+rF27FosWLQIgZcKXL18Ok8mEN998k5lJCksw59qJRFGEKIpwOp2jdZikAcOda3fddRd27tyJ7du3Kz8A4IEHHsDq1atjdNSkRuFc1+TzTQ6ciIIx3LlWXl6OoqIiHDhwoN/vO3jwIMrKykb7cEnFQo1Dn3jiCUyZMgWLFy8O6evEdWk60WhZtWoVbrjhBpx66qmYP38+HnzwQXR3d+Omm25SgvCenh4899xzsNlssNlsAIDc3Fzo9foYHz2pyVDn2pEjR/DSSy9h+fLlyM3NRU1NDf7f//t/SEpKwoUXXhjrQyeVGepcy8/PHzBbOWbMGIwdOzYGR0tqNtS5VllZieeffx4XXnghsrOzsXPnTtxxxx1YunQpZsyYEetDJ5UZ6lwTBAE//elPcc8992DmzJmYNWsWnn76aezfvx+vvPJKrA+dNKq3txfPP/88fvnLX4b8e+M2EA+n1IkoXNdccw2am5vxq1/9Cg0NDZg1axbee+895Ofn4+OPP8ZXX30FABg/fny/31dVVYXy8vIYHDGp1VDnWl1dHT777DM8+OCDaG9vR35+PpYuXYovv/wSeXl5sT50UpmhzjWiaBrqXHO5XPjwww+VgKm0tBRXXnklfvGLX8T6sEmFhruu3X777XA4HLjjjjvQ1taGmTNnYs2aNexFQCEJJQ595ZVX0NPTg29/+9shfx1BFEUxoiMdQQsWLMD8+fPx0EMPAZDKT8aMGYOVK1firrvuUl738ccf48wzz0R7ezsyMjJidLRERERERESkdsHGocuWLUNOTk5YVRdxmxEHhi4/AYCGhgY0NDQozT527dqF1NRUjBkzBllZWbE8dCIiIiIiIlKh4eJQQGo4+emnn+I///lPWF8jrgPx4cpPHn30Udx3333K65cuXQoAWL16NW688cZYHDIRERERERGpWDDbu5588kmUlJRg+fLlYX2NuC5NJyIiIiIiItKauB1fRkRERERERKRFDMSJiIiIiIiIRhEDcSIiIiIiIqJRxECciIiIiIiIaBQxECciIiIiIiIaRXEZiN944424/PLLY30YRERERERERFEXl4E4ERERERERkVbFfSD+3nvv4fTTT0dGRgays7Nx8cUXo7KyUvn80aNHIQgCXnvtNZx55plITk7GzJkzsX79+hgeNREREREREdHA4j4Q7+7uxqpVq7B582asXbsWOp0OV1xxBXw+X7/X/fznP8dPfvITbN++HRMnTsS1114Lj8cTo6MmIiIiIiIiGpgh1gcwnCuvvLLf/z/55JPIzc3F3r17MX36dOXjP/nJT3DRRRcBAO677z5MmzYNhw8fxuTJk0f1eImIiIiIiIiGEvcZ8UOHDuHaa69FRUUF0tLSUF5eDgCorq7u97oZM2Yovy4sLAQANDU1jdpxEhEREREREQUj7jPil1xyCcrKyvD444+jqKgIPp8P06dPh8vl6vc6o9Go/FoQBAA4qXydiIiIiIiIKNbiOhBvbW3FgQMH8Pjjj2PJkiUAgM8//zzGR0VEREREREQUvrgOxDMzM5GdnY2///3vKCwsRHV1Ne66665YHxYRERERERFR2OJyj7jP54PBYIBOp8OLL76ILVu2YPr06bjjjjvwhz/8IdaHR0RERERERBQ2QRRFMdYHcaLzzz8f48ePx1//+tdYHwoRERERERFRVMVVRry9vR1vv/02Pv74Y5xzzjmxPhwiIiIiIiKiqIurPeLf+c53sGnTJtx555247LLLYn04RERERERERFEXl6XpRERERERERFoVV6XpRERERERERFrHQJyIiIiIiIhoFMUkEL///vsxb948pKamIi8vD5dffjkOHDjQ7zUOhwMrVqxAdnY2rFYrrrzySjQ2NvZ7zY9+9CPMnTsXZrMZs2bNGvBr/etf/8KsWbOQnJyMsrIyjj8jIiIiIiKimIpJIP7JJ59gxYoV2LBhA9asWQO3243ly5eju7tbec0dd9yBt956Cy+//DI++eQT1NXV4Wtf+9pJ7/Wd73wH11xzzYBf591338X111+P2267Dbt378YjjzyCBx54gGPRiIiIiIiIKGbiollbc3Mz8vLy8Mknn2Dp0qXo7OxEbm4unn/+eVx11VUAgP3792PKlClYv349Fi5c2O/333vvvXjjjTewffv2fh+/7rrr4Ha78fLLLysfe+ihh/D73/8e1dXVEARhxP9sRERERERERH3FxR7xzs5OAEBWVhYAYMuWLXC73f1miU+ePBljxozB+vXrg35fp9MJi8XS72NJSUmoqanBsWPHonDkRERERERERKGJeSDu8/lw++2347TTTsP06dMBAA0NDTCZTMjIyOj32vz8fDQ0NAT93ueddx5ee+01rF27Fj6fDwcPHsSf/vQnAEB9fX3U/gxEREREREREwYp5IL5ixQrs3r0bL774YtTf+5ZbbsHKlStx8cUXw2QyYeHChfjGN74BANDpYv5HJyIiIiIiogQU02h05cqVePvtt/HRRx+hpKRE+XhBQQFcLhc6Ojr6vb6xsREFBQVBv78gCPjd736Hrq4uHDt2DA0NDZg/fz4AoKKiIip/BiIiIiIiIqJQxCQQF0URK1euxOuvv45169Zh7Nix/T4/d+5cGI1GrF27VvnYgQMHUF1djUWLFoX89fR6PYqLi2EymfDCCy9g0aJFyM3NjfjPQURERERERBQqQyy+6IoVK/D888/j3//+N1JTU5V93+np6UhKSkJ6ejpuvvlmrFq1CllZWUhLS8MPf/hDLFq0qF/H9MOHD6OrqwsNDQ3o7e1VuqZPnToVJpMJLS0teOWVV7Bs2TI4HA6sXr1aGYdGREREREREFAsxGV822Niw1atX48YbbwQAOBwO3HnnnXjhhRfgdDpx3nnn4ZFHHulXmr5s2bIBg+qqqiqUl5ejpaUFl1xyCXbt2gVRFLFo0SL8z//8DxYsWDAify4iIiIiIiKi4cTFHHEiIiIiIiKiRMHW4URERERERESjiIE4ERERERER0ShiIE5EREREREQ0ihiIExEREREREY0iBuJEREREREREo4iBOBEREREREdEoYiBORERERERENIoYiBMRERERERGNIgbiRERERERERKOIgTgRERERERHRKGIgTkRERERERDSKGIgTERERERERjaL/D46VJLJ5jjjQAAAAAElFTkSuQmCC\n",
                         "text/plain": [
                             "<Figure size 1200x800 with 1 Axes>"
                         ]
@@ -1073,15 +1081,17 @@
                 "                             'Attenuated Power': my_data['Compressor Power'].apply(attenuate_power)})\n",
                 "clipped_data.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
-            "metadata": {},
+            "metadata": {
+                "keep_output_in_docs": true
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<AxesSubplot:>"
                         ]
                     },
@@ -1220,13 +1230,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.8"
+            "version": "3.8.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Version Considerations.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Version Considerations.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/Workbook Templates.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/Workbook Templates.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9852276879100219%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/html\': [\'<div style="background-color: '*

 * *            '#EEFFEE;color:black; text-align: left;">Logged in to '*

 * *            '<strong>http://localhost:34216</strong> successfully as '*

 * *            '<strong>agent_api_key</strong>.<br>Seeq Server Version: '*

 * *            '<strong>R63.0.0-SNAPSHOT</strong><br>Seeq SDK Module Version: <strong>63.0.0</strong> '*

 * *            '@ C:\\\\GitHub\\\\crab\\\\sdk\\\\pypi\\\\seeq\\\\sdk<br>Seeq SPy Module Version: '*

 * *         […]*

```diff
@@ -27,15 +27,15 @@
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Logged in to <strong>http://localhost:34216</strong> successfully as <strong>agent_api_key (Mark Derbecker)</strong>.<br>Seeq Server Version: <strong>R61.0.0-SNAPSHOT</strong><br>Seeq SDK Module Version: <strong>61.0.0</strong> @ C:\\GitHub\\crab\\sdk\\pypi\\seeq\\sdk<br>Seeq SPy Module Version: <strong>185.3</strong> @ C:\\GitHub\\crab\\sdk\\pypi\\seeq\\spy</div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Logged in to <strong>http://localhost:34216</strong> successfully as <strong>agent_api_key</strong>.<br>Seeq Server Version: <strong>R63.0.0-SNAPSHOT</strong><br>Seeq SDK Module Version: <strong>63.0.0</strong> @ C:\\GitHub\\crab\\sdk\\pypi\\seeq\\sdk<br>Seeq SPy Module Version: <strong>189.1</strong> @ C:\\GitHub\\crab\\sdk\\pypi\\seeq\\spy</div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -168,30 +168,54 @@
                 "# Retrieve a specific analysis worksheet from the list of returned workbooks\n",
                 "worksheet = analysis_template.worksheets['Trend Template']\n",
                 "\n",
                 "worksheet"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "c6b81030",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[Workbook \"Users >> mark.derbecker@seeq.com >> Workbook Templates >> Analysis Template\" (F01FD57A-1112-4020-9430-CF27C2847D1B agent_api_key Workbook Template Example 1),\n",
+                            " Workbook \"Users >> mark.derbecker@seeq.com >> Workbook Templates >> Data Lab Visualization Example\" (6BAED6F7-3DF3-4238-AB18-7A9ABE284581 agent_api_key Workbook Template Example 1),\n",
+                            " Workbook \"Users >> mark.derbecker@seeq.com >> Workbook Templates >> Topic Template\" (90931EF8-D80B-4F22-8568-3683DD806D50 agent_api_key Workbook Template Example 1)]"
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "workbooks"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "id": "b934ba1f",
             "metadata": {
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "When you load a workbook as a template, it exposes a `code` attribute that tells you how to plug specific items into the template. These are referred to as the _parameters_."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "id": "adb25e8e",
             "metadata": {
+                "keep_output_in_docs": true,
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
@@ -239,15 +263,15 @@
                 "## Pushing with a Template Worksheet\n",
                 "\n",
                 "First let's create a metadata DataFrame with some sinusoids:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "id": "4c9e319d",
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
@@ -277,15 +301,15 @@
             },
             "source": [
                 "Next, we will copy and paste the code block that we printed earlier into a real code cell so that we can set the parameters appropriately. In this example, we're just specifying the `Name` of the signals (replacing the `None` placeholders), but we could have supplied `ID`, `Type`, `Path` and/or `Asset` values that correspond to the row being pushed. (It can also be a one-row DataFrame instead of a dictionary.)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "id": "431c4e06",
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
@@ -314,26 +338,26 @@
             },
             "source": [
                 "Now we push the metadata DataFrame and pass in the worksheet argument:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "id": "80286f9e",
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>1EDA1D09-E491-6A26-A0B3-DD1752345222</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/1EDA1CB1-F3BF-6338-A64B-AF0F60A998BD/workbook/1EDA1D09-E491-6A26-A0B3-DD1752345222/worksheet/1EDA1D09-E889-644C-AF5D-DF75684CC17F\" target=\"_new\">http://localhost:34216/1EDA1CB1-F3BF-6338-A64B-AF0F60A998BD/workbook/1EDA1D09-E491-6A26-A0B3-DD1752345222/worksheet/1EDA1D09-E889-644C-AF5D-DF75684CC17F</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/0EE1D1BF-8B15-FDC0-AE5B-568A5610931A/workbook/0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A/worksheet/0EE1D1BF-9C98-6480-8790-737270A49CCD\" target=\"_blank\">http://localhost:34216/0EE1D1BF-8B15-FDC0-AE5B-568A5610931A/workbook/0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A/worksheet/0EE1D1BF-9C98-6480-8790-737270A49CCD</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -373,75 +397,75 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>Sinusoid 1</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>sinusoid(1h)</td>\n",
-                            "      <td>1EDA1D09-E491-6A26-A0B3-DD1752345222</td>\n",
+                            "      <td>0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>[]</td>\n",
-                            "      <td>[1EDA1D09-E491-6A26-A0B3-DD1752345222] {Signal...</td>\n",
-                            "      <td>1EDA1D09-E5A3-612E-83FC-A33ECBD7AA48</td>\n",
+                            "      <td>[0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A] {Signal...</td>\n",
+                            "      <td>0EE1D1BF-96F7-FDA0-B0A5-E336623058AF</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>Sinusoid 2</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>sinusoid(2h)</td>\n",
-                            "      <td>1EDA1D09-E491-6A26-A0B3-DD1752345222</td>\n",
+                            "      <td>0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>[]</td>\n",
-                            "      <td>[1EDA1D09-E491-6A26-A0B3-DD1752345222] {Signal...</td>\n",
-                            "      <td>1EDA1D09-E5CA-6234-890E-BBED9BC6C3A9</td>\n",
+                            "      <td>[0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A] {Signal...</td>\n",
+                            "      <td>0EE1D1BF-97D6-6050-B707-05240DB67E2B</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>Sinusoid 3</td>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>sinusoid(3h)</td>\n",
-                            "      <td>1EDA1D09-E491-6A26-A0B3-DD1752345222</td>\n",
+                            "      <td>0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>[]</td>\n",
-                            "      <td>[1EDA1D09-E491-6A26-A0B3-DD1752345222] {Signal...</td>\n",
-                            "      <td>1EDA1D09-E5CA-623A-8DA9-27B85C9FA1BD</td>\n",
+                            "      <td>[0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A] {Signal...</td>\n",
+                            "      <td>0EE1D1BF-97F3-7510-8F52-F225AD42ED56</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "         Name              Type       Formula  \\\n",
                             "0  Sinusoid 1  CalculatedSignal  sinusoid(1h)   \n",
                             "1  Sinusoid 2  CalculatedSignal  sinusoid(2h)   \n",
                             "2  Sinusoid 3  CalculatedSignal  sinusoid(3h)   \n",
                             "\n",
                             "                              Scoped To Datasource Class  Datasource ID  \\\n",
-                            "0  1EDA1D09-E491-6A26-A0B3-DD1752345222    Seeq Data Lab  Seeq Data Lab   \n",
-                            "1  1EDA1D09-E491-6A26-A0B3-DD1752345222    Seeq Data Lab  Seeq Data Lab   \n",
-                            "2  1EDA1D09-E491-6A26-A0B3-DD1752345222    Seeq Data Lab  Seeq Data Lab   \n",
+                            "0  0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A    Seeq Data Lab  Seeq Data Lab   \n",
+                            "1  0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A    Seeq Data Lab  Seeq Data Lab   \n",
+                            "2  0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A    Seeq Data Lab  Seeq Data Lab   \n",
                             "\n",
                             "  Formula Parameters                                            Data ID  \\\n",
-                            "0                 []  [1EDA1D09-E491-6A26-A0B3-DD1752345222] {Signal...   \n",
-                            "1                 []  [1EDA1D09-E491-6A26-A0B3-DD1752345222] {Signal...   \n",
-                            "2                 []  [1EDA1D09-E491-6A26-A0B3-DD1752345222] {Signal...   \n",
+                            "0                 []  [0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A] {Signal...   \n",
+                            "1                 []  [0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A] {Signal...   \n",
+                            "2                 []  [0EE1D1BF-8CD2-7320-9148-A66D3BAEBF7A] {Signal...   \n",
                             "\n",
                             "                                     ID Push Result  \n",
-                            "0  1EDA1D09-E5A3-612E-83FC-A33ECBD7AA48     Success  \n",
-                            "1  1EDA1D09-E5CA-6234-890E-BBED9BC6C3A9     Success  \n",
-                            "2  1EDA1D09-E5CA-623A-8DA9-27B85C9FA1BD     Success  "
+                            "0  0EE1D1BF-96F7-FDA0-B0A5-E336623058AF     Success  \n",
+                            "1  0EE1D1BF-97D6-6050-B707-05240DB67E2B     Success  \n",
+                            "2  0EE1D1BF-97F3-7510-8F52-F225AD42ED56     Success  "
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "spy.push(metadata=metadata_df, workbook='Workbook Template Example 1', worksheet=worksheet)"
             ]
@@ -479,58 +503,68 @@
                 "## Pushing with a Template Workbook\n",
                 "\n",
                 "You can also push an entire workbook instead of just a single worksheet. Following much the same pattern, you will print the parameters code for the workbook like so:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "id": "e9a8feeb",
-            "metadata": {
-                "pycharm": {
-                    "name": "#%%\n"
-                }
-            },
+            "execution_count": 9,
+            "id": "0c0ada40",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Success</div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
-                },
+                }
+            ],
+            "source": [
+                "workbooks = spy.workbooks.load('./Support Files/Workbook Templates.zip',\n",
+                "                               as_template_with_label=f'{spy.user.username} Workbook Template Example 2')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "e9a8feeb",
+            "metadata": {
+                "keep_output_in_docs": true,
+                "pycharm": {
+                    "name": "#%%\n"
+                }
+            },
+            "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "workbook.parameters = {\n",
                         "    \"D2C089B6-CE85-46FC-8392-E11CC0C08336 [Signal] Area A_Compressor Stage\": None,\n",
                         "    \"9564A6B8-8A8F-4F6D-AC63-00EA38962B7A [Signal] Area A_Temperature\": None,\n",
                         "    \"DCED9C36-A4BE-4783-9216-DC06B3F57D8C [Signal] Area A_Compressor Power\": None,\n",
                         "    \"Temperature Journal Link Text\": None,\n",
                         "    \"Compressor Power Journal Link Text\": None,\n",
                         "    \"Compressor Stage Journal Link Text\": None,\n",
                         "    \"favorite color\": None,\n",
                         "    \"8A4F0E26-8A0C-4127-9E11-B67E031C6049 [Signal] Example >> Cooling Tower 1 >> Area A >> Temperature\": None,\n",
-                        "    \"07F3161F-6644-4505-BC33-16D6155B004E [Condition] Hot\": None,\n",
-                        "    \"4B40EAFC-91ED-4AB0-8199-F21AF40A8350 [Asset] Example >> Area A\": None,\n",
-                        "    \"D16FC368-AE8E-47B4-B1A3-9C2A3FBA2BB6 [Asset] Cooling Tower 1\": None\n",
+                        "    \"D16FC368-AE8E-47B4-B1A3-9C2A3FBA2BB6 [Asset] Example >> Cooling Tower 1\": None,\n",
+                        "    \"4B40EAFC-91ED-4AB0-8199-F21AF40A8350 [Asset] Example >> Cooling Tower 1 >> Area A\": None,\n",
+                        "    \"07F3161F-6644-4505-BC33-16D6155B004E [Condition] Hot\": None\n",
                         "}\n"
                     ]
                 }
             ],
             "source": [
-                "workbooks = spy.workbooks.load('./Support Files/Workbook Templates.zip',\n",
-                "                               as_template_with_label=f'{spy.user.username} Workbook Template Example 2')\n",
-                "\n",
                 "# Retrieve a specific workbook from the list of returned workbooks\n",
                 "workbook = workbooks['Analysis Template']\n",
                 "\n",
                 "print(workbook.code)"
             ]
         },
         {
@@ -543,15 +577,15 @@
             },
             "source": [
                 "Again, we will create a DataFrame full of signals, but this time we'll put them in an asset tree so we can illustrate how to properly populate a Treemap template."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 11,
             "id": "f8da2513",
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
@@ -569,15 +603,15 @@
                 "     'Formula': 'squareWave(12h, 15V)'},\n",
                 "    {'Path': 'Waveforms', 'Asset': 'Waveforms 2', 'Name': 'Hours', 'Type': 'Condition', 'Formula': 'hours()'},\n",
                 "])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 12,
             "id": "2e52e11a",
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
@@ -620,26 +654,26 @@
             },
             "source": [
                 "Now when we push, we'll pass the `workbook` argument instead of the `worksheet` argument."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 13,
             "id": "04835241",
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>1EDA1D09-ECCF-6066-BA4C-83098973BDE0</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/1EDA1CB1-F3BF-6338-A64B-AF0F60A998BD/workbook/1EDA1D09-ECCF-6066-BA4C-83098973BDE0/worksheet/1EDA1D09-F4E5-6604-A979-ED5BDD4B4F65\" target=\"_new\">http://localhost:34216/1EDA1CB1-F3BF-6338-A64B-AF0F60A998BD/workbook/1EDA1D09-ECCF-6066-BA4C-83098973BDE0/worksheet/1EDA1D09-F4E5-6604-A979-ED5BDD4B4F65</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>0EE1D1BF-A342-FD30-81FC-4D39935DFC3B</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/0EE1D1BF-8B15-FDC0-AE5B-568A5610931A/workbook/0EE1D1BF-A342-FD30-81FC-4D39935DFC3B/worksheet/0EE1D1BF-A797-7390-BA1B-D5EB32750424\" target=\"_blank\">http://localhost:34216/0EE1D1BF-8B15-FDC0-AE5B-568A5610931A/workbook/0EE1D1BF-A342-FD30-81FC-4D39935DFC3B/worksheet/0EE1D1BF-A797-7390-BA1B-D5EB32750424</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -678,24 +712,24 @@
                 "In the examples above, we are both creating items (signals/conditions/scalars/etc) and using them in a template -- all in one call to `spy.push()`.\n",
                 "\n",
                 "If the items are already created, then you can use `spy.workbooks.push()` instead, like so:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 14,
             "id": "34839059",
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Push successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Workbook Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td><td style=\"background-color: #EEFFEE; text-align: left;\">Pushed Workbook ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">URL</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">F01FD57A-1112-4020-9430-CF27C2847D1B agent_api_key Workbook Template Example 2.1</td><td style=\"text-align: left; vertical-align: top;\">Workbook Template Example 2.1</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Analysis</td><td style=\"text-align: right; vertical-align: top;\">20</td><td style=\"vertical-align: top;\">00:00:00.76</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">1EDA1CDC-2487-6A25-B58C-2962223DB919</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/workbook/1EDA1CDC-2487-6A25-B58C-2962223DB919/worksheet/1EDA1CDC-271F-6B34-BC01-7D22A631E4B8\">link</a></td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Push successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Workbook Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td><td style=\"background-color: #EEFFEE; text-align: left;\">Pushed Workbook ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">URL</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">F01FD57A-1112-4020-9430-CF27C2847D1B agent_api_key Workbook Template Example 2.1</td><td style=\"text-align: left; vertical-align: top;\">Workbook Template Example 2.1</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Analysis</td><td style=\"text-align: right; vertical-align: top;\">13</td><td style=\"vertical-align: top;\">00:00:00.66</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">0EE1D1BF-B47C-6010-B11C-23C39D575D9F</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/workbook/0EE1D1BF-B47C-6010-B11C-23C39D575D9F/worksheet/0EE1D1BF-B4C7-FB00-A531-0FCF611E472F\">link</a></td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -735,39 +769,39 @@
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>F01FD57A-1112-4020-9430-CF27C2847D1B agent_api...</td>\n",
                             "      <td>Workbook Template Example 2.1</td>\n",
                             "      <td>Workbook</td>\n",
                             "      <td>Analysis</td>\n",
-                            "      <td>20</td>\n",
-                            "      <td>0:00:00.756971</td>\n",
+                            "      <td>13</td>\n",
+                            "      <td>0:00:00.655838</td>\n",
                             "      <td>Success</td>\n",
-                            "      <td>1EDA1CDC-2487-6A25-B58C-2962223DB919</td>\n",
-                            "      <td>http://localhost:34216/workbook/1EDA1CDC-2487-...</td>\n",
+                            "      <td>0EE1D1BF-B47C-6010-B11C-23C39D575D9F</td>\n",
+                            "      <td>http://localhost:34216/workbook/0EE1D1BF-B47C-...</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                                  ID  \\\n",
                             "0  F01FD57A-1112-4020-9430-CF27C2847D1B agent_api...   \n",
                             "\n",
                             "                            Name      Type Workbook Type Count  \\\n",
-                            "0  Workbook Template Example 2.1  Workbook      Analysis    20   \n",
+                            "0  Workbook Template Example 2.1  Workbook      Analysis    13   \n",
                             "\n",
                             "             Time   Result                    Pushed Workbook ID  \\\n",
-                            "0  0:00:00.756971  Success  1EDA1CDC-2487-6A25-B58C-2962223DB919   \n",
+                            "0  0:00:00.655838  Success  0EE1D1BF-B47C-6010-B11C-23C39D575D9F   \n",
                             "\n",
                             "                                                 URL  \n",
-                            "0  http://localhost:34216/workbook/1EDA1CDC-2487-...  "
+                            "0  http://localhost:34216/workbook/0EE1D1BF-B47C-...  "
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Retrieve Area B items from the Example Data asset tree\n",
                 "area_b_signals = spy.search({'Path': 'Example >> Cooling Tower 1', 'Asset': 'Area B'})\n",
@@ -827,15 +861,15 @@
                 "### A Single Topic Document with Multiple Assets\n",
                 "\n",
                 "In this first example, we will create a single Topic Document that has a separate _section_ for each asset."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 15,
             "id": "fee7f2a6",
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [
@@ -883,17 +917,18 @@
                 "(Note that if you want to exert more precise control over how your section is rendered -- for example, if you want each section to be rendered by a `<tr>` row in a table instead of as separate tables -- you can use the `pretty_print_html=True` argument when you save the workbook templates, and then you can manually go into the saved HTML files and tweak where the Mustache tokens are placed.)\n",
                 "\n",
                 "As you'll see below, we are going to have a block for each asset."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 16,
             "id": "9aa6ea09",
             "metadata": {
+                "keep_output_in_docs": true,
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
@@ -930,17 +965,18 @@
             },
             "source": [
                 "Notice that the parameters code for the document contains an `Assets` entry, and it's a list that includes entries for each of the pieces of embedded content (as well as for the mustache variable `Asset Name`). We will specify a list of entries that are specific to each asset. First we need to create a set of content entries in the form of worksheet templates. Let's look at the code for each worksheet:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 17,
             "id": "9e191078",
             "metadata": {
+                "keep_output_in_docs": true,
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
@@ -957,17 +993,17 @@
                         "}\n",
                         "worksheet.parameters = {\n",
                         "    \"9564A6B8-8A8F-4F6D-AC63-00EA38962B7A [Signal] Area A_Temperature\": None,\n",
                         "    \"DCED9C36-A4BE-4783-9216-DC06B3F57D8C [Signal] Area A_Compressor Power\": None\n",
                         "}\n",
                         "worksheet.parameters = {\n",
                         "    \"8A4F0E26-8A0C-4127-9E11-B67E031C6049 [Signal] Example >> Cooling Tower 1 >> Area A >> Temperature\": None,\n",
-                        "    \"07F3161F-6644-4505-BC33-16D6155B004E [Condition] Hot\": None,\n",
-                        "    \"4B40EAFC-91ED-4AB0-8199-F21AF40A8350 [Asset] Example >> Area A\": None,\n",
-                        "    \"D16FC368-AE8E-47B4-B1A3-9C2A3FBA2BB6 [Asset] Cooling Tower 1\": None\n",
+                        "    \"D16FC368-AE8E-47B4-B1A3-9C2A3FBA2BB6 [Asset] Example >> Cooling Tower 1\": None,\n",
+                        "    \"4B40EAFC-91ED-4AB0-8199-F21AF40A8350 [Asset] Example >> Cooling Tower 1 >> Area A\": None,\n",
+                        "    \"07F3161F-6644-4505-BC33-16D6155B004E [Condition] Hot\": None\n",
                         "}\n",
                         "worksheet.parameters = {\n",
                         "    \"D2C089B6-CE85-46FC-8392-E11CC0C08336 [Signal] Area A_Compressor Stage\": None,\n",
                         "    \"9564A6B8-8A8F-4F6D-AC63-00EA38962B7A [Signal] Area A_Temperature\": None,\n",
                         "    \"DCED9C36-A4BE-4783-9216-DC06B3F57D8C [Signal] Area A_Compressor Power\": None\n",
                         "}\n"
                     ]
@@ -995,15 +1031,15 @@
             },
             "source": [
                 "We're going to create a separate set of worksheets _per asset_. We'll do that by making a copy of each worksheet template in a `for` loop, and we'll store them in a dictionary for later use."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 18,
             "id": "ffb07d6f",
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
@@ -1078,15 +1114,15 @@
             },
             "source": [
                 "Now we will fill in the Organizer Topic document's template parameters by using the worksheet templates that we assembled above. Note below that we are using a [list comprehension](https://www.w3schools.com/python/python_lists_comprehension.asp) to create the `Assets` list of each Waveform asset."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 19,
             "id": "d5ceea8e",
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
@@ -1124,26 +1160,26 @@
             },
             "source": [
                 "Now we do some final bookkeeping to tidy things up and push. Click on the link that corresponds to the Topic to see it in Organizer."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 20,
             "id": "d844ef07",
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Push successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Workbook Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td><td style=\"background-color: #EEFFEE; text-align: left;\">Pushed Workbook ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">URL</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">F01FD57A-1112-4020-9430-CF27C2847D1B agent_api_key Workbook Template Example 3</td><td style=\"text-align: left; vertical-align: top;\">Workbook Template Example 3</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Analysis</td><td style=\"text-align: right; vertical-align: top;\">46</td><td style=\"vertical-align: top;\">00:00:02.25</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">1EDA1D0A-100E-687D-A389-894EB867EF33</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/workbook/1EDA1D0A-100E-687D-A389-894EB867EF33/worksheet/1EDA1D0A-1DF1-6488-B7DF-FBA5925CA34C\">link</a></td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">90931EF8-D80B-4F22-8568-3683DD806D50 agent_api_key Workbook Template Example 3</td><td style=\"text-align: left; vertical-align: top;\">Workbook Template Example 3</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Topic</td><td style=\"text-align: right; vertical-align: top;\">2</td><td style=\"vertical-align: top;\">00:00:00.22</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">1EDA1D0A-120A-658C-99C3-55F9414A0E1F</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/workbook/1EDA1D0A-120A-658C-99C3-55F9414A0E1F/worksheet/1EDA1D0A-2C49-6361-A301-776F7690B645\">link</a></td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Push successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Workbook Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td><td style=\"background-color: #EEFFEE; text-align: left;\">Pushed Workbook ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">URL</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">F01FD57A-1112-4020-9430-CF27C2847D1B agent_api_key Workbook Template Example 3</td><td style=\"text-align: left; vertical-align: top;\">Workbook Template Example 3</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Analysis</td><td style=\"text-align: right; vertical-align: top;\">39</td><td style=\"vertical-align: top;\">00:00:02.24</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">0EE1D1BF-C564-F9E0-B16A-68205AE874B4</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/workbook/0EE1D1BF-C564-F9E0-B16A-68205AE874B4/worksheet/0EE1D1BF-D246-FF50-9102-2D7B87E4B19E\">link</a></td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">90931EF8-D80B-4F22-8568-3683DD806D50 agent_api_key Workbook Template Example 3</td><td style=\"text-align: left; vertical-align: top;\">Workbook Template Example 3</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Topic</td><td style=\"text-align: right; vertical-align: top;\">2</td><td style=\"vertical-align: top;\">00:00:00.81</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">0EE1D1BF-C5C1-6640-BA54-D67542685763</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/workbook/0EE1D1BF-C5C1-6640-BA54-D67542685763/worksheet/0EE1D1BF-E1EF-FBF0-8BD3-7606C245FB41\">link</a></td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -1160,16 +1196,16 @@
                 "# for the user to see the templates. So we set the \"Archived\" property to True -- they\n",
                 "# will still be pushed, but they'll be in the trash and the user won't see them.\n",
                 "analysis.worksheets['Trend Template']['Archived'] = True\n",
                 "analysis.worksheets['XY Plot Template']['Archived'] = True\n",
                 "analysis.worksheets['Treemap Template']['Archived'] = True\n",
                 "analysis.worksheets['Table Template']['Archived'] = True\n",
                 "\n",
-                "# Note that we pass in the list of workbooks (which includes the Analysis and the Topic)\n",
-                "pushed_df = spy.push(metadata=metadata_df, workbook=workbooks)\n",
+                "# Note that we pass in a list that includes the Analysis and the Topic\n",
+                "pushed_df = spy.push(metadata=metadata_df, workbook=[topic, analysis])\n",
                 "\n",
                 "# Show the inner Push Workbooks status object's display instead of the metadata push status,\n",
                 "# since it has links to the Topic.\n",
                 "pushed_df.spy.status.inner['Push Workbooks'].display()"
             ]
         },
         {
@@ -1201,22 +1237,22 @@
                 "Now let's see how it would look if you wanted a separate Topic Document for each Asset instead of putting them all in one Document.\n",
                 "\n",
                 "It looks very similar, but you'll see that we use the `copy()` function to make separate documents."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 21,
             "id": "ca90ef13",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Push successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Workbook Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td><td style=\"background-color: #EEFFEE; text-align: left;\">Pushed Workbook ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">URL</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">F01FD57A-1112-4020-9430-CF27C2847D1B agent_api_key Workbook Template Example 4</td><td style=\"text-align: left; vertical-align: top;\">Workbook Template Example 4</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Analysis</td><td style=\"text-align: right; vertical-align: top;\">46</td><td style=\"vertical-align: top;\">00:00:02.16</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">1EDA1D0A-32D8-6ED9-B199-ADD43C97A0F1</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/workbook/1EDA1D0A-32D8-6ED9-B199-ADD43C97A0F1/worksheet/1EDA1D0A-3B8B-6879-B23E-ABA70A6E4CD8\">link</a></td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">90931EF8-D80B-4F22-8568-3683DD806D50 agent_api_key Workbook Template Example 4</td><td style=\"text-align: left; vertical-align: top;\">Workbook Template Example 4</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Topic</td><td style=\"text-align: right; vertical-align: top;\">6</td><td style=\"vertical-align: top;\">00:00:00.42</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">1EDA1D0A-3549-6EE8-BA31-DDA541931291</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/workbook/1EDA1D0A-3549-6EE8-BA31-DDA541931291/worksheet/1EDA1D0A-50C1-64F7-9329-8726262FBC48\">link</a></td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Push successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Workbook Type</td><td style=\"background-color: #EEFFEE; text-align: left;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td><td style=\"background-color: #EEFFEE; text-align: left;\">Pushed Workbook ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">URL</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">F01FD57A-1112-4020-9430-CF27C2847D1B agent_api_key Workbook Template Example 4</td><td style=\"text-align: left; vertical-align: top;\">Workbook Template Example 4</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Analysis</td><td style=\"text-align: right; vertical-align: top;\">39</td><td style=\"vertical-align: top;\">00:00:01.99</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">0EE1D1BF-EEC5-EE10-B79E-77ADC7F9C1EC</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/workbook/0EE1D1BF-EEC5-EE10-B79E-77ADC7F9C1EC/worksheet/0EE1D1BF-F368-6670-8821-D50CC117A304\">link</a></td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">90931EF8-D80B-4F22-8568-3683DD806D50 agent_api_key Workbook Template Example 4</td><td style=\"text-align: left; vertical-align: top;\">Workbook Template Example 4</td><td style=\"text-align: left; vertical-align: top;\">Workbook</td><td style=\"text-align: left; vertical-align: top;\">Topic</td><td style=\"text-align: right; vertical-align: top;\">6</td><td style=\"vertical-align: top;\">00:00:00.54</td><td style=\"text-align: left; vertical-align: top;\">Success</td><td style=\"text-align: left; vertical-align: top;\">0EE1D1BF-EF22-EA70-B7AE-2A60E1411BE2</td><td style=\"text-align: left; vertical-align: top;\"><a target=\"_blank\" href=\"http://localhost:34216/workbook/0EE1D1BF-EF22-EA70-B7AE-2A60E1411BE2/worksheet/0EE1D1C0-09CF-6440-A80A-F64EE5DA3BF2\">link</a></td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -1259,22 +1295,34 @@
                 "            }\n",
                 "        ]\n",
                 "    }\n",
                 "\n",
                 "# Since we have created a separate document for each asset, we don't want to see the template doc in the Topic\n",
                 "doc_template['Archived'] = True\n",
                 "\n",
-                "pushed_df = spy.push(metadata=metadata_df, workbook=workbooks)\n",
+                "pushed_df = spy.push(metadata=metadata_df, workbook=[topic, analysis])\n",
                 "pushed_df.spy.status.inner['Push Workbooks'].display()"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "d04efadf",
+            "metadata": {},
+            "source": [
+                "### A Topic Document with an Image\n",
+                "\n",
+                "In the examples above, you saw how to use syntax like `{{Asset Name}}` as a placeholder in the template that became a parameter you could specify in your SPy code.\n",
+                "\n",
+                "You can do a similar thing with pictures/images in your document. The most common use for this capability is to push a custom visualization (that you created in Python) into your document, and typically you'll want to do that on a schedule. A separate [Data Lab Visualizations](Data%20Lab%20Visualizations.ipynb) notebook walks you through how to accomplish that."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a3b9d0f1",
+            "id": "8c832832",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -1288,13 +1336,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.8"
+            "version": "3.8.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.acl.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.acl.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.login.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.login.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.pull.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.pull.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.push.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.push.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.search.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.search.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.swap.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.swap.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.widgets.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.widgets.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.workbooks.ipynb` & `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.workbooks.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/docs/_copy.py` & `seeq-spy-189.3/seeq/spy/docs/_copy.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/jobs/_execute.py` & `seeq-spy-189.3/seeq/spy/jobs/_execute.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/jobs/_pull.py` & `seeq-spy-189.3/seeq/spy/jobs/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/jobs/_push.py` & `seeq-spy-189.3/seeq/spy/jobs/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/jobs/_schedule.py` & `seeq-spy-189.3/seeq/spy/jobs/_schedule.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/notifications/_emails.py` & `seeq-spy-189.3/seeq/spy/notifications/_emails.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/utils/__init__.py` & `seeq-spy-189.3/seeq/spy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/widgets/_ipy_utils.py` & `seeq-spy-189.3/seeq/spy/widgets/_ipy_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/widgets/_widgets.py` & `seeq-spy-189.3/seeq/spy/widgets/_widgets.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/__init__.py` & `seeq-spy-189.3/seeq/spy/workbooks/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_annotation.py` & `seeq-spy-189.3/seeq/spy/workbooks/_annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import requests
 from bs4 import BeautifulSoup
 
 from seeq.base.seeq_names import SeeqNames
 from seeq.sdk import *
 from seeq.spy import _common
-from seeq.spy import _login, _metadata
+from seeq.spy import _login
 from seeq.spy._errors import *
 from seeq.spy._redaction import safely, request_safely
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.workbooks import _item, _render
 from seeq.spy.workbooks._content import Content, DateRange, AssetSelection
 from seeq.spy.workbooks._item import Item
@@ -53,19 +53,20 @@
 
     def refresh_from(self, new_item, item_map: ItemMap, status: Status):
         self.annotation_type = new_item.annotation_type
         # Note that we purposefully don't touch the worksheet reference, since it will have stayed the same
         self._set_html(new_item.html)
         self._images = new_item.images
 
-    def _find_image_references(self):
-        if not self.html:
+    @staticmethod
+    def _find_image_references(html):
+        if not html:
             return list()
 
-        matches = re.finditer(r'src="/api(/annotations/(.*?)/images/(.*?))"', self.html)
+        matches = re.finditer(r'src="/api(/annotations/(.*?)/images/(.*?))"', html)
         return [(match.group(1), match.group(2), match.group(3)) for match in matches]
 
     @property
     def html(self):
         return self._html
 
     @html.setter
@@ -174,15 +175,15 @@
             lambda: Item._dict_from_item_output(Item._get_item_output(session, self.id)),
             action_description=f'get properties of Annotation {self.id}',
             status=status)
 
         self._definition = definition
 
         if include_images:
-            image_references = self._find_image_references()
+            image_references = Annotation._find_image_references(self.html)
             for query_params, annotation_id, image_id in image_references:
                 if (annotation_id, image_id) in self.images:
                     continue
 
                 self.worksheet.workbook.update_status('Pulling image', 1)
 
                 api_client_url = session.get_api_url()
@@ -234,24 +235,23 @@
 
         html = self._push_specific(session, item_map, datasource_output, label, new_annotation, relevant_annotation)
 
         # Create an override map for image mapping, which can be different for the same annotation in the case of a
         # template
         images_map = dict()
 
-        # First add a prefix to existing image references in the HTML so that we can handle cases where
+        # We add a prefix to existing image references in the HTML so that we can handle cases where
         # the names that are picked by "POST /annotations/{id}/images" overlap with existing names and would
         # otherwise cause the find & replace that happens later to be non-deterministic
         image_prefix = 'ToBeMapped_'
-        html = re.sub(r'src="(/api/annotations/.*?/images/)(.*?)"', rf'src="\1{image_prefix}\2"', html)
 
         if push_images:
             item_map[f'Images for {self.id}'] = images_map
 
-            for _, annotation_id, image_id in self._find_image_references():
+            for _, annotation_id, image_id in Annotation._find_image_references(html):
                 api_client_url = session.get_api_url()
                 request_url = api_client_url + '/annotations/%s/images' % relevant_annotation.id
 
                 self.worksheet.workbook.update_status('Pushing image', 1)
 
                 response = requests.post(url=request_url,
                                          files={
@@ -274,14 +274,16 @@
                 match = re.match(r'.*?images/(.*)', link_json['link'])
                 new_image_id = match.group(1)
 
                 images_map[f'{image_prefix}{image_id}'] = new_image_id
         else:
             images_map = item_map[f'Images for {self.id}']
 
+        html = re.sub(r'src="(/api/annotations/.*?/images/)(.*?)"', rf'src="\1{image_prefix}\2"', html)
+
         bs = BeautifulSoup(html, features='html.parser')
         find_result = bs.find_all(['p', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'title'])
         name = 'Unnamed'
         description = None
 
         if len(find_result) > 0:
             name = ' '.join(re.split(r'[\s\n]+', find_result[0].get_text().strip())[:20])
@@ -321,24 +323,26 @@
             new_annotation.interests.append(new_interest)
 
         new_annotation.created_by_id = relevant_annotation.created_by.id
         safely(lambda: annotations_api.update_annotation(id=relevant_annotation.id, body=new_annotation),
                action_description=f'update Annotation {relevant_annotation.id}',
                status=status)
 
-        ignored_properties = _metadata.IGNORED_PROPERTIES + [SeeqNames.Properties.background,
-                                                             SeeqNames.Properties.condition_formula_now,
-                                                             SeeqNames.Properties.document]
+        # Annotations have a lot of properties that are managed by Appserver and shouldn't be pushed. We need to push
+        # only a small, curated set that are actually configuration items on the Topic Document.
+        properties_to_push = [SeeqNames.Properties.timezone,
+                              SeeqNames.Properties.is_ck_enabled]
+
         added_or_updated_properties = [ScalarPropertyV1(name=k, value=v)
                                        for k, v in self.definition_dict.items()
-                                       if k not in ignored_properties and v is not None]
+                                       if k in properties_to_push and v is not None]
 
         deleted_properties = [ScalarPropertyV1(name=k, value=v)
                               for k, v in self.definition_dict.items()
-                              if k not in ignored_properties and v is None]
+                              if k in properties_to_push and v is None]
 
         if len(added_or_updated_properties) > 0:
             safely(lambda: items_api.set_properties(id=relevant_annotation.id, body=added_or_updated_properties),
                    action_description=f'set properties for Annotation {relevant_annotation.id}',
                    status=status, additional_errors=[400])
 
         if len(deleted_properties) > 0:
```

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_content.py` & `seeq-spy-189.3/seeq/spy/workbooks/_content.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_data.py` & `seeq-spy-189.3/seeq/spy/workbooks/_data.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_folder.py` & `seeq-spy-189.3/seeq/spy/workbooks/_folder.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_item.py` & `seeq-spy-189.3/seeq/spy/workbooks/_item.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_item_map.py` & `seeq-spy-189.3/seeq/spy/workbooks/_item_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,16 @@
             if _id is None:
                 # This is the case of a Mustachioed annotation with {{variable}} tokens in it
                 continue
 
             if isinstance(value, pd.DataFrame):
                 if len(value) > 1:
                     raise SPyValueError(f'Multiple rows in template_parameters dict for "{key}":\n{value}')
+                if len(value) == 0:
+                    raise SPyValueError(f'Empty DataFrame in template_parameters dict for "{key}"')
                 value = value.iloc[0].to_dict()
             elif isinstance(value, str):
                 value = {'ID': value} if _common.is_guid(value) else {'Name': value}
             elif isinstance(value, spy.workbooks.ItemTemplate):
                 continue
 
             if _common.present(value, 'ID') and not _common.get(value, 'Reference', default=False):
```

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_load.py` & `seeq-spy-189.3/seeq/spy/workbooks/_load.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_mustache.py` & `seeq-spy-189.3/seeq/spy/workbooks/_mustache.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import re
 
 import chevron
+
 from seeq.spy import _common
 
 
 class MustachioedAnnotation:
     """
     Wraps a piece of HTML and exposes any Mustache variables in a way that is useful to the templating system. Also
     facilitates rendering of a template with Mustache variables replaced.
@@ -19,14 +20,16 @@
 
     def __init__(self, html, resolve_content_key_func=None):
         self._html = _common.fix_up_ckeditor_curly_brace_weirdness(html)
 
         if resolve_content_key_func is not None:
             self._html = MustachioedAnnotation._parameterize_seeq_content_ids(self._html, resolve_content_key_func)
 
+        self._html = MustachioedAnnotation._fix_up_images(self._html)
+
         self._validate()
 
     @property
     def html(self):
         return self._html
 
     @property
@@ -39,14 +42,20 @@
 
     @staticmethod
     def _parameterize_seeq_content_ids(html, resolve_content_key_func):
         return re.sub(r'data-seeq-content="([^"]+)"',
                       lambda m: f'data-seeq-content="{{{{{resolve_content_key_func(m.group(1))}}}}}"',
                       html)
 
+    @staticmethod
+    def _fix_up_images(html):
+        return re.sub(r'<img ([^>]*) src="/api/annotations/([^"]+)" alt="\{\W?\{([^}]+)}\W?}">',
+                      r'<img \1 src="{{[Image] \3}}" alt="{{[AltText] \3}}">',
+                      html)
+
     # noinspection PyBroadException
     @staticmethod
     def invalid_mustache_characters():
         invalid_chars = str()
         for i in range(0, 65536):
 
             try:
```

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_pull.py` & `seeq-spy-189.3/seeq/spy/workbooks/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_push.py` & `seeq-spy-189.3/seeq/spy/workbooks/_push.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
                 _common.raise_or_catalog(status, e=e)
 
         if not at_least_one_thing_pushed_this_iteration:
             if status.errors == 'raise':
                 raise SPyRuntimeError('Could not find the following dependencies:\n%s\n'
                                       'Therefore, could not import the following workbooks:\n%s\n' %
                                       ('\n'.join(dependencies_not_found),
-                                       '\n'.join([str(workbook) for workbook in workbooks])))
+                                       '\n'.join([str(workbook) for _, workbook in remaining_workbooks])))
 
             break
 
     Annotation.push_fixups(session, status, item_map)
 
     new_workbooks = None
     if refresh and at_least_one_thing_pushed:
```

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_render.py` & `seeq-spy-189.3/seeq/spy/workbooks/_render.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_report_content_utilities.py` & `seeq-spy-189.3/seeq/spy/workbooks/_report_content_utilities.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_save.py` & `seeq-spy-189.3/seeq/spy/workbooks/_save.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_search.py` & `seeq-spy-189.3/seeq/spy/workbooks/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_template.py` & `seeq-spy-189.3/seeq/spy/workbooks/_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import copy
 import json
+import os
 import re
 from typing import Optional, List, Callable, Union
 
 from seeq.spy import _common
 from seeq.spy._errors import *
 from seeq.spy._session import Session
 from seeq.spy._status import Status
@@ -827,32 +828,56 @@
             return _new_content
 
         parameters = item_map.parameters
 
         if parameters is None:
             parameters = self.worksheet.code_dict()
 
-        parameters_with_content = AnnotationTemplate._walk_dict(parameters, _workstep_to_content)
+        massaged_parameters = AnnotationTemplate._walk_dict(parameters, _workstep_to_content)
 
         html = super()._push_specific(session, item_map, datasource_output, label, new_annotation, existing_annotation,
                                       new_content_dict, status)
 
         item_map[f'Content for {self.id}'] = new_content_dict
 
         def _content_to_id(_key, _val):
             if not isinstance(_val, ContentTemplate):
                 return _val
 
             return item_map[_val.id]
 
-        parameters_with_content_ids = AnnotationTemplate._walk_dict(parameters_with_content, _content_to_id)
+        massaged_parameters = AnnotationTemplate._walk_dict(massaged_parameters, _content_to_id)
+
+        def _image_file_to_img_src(_key, _val):
+            if '[Image]' not in _key:
+                return _val
+
+            if _val is None:
+                raise SPyValueError(f'Template parameter value for "{_key}" is missing. You must supply a filename '
+                                    f'for an image file.')
+
+            if not isinstance(_val, str):
+                raise SPyTypeError(f'Template parameter value for "{_key}" must be a string (the filename of the '
+                                   f'image)')
+
+            if not os.path.exists(_val):
+                raise SPyValueError(f'Image file "{_val}" does not exist (for template parameter "{_key}")')
+
+            _, _image_format = os.path.splitext(_val)
+            _image_name = f'{_common.new_placeholder_guid()}{_image_format.lower()}'
+            with open(_val, 'rb') as _img:
+                self.images[(item_map[self.id], _image_name)] = _img.read()
+
+            return f'/api/annotations/{item_map[self.id]}/images/{_image_name}'
+
+        massaged_parameters = AnnotationTemplate._walk_dict(massaged_parameters, _image_file_to_img_src)
 
         mustache = MustachioedAnnotation(html, lambda content_id: self.resolve_content_code_key(content_id))
 
-        new_html = mustache.render(parameters_with_content_ids)
+        new_html = mustache.render(massaged_parameters)
 
         self._after_push(item_map)
 
         return new_html
 
 
 class DateRangeTemplate(ItemTemplate, DateRange):
```

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_user.py` & `seeq-spy-189.3/seeq/spy/workbooks/_user.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_workbook.py` & `seeq-spy-189.3/seeq/spy/workbooks/_workbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,15 +502,15 @@
                         status=self.status)
 
                 # Now go back through all the worksheets to see if any worksteps weren't resolved
                 for worksheet in self.worksheets:
                     if specific_worksheet_ids is not None and worksheet.id not in specific_worksheet_ids:
                         continue
 
-                    dependencies_not_found.update(worksheet.find_unresolved_worksteps(item_map))
+                    dependencies_not_found.update(worksheet.find_unresolved_worksteps())
 
             if first_worksheet_id is not None:
                 link_url = '%s/%sworkbook/%s/worksheet/%s' % (
                     session.public_url,
                     (folder_id + '/') if folder_id is not None else '',
                     workbook_output.id,
                     first_worksheet_id
```

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_worksheet.py` & `seeq-spy-189.3/seeq/spy/workbooks/_worksheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from seeq.spy.workbooks._item import Item, ItemList
 from seeq.spy.workbooks._item_map import ItemMap
 from seeq.spy.workbooks._workstep import Workstep, AnalysisWorkstep, ExistingWorkstepWalk
 
 
 class Worksheet(Item):
     _annotation: Union[Journal, Report]
+    _item_map_for_push: Optional[ItemMap]
 
     def __new__(cls, *args, **kwargs):
         if cls is Worksheet:
             raise SPyTypeError("Worksheet may not be instantiated directly, create either AnalysisWorksheet or "
                                "TopicWorksheet")
 
         return object.__new__(cls)
@@ -125,14 +126,16 @@
         pass
 
     def item_map_worksteps_key(self):
         return f'Worksteps for {self.id}'
 
     def push(self, session: Session, pushed_workbook_id, item_map, datasource_output, existing_worksheet_identifiers,
              include_inventory, include_annotations, label=None, status: Status = None):
+        self._item_map_for_push = item_map
+
         existing_worksheet_id = None
 
         # After Integrated Security was introduced, we can no longer search for Worksheets using Data ID,
         # so we use the passed-in dictionary that the Workbook assembled to find existing worksheets.
         # So we call this "SPy ID" even though it's just the Data ID we would have used if searching was still
         # supported. Why not still use Data ID? Because with the introduction of templates, it's much easier to
         # choose a label that causes a conflicting Data ID in some other workbook, and it's really hard to make the
@@ -183,20 +186,20 @@
     @property
     def referenced_worksteps(self):
         return self._annotation.referenced_worksteps
 
     def find_workbook_links(self, session: Session, status: Status):
         return self._annotation.find_workbook_links(session, status)
 
-    def find_unresolved_worksteps(self, item_map: ItemMap):
+    def find_unresolved_worksteps(self):
         # Unresolved Report workstep dependencies will be found when pushing the associated document
         dependencies_not_found = set()
-        for workstep_tuple in self._annotation.find_workstep_references(item_map=item_map):
+        for workstep_tuple in self._annotation.find_workstep_references(item_map=self._item_map_for_push):
             referenced_workbook_id, referenced_worksheet_id, referenced_workstep_id = workstep_tuple
-            if referenced_workstep_id not in item_map:
+            if referenced_workstep_id not in self._item_map_for_push:
                 dependencies_not_found.add(
                     'Workbook %s, Worksheet %s, Workstep %s' % (
                         referenced_workbook_id, referenced_worksheet_id, referenced_workstep_id))
         return dependencies_not_found
 
     def current_workstep(self) -> AnalysisWorkstep:
         return self.worksteps[self.definition['Current Workstep ID']]
```

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/_workstep.py` & `seeq-spy-189.3/seeq/spy/workbooks/_workstep.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq/spy/workbooks/app.css` & `seeq-spy-189.3/seeq/spy/workbooks/app.css`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.0/seeq_spy.egg-info/PKG-INFO` & `seeq-spy-189.3/seeq_spy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 189.0
+Version: 189.3
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-189.0/seeq_spy.egg-info/SOURCES.txt` & `seeq-spy-189.3/seeq_spy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 README.md
 setup.py
 seeq/base/__init__.py
 seeq/base/proputil.py
 seeq/base/seeq_names.py
 seeq/base/system.py
 seeq/base/util.py
-seeq/scripts/create_monitoring_alerts.py
-seeq/scripts/create_monitoring_workbook.py
 seeq/spy/__init__.py
 seeq/spy/_common.py
 seeq/spy/_config.py
 seeq/spy/_datalab.py
 seeq/spy/_errors.py
 seeq/spy/_login.py
 seeq/spy/_metadata.py
@@ -55,14 +53,15 @@
 seeq/spy/docs/__init__.py
 seeq/spy/docs/_copy.py
 seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
 seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
 seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
 seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
 seeq/spy/docs/Documentation/Command Reference.ipynb
+seeq/spy/docs/Documentation/Data Lab Visualizations.ipynb
 seeq/spy/docs/Documentation/Tutorial.ipynb
 seeq/spy/docs/Documentation/Version Considerations.ipynb
 seeq/spy/docs/Documentation/Workbook Templates.ipynb
 seeq/spy/docs/Documentation/spy.acl.ipynb
 seeq/spy/docs/Documentation/spy.jobs.ipynb
 seeq/spy/docs/Documentation/spy.login.ipynb
 seeq/spy/docs/Documentation/spy.pull.ipynb
```

### Comparing `seeq-spy-189.0/setup.py` & `seeq-spy-189.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq-spy",
-    version="189.0",
+    version="189.3",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="Easy-to-use Python interface for Seeq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```


# Comparing `tmp/impsparc-2.0.2.tar.gz` & `tmp/impsparc-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impsparc-2.0.2.tar", last modified: Mon Apr 17 16:25:04 2023, max compression
+gzip compressed data, was "impsparc-3.0.1.tar", last modified: Thu Jul 13 03:50:08 2023, max compression
```

## Comparing `impsparc-2.0.2.tar` & `impsparc-3.0.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.560164 impsparc-2.0.2/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1064 2023-04-06 04:16:23.000000 impsparc-2.0.2/LICENSE.md
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      244 2023-04-06 04:16:23.000000 impsparc-2.0.2/MANIFEST.in
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-17 16:25:04.559888 impsparc-2.0.2/PKG-INFO
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      626 2023-04-06 04:18:27.000000 impsparc-2.0.2/README.md
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.338197 impsparc-2.0.2/cvsvc_apirisk/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/__init__.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.357154 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   363678 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   262350 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      615 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      753 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23616 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16394 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16378 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.358863 impsparc-2.0.2/cvsvc_apirisk/score/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2914 2023-04-17 14:42:16.000000 impsparc-2.0.2/cvsvc_apirisk/score/base.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.370710 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       80 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59992 2023-04-17 15:04:42.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1503 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.424161 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2433 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2453 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2662 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2684 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2697 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2117 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2387 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2385 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2393 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2391 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2722 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2731 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.472904 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2346 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2474 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2477 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2459 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2462 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2760 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3371 2023-04-17 15:04:03.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/json_line.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.488972 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2084 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2418 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2339 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2867 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2292 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2163 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     5713 2023-04-17 16:21:41.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2685 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2635 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2479 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2769 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.490411 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.333743 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.537608 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.544739 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15291 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16918 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15192 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    28781 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11370 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1363 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11350 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11421 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      966 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.556058 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      423 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16193 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      209 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3581 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3478 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3944 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      309 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      406 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6482 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     9574 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1212 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    88994 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.493009 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.330965 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.500709 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   207965 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      687 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      756 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2033 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.505305 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59219 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   195090 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4023 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    56178 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.513775 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   100782 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   163872 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    80388 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11245 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      393 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.530448 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   181852 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   105536 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60520 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23940 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   388460 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   154228 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    10556 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4960 2023-04-06 04:16:23.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6244 2023-04-17 15:01:30.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_common.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3358 2023-04-17 14:46:48.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    27120 2023-04-17 15:02:48.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main_cr.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    14646 2023-04-17 15:02:09.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_spec_util.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1192 2023-04-17 15:03:29.000000 impsparc-2.0.2/cvsvc_apirisk/score/spec_security/yaml_line.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-04-17 16:25:04.559378 impsparc-2.0.2/impsparc.egg-info/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/PKG-INFO
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6777 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/SOURCES.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        1 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/dependency_links.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      164 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/entry_points.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      185 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/requires.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       14 2023-04-17 16:25:04.000000 impsparc-2.0.2/impsparc.egg-info/top_level.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       38 2023-04-17 16:25:04.560245 impsparc-2.0.2/setup.cfg
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1196 2023-04-17 14:30:26.000000 impsparc-2.0.2/setup.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.686656 impsparc-3.0.1/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1064 2023-07-12 16:38:34.000000 impsparc-3.0.1/LICENSE.md
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      244 2023-07-12 16:38:34.000000 impsparc-3.0.1/MANIFEST.in
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-07-13 03:50:08.686089 impsparc-3.0.1/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      626 2023-07-12 16:38:34.000000 impsparc-3.0.1/README.md
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.506711 impsparc-3.0.1/cvsvc_apirisk/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/__init__.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.514406 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   363678 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   262350 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      615 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      753 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23616 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16394 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16378 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.516132 impsparc-3.0.1/cvsvc_apirisk/score/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2891 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/base.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.524904 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       80 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60355 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1503 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.538238 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2433 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2453 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2662 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2684 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2697 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2117 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2387 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2385 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2393 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2391 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2722 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2731 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.567279 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2346 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2474 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2477 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2459 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2462 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2760 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3371 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/json_line.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.593632 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2084 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2418 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2339 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2867 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2292 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2163 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     5713 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2685 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2635 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2479 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2769 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.595843 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.503202 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.658957 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.664183 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15291 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16918 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15192 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    28781 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11370 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1363 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11350 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11421 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      966 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.677845 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      423 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16193 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      209 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3581 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3478 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3944 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      309 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      406 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6482 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     9574 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1212 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    88994 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.598041 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.501251 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.607617 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   207965 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      687 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      756 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2033 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.616453 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59219 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   195090 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4023 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    56178 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.641064 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   100782 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   163872 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    80388 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11245 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      393 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.653216 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   181852 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   105536 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60520 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23940 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   388460 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   154228 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    10556 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4960 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6250 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_common.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3384 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_main.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    27565 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_main_cr.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15731 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_spec_util.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1192 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/yaml_line.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.685021 impsparc-3.0.1/impsparc.egg-info/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6777 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/SOURCES.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        1 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/dependency_links.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      164 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/entry_points.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      213 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/requires.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       14 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/top_level.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       38 2023-07-13 03:50:08.686845 impsparc-3.0.1/setup.cfg
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1245 2023-07-13 03:34:45.000000 impsparc-3.0.1/setup.py
```

### Comparing `impsparc-2.0.2/LICENSE.md` & `impsparc-3.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/PKG-INFO` & `impsparc-3.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 2.0.2
+Version: 3.0.1
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ImpSpARC
-
 API Specification Analysis for Risks and Compliance
 
 ImpSpARC is a tool that will analyse API Specification for Security Risks and Compliance violations.
 
-API Specification captures the design of an API and is an integral part of API development process. The design of an API is captured in various formats such as Swagger, OpenAPI, RAML, etc.
+API Specification captures the design of an API and is an integral part of API development process. The design of an API is captured in various formats such as Swagger, OpenAPI, RAML, etc. 
 
 ImpSpARC analyses API specifications written in Swagger or OpenAPI format against the security best practices and then provides an assessment score and severity. The ImpSpARC tool also provides a language to codfiy your custom Risk and Compliance voilation rules too.
```

### Comparing `impsparc-2.0.2/README.md` & `impsparc-3.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # ImpSpARC
-
 API Specification Analysis for Risks and Compliance
 
 ImpSpARC is a tool that will analyse API Specification for Security Risks and Compliance violations.
 
-API Specification captures the design of an API and is an integral part of API development process. The design of an API is captured in various formats such as Swagger, OpenAPI, RAML, etc.
+API Specification captures the design of an API and is an integral part of API development process. The design of an API is captured in various formats such as Swagger, OpenAPI, RAML, etc. 
 
 ImpSpARC analyses API specifications written in Swagger or OpenAPI format against the security best practices and then provides an assessment score and severity. The ImpSpARC tool also provides a language to codfiy your custom Risk and Compliance voilation rules too.
```

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf` & `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf` & `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json` & `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt` & `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip` & `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json` & `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json` & `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/base.py` & `impsparc-3.0.1/cvsvc_apirisk/score/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         -------
         result: int
             Result desc
         """
         self.score = None
         self.meta = None
         self.children = {}      # If empty, means leaf node
-        self.score = 0
 
         return
 
     def __repr__(self):
         """
         Description
```

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,22 @@
             else:
                 raise ValueError('Incorrect input file. Should be JSON/YAML.')
 
             # ipdb.set_trace()
 
             # Check whether OpenAPI v2 or v3
             if 'swagger' in raw_spec:
+                report['files'][abs_path]['basePath'] = raw_spec.get('basePath', [])
+                #basepath = raw_spec['basepath']
                 openapi_ver = 'v2'
             elif 'openapi' in raw_spec:
+                if raw_spec.get('servers', []):
+                    report['files'][abs_path]['url'] = raw_spec.get('servers', [])[0].get('url', [])
+                else:
+                    report['files'][abs_path]['url'] = []
                 openapi_ver = 'v3'
             else:
                 raise ValueError('Incorrect specification format')
 
             target_obj['raw_spec'] = raw_spec
             spec_main_cr = \
                 SpecSecCustomRulesMain(target_obj=target_obj,
```

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/json_line.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/json_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_common.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,7 +229,13 @@
                 line_num = cvlrange_ds[-1]['cvlrange26uel7Ao'][0]
 
         linenum_idstr = '[%d]' % line_num
     except:
         linenum_idstr = ''
 
     return linenum_idstr
+
+
+
+
+
+
```

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         except ParseError:
             # Try again because prance's __parse_json() gets messed up because
             # of six.text_type(). Provide it a string rather than dict
             parse = ResolvingParser(spec_string=json.dumps(self.target_obj['raw_spec']),
                                     content_type='application/json', recursion_limit_handler=reclimit_handler)
 
         self.target_obj['spec_obj'] = parse.specification
-        self.qspec = QuerySpec(spec_obj=self.target_obj['spec_obj'])
+        self.qspec = QuerySpec(spec_obj=self.target_obj['spec_obj'], openapi_ver =openapi_ver)
 
         self.add_child(SpecSecSecurityAttr07(self.qspec, openapi_ver))
 
     def __repr__(self):
         """
         Description
```

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_main_cr.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_main_cr.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,14 +258,23 @@
         -------
         result: int
             Result desc
         """
         identifier = node  # .replace('->', '.')
         # ipdb.set_trace()
 
+        if '->' in str(node):
+            new_node, _ = node.rsplit('->', 1)
+            node_present = self.spec_main.qspec.G.hasNode(self.spec_main.qspec.node_id_mapping.get(
+                    new_node, self.spec_main.qspec.total_node_plus_ten))
+            if node_present:
+                node_val = self.spec_main.qspec.get_node_value(new_node)
+                if node_val == 'circular_ref':
+                    return '(False == True)'
+
         if condition in {'<', '>', '<=', '>=', '==', '!='}:
             try:
                 if str(node).lower() in {'true', 'false'}:
                     id_value = node
                 else:
                     id_value = int(self.spec_main.qspec.get_node_value(node))
                     value = int(value)
```

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/sps_spec_util.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_spec_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 PATH_OPS_v2 = ['get', 'put', 'post', 'delete', 'options', 'head', 'patch']
 
 
 class QuerySpec(object):
 
-    def __init__(self, spec_obj):
+    def __init__(self, spec_obj, openapi_ver):
         """
         Description
 
         Params
         ------
         p1 : float
             Param description
@@ -28,14 +28,15 @@
         result: int
             Result desc
         """
         self.ROOT_NODE = '#'
         self.spec_obj = spec_obj
         self.G = nk.Graph(directed=True)
         self.node_id_mapping = dict()
+        self.openapi_ver = openapi_ver
 
         node_name_sp = self.G.attachNodeAttribute('nodenamesp', str)
         node_name_raw = self.G.attachNodeAttribute('nodenameraw', str)
         child_type = self.G.attachNodeAttribute('childtype', str)
 
         self.node_attributes = {'node_name_sp': node_name_sp,
                                 'node_name_raw': node_name_raw,
@@ -93,22 +94,34 @@
         node_names = []
         data_types = {}
         for node in self.G.iterNodes():
             if self.node_attributes['node_name_raw'][node] == 'parameters':
                 for param_obj_node in self.G.iterNeighbors(node):
                     node_names.append(self.node_attributes['node_name_sp'][param_obj_node])
                     for param_list in self.G.iterNeighbors(param_obj_node):
-                        if self.node_attributes['node_name_raw'][param_list] == 'type':
-                            for _type in self.G.iterNeighbors(param_list):
-                                param_type = self.node_attributes['node_name_sp'][_type]
-                                p_type = param_type.split('->')[-1]
-                                if p_type in data_types:
-                                    data_types[p_type] = data_types[p_type] + 1
-                                else:
-                                    data_types[p_type] = 1
+                        if self.openapi_ver == 'v3':
+                            if self.node_attributes['node_name_raw'][param_list] == 'schema':
+                                for _type in self.G.iterNeighbors(param_list):
+                                    if self.node_attributes['node_name_raw'][_type] == 'type':
+                                        for param_type_o3 in self.G.iterNeighbors(_type):
+                                            param_type = self.node_attributes['node_name_sp'][param_type_o3]
+                                            p_type = param_type.split('->')[-1]
+                                            if p_type in data_types:
+                                                data_types[p_type] = data_types[p_type] + 1
+                                            else:
+                                                data_types[p_type] = 1
+                        elif self.openapi_ver == 'v2':
+                            if self.node_attributes['node_name_raw'][param_list] == 'type':
+                                for _type in self.G.iterNeighbors(param_list):
+                                    param_type = self.node_attributes['node_name_sp'][_type]
+                                    p_type = param_type.split('->')[-1]
+                                    if p_type in data_types:
+                                        data_types[p_type] = data_types[p_type] + 1
+                                    else:
+                                        data_types[p_type] = 1
         return node_names, data_types
 
     def get_op_objs_list(self):
         method_set = set()
         methods = self.get_op_objs()
         for method in methods:
             method_set.add(method.split('->')[-1])
@@ -121,14 +134,15 @@
             if nodename in self.get_op_objs_list():
                 if nodename in node_names:
                     node_names[nodename] = node_names[nodename] + 1
                 else:
                     node_names[nodename] = 1
         return node_names
 
+
     def get_header_objs(self):
         """
         Description
 
         Params
         ------
         p1 : float
@@ -340,17 +354,17 @@
             Result desc
         """
         node_names = []
         paths_node = '%s->paths' % self.ROOT_NODE
         if self.G.hasNode(self.node_id_mapping.get(paths_node, self.total_node_plus_ten)):
             for pathitem_node in self.G.iterNeighbors(self.node_id_mapping[paths_node]):
                 for op in PATH_OPS_v2:
-                    op_node = '%s->%s' % (pathitem_node, op)
+                    op_node = '%s->%s' % (self.node_attributes['node_name_sp'][pathitem_node], op)
                     if self.G.hasNode(self.node_id_mapping.get(op_node, self.total_node_plus_ten)):
-                        node_names.append(self.node_attributes['node_name_sp'][op_node])
+                        node_names.append(op_node)
 
         return node_names
 
     def get_keyword_objs(self, keyword):
         """
         Description
 
@@ -392,14 +406,16 @@
         Returns
         -------
         result: int
             Result desc
         """
 
         def helper(created_graph, previous_node, attr_name_sp_val, obj):
+            if obj == {}:
+                obj = 'circular_ref'
 
             if type(obj) in {str, int, float}:
                 # Add the value
                 attr_name_sp_val_curr_node = '%s->%s' % (attr_name_sp_val, obj)
                 curr_node = created_graph.addNode()
                 created_graph.addEdge(previous_node, curr_node)
                 self.node_attributes['node_name_sp'][curr_node] = attr_name_sp_val_curr_node
```

### Comparing `impsparc-2.0.2/cvsvc_apirisk/score/spec_security/yaml_line.py` & `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/yaml_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/impsparc.egg-info/PKG-INFO` & `impsparc-3.0.1/impsparc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 2.0.2
+Version: 3.0.1
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ImpSpARC
-
 API Specification Analysis for Risks and Compliance
 
 ImpSpARC is a tool that will analyse API Specification for Security Risks and Compliance violations.
 
-API Specification captures the design of an API and is an integral part of API development process. The design of an API is captured in various formats such as Swagger, OpenAPI, RAML, etc.
+API Specification captures the design of an API and is an integral part of API development process. The design of an API is captured in various formats such as Swagger, OpenAPI, RAML, etc. 
 
 ImpSpARC analyses API specifications written in Swagger or OpenAPI format against the security best practices and then provides an assessment score and severity. The ImpSpARC tool also provides a language to codfiy your custom Risk and Compliance voilation rules too.
```

### Comparing `impsparc-2.0.2/impsparc.egg-info/SOURCES.txt` & `impsparc-3.0.1/impsparc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impsparc-2.0.2/setup.py` & `impsparc-3.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impsparc",
-    version=os.environ.get("VER", "2.0.2"),
+    version=os.environ.get("VER", "3.0.1"),
     author="Priyank Chheda",
     author_email="priyank.chheda@imperva.com",
     description="API Specification Analysis for Risks and Compliance",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
@@ -31,10 +31,12 @@
         "numpy==1.22.3",
         "networkit==10.1",
         "parsimonious==0.8.1",
         "sanic==20.3.0",
         "jinja2==3.0.3",
         "idna==2.10",
         "PyYAML==6.0",
+        "psutil==5.9.2",
+        "pandas==2.0.0"
     ],
     include_package_data=True,
 )
```


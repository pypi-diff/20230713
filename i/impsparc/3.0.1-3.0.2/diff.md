# Comparing `tmp/impsparc-3.0.1.tar.gz` & `tmp/impsparc-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impsparc-3.0.1.tar", last modified: Thu Jul 13 03:50:08 2023, max compression
+gzip compressed data, was "impsparc-3.0.2.tar", last modified: Thu Jul 13 13:23:19 2023, max compression
```

## Comparing `impsparc-3.0.1.tar` & `impsparc-3.0.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.686656 impsparc-3.0.1/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1064 2023-07-12 16:38:34.000000 impsparc-3.0.1/LICENSE.md
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      244 2023-07-12 16:38:34.000000 impsparc-3.0.1/MANIFEST.in
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-07-13 03:50:08.686089 impsparc-3.0.1/PKG-INFO
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      626 2023-07-12 16:38:34.000000 impsparc-3.0.1/README.md
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.506711 impsparc-3.0.1/cvsvc_apirisk/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/__init__.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.514406 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   363678 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   262350 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      615 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      753 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23616 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16394 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16378 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.516132 impsparc-3.0.1/cvsvc_apirisk/score/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2891 2023-07-12 16:38:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/base.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.524904 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       80 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60355 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1503 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.538238 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2433 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2453 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2662 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2684 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2697 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2117 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2387 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2385 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2393 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2391 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2722 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2731 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.567279 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2346 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2474 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2477 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2459 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2462 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2760 2023-07-13 03:31:33.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3371 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/json_line.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.593632 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2084 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2418 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2339 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2867 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2292 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2163 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     5713 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2685 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2635 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2479 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2769 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.595843 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.503202 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.658957 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.664183 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15291 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16918 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15192 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    28781 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11370 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1363 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11350 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11421 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      966 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.677845 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      423 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16193 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      209 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3581 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3478 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3944 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      309 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      406 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6482 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     9574 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1212 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    88994 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.598041 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.501251 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.607617 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   207965 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      687 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      756 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2033 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.616453 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59219 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   195090 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4023 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    56178 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.641064 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   100782 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   163872 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    80388 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11245 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      393 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.653216 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   181852 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   105536 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60520 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23940 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   388460 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   154228 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    10556 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4960 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6250 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_common.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3384 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_main.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    27565 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_main_cr.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15731 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_spec_util.py
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1192 2023-07-13 03:31:34.000000 impsparc-3.0.1/cvsvc_apirisk/score/spec_security/yaml_line.py
-drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:50:08.685021 impsparc-3.0.1/impsparc.egg-info/
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/PKG-INFO
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6777 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/SOURCES.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        1 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/dependency_links.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      164 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/entry_points.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      213 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/requires.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       14 2023-07-13 03:50:08.000000 impsparc-3.0.1/impsparc.egg-info/top_level.txt
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       38 2023-07-13 03:50:08.686845 impsparc-3.0.1/setup.cfg
--rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1245 2023-07-13 03:34:45.000000 impsparc-3.0.1/setup.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:19.087147 impsparc-3.0.2/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1064 2023-07-12 16:38:34.000000 impsparc-3.0.2/LICENSE.md
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      244 2023-07-12 16:38:34.000000 impsparc-3.0.2/MANIFEST.in
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-07-13 13:23:19.086096 impsparc-3.0.2/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      626 2023-07-12 16:38:34.000000 impsparc-3.0.2/README.md
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:18.877759 impsparc-3.0.2/cvsvc_apirisk/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-12 16:38:34.000000 impsparc-3.0.2/cvsvc_apirisk/__init__.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:18.888491 impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   363678 2023-07-12 16:38:34.000000 impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   262350 2023-07-12 16:38:34.000000 impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      615 2023-07-12 16:38:34.000000 impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      753 2023-07-12 16:38:34.000000 impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23616 2023-07-12 16:38:34.000000 impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16394 2023-07-12 16:38:34.000000 impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16378 2023-07-12 16:38:34.000000 impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:18.889796 impsparc-3.0.2/cvsvc_apirisk/score/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-12 16:38:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2891 2023-07-12 16:38:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/base.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:18.900044 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       80 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60355 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1503 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:18.920712 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2433 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2453 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2662 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2684 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2697 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2117 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2387 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2385 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2393 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2391 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2722 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2731 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:18.934983 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2346 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2474 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2477 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2459 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2462 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2760 2023-07-13 03:31:33.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3371 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/json_line.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:18.957591 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2084 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2418 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2339 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2867 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2292 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2163 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     5930 2023-07-13 03:54:10.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2685 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2635 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2479 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2769 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:18.959733 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:18.873410 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:19.059728 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:19.065975 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15291 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16918 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15192 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    28781 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11370 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1363 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11350 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11421 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      966 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:19.079454 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      423 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    16193 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      209 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3581 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3478 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3944 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      309 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      406 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6482 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     9574 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1212 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    88994 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:18.964434 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:18.871074 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:19.005082 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   207965 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      687 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      756 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     2033 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:19.013872 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    59219 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   195090 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4023 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    56178 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:19.025629 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   100782 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   163872 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    80388 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    11245 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      393 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:19.047132 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   181852 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   105536 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    60520 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    23940 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   388460 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967   154228 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    10556 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     4960 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6250 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sps_common.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     3384 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sps_main.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    28279 2023-07-13 03:52:09.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sps_main_cr.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967    15731 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sps_spec_util.py
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1192 2023-07-13 03:31:34.000000 impsparc-3.0.2/cvsvc_apirisk/score/spec_security/yaml_line.py
+drwxr-xr-x   0 nainika.aggarwal (1389333189) 347102967        0 2023-07-13 13:23:19.084465 impsparc-3.0.2/impsparc.egg-info/
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      985 2023-07-13 13:23:18.000000 impsparc-3.0.2/impsparc.egg-info/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     6777 2023-07-13 13:23:18.000000 impsparc-3.0.2/impsparc.egg-info/SOURCES.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967        1 2023-07-13 13:23:18.000000 impsparc-3.0.2/impsparc.egg-info/dependency_links.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      164 2023-07-13 13:23:18.000000 impsparc-3.0.2/impsparc.egg-info/entry_points.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967      213 2023-07-13 13:23:18.000000 impsparc-3.0.2/impsparc.egg-info/requires.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       14 2023-07-13 13:23:18.000000 impsparc-3.0.2/impsparc.egg-info/top_level.txt
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967       38 2023-07-13 13:23:19.087309 impsparc-3.0.2/setup.cfg
+-rw-r--r--   0 nainika.aggarwal (1389333189) 347102967     1245 2023-07-13 13:23:15.000000 impsparc-3.0.2/setup.py
```

### Comparing `impsparc-3.0.1/LICENSE.md` & `impsparc-3.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/PKG-INFO` & `impsparc-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 3.0.1
+Version: 3.0.2
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impsparc-3.0.1/README.md` & `impsparc-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf` & `impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf` & `impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json` & `impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt` & `impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip` & `impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json` & `impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json` & `impsparc-3.0.2/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/base.py` & `impsparc-3.0.2/cvsvc_apirisk/score/base.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/json_line.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/json_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,16 @@
 
                             if not self.qspec.G.hasNode(
                                     self.qspec.node_id_mapping.get(target_node, self.qspec.total_node_plus_ten)):
                                 # v = self.fix_template.copy()
                                 # v['entity'] = scope_node
                                 # v['score'] = self.attr_wt
                                 # meta.append(v['entity'])
-                                meta.append(scope_node)
+                                meta_node = '%s->%s->%s->%s' % (security_node, self.qspec.node_attributes['node_name_raw'][security_idx_node], secschm_name, self.qspec.node_attributes['node_name_raw'][scope_node_idx])
+                                meta.append(meta_node)
 
         self.score = self.attr_wt * int(len(meta) > 0)
         if len(meta) > 0:
             self.meta = meta
 
     def compute_openapiv3(self):
         """
```

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_common.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sps_common.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_main.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sps_main.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_main_cr.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sps_main_cr.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,15 @@
 
         if key_enabled:
             nodes = list(map(lambda n: n + '__key__', nodes))
 
         # [] for pernode_raw_rule which is applicable only for nested rule
         return nodes, []
 
-    def check_embd_rule(self, rule):
+    def check_embd_rule(self, rule, abs_path):
         """
         Description
 
         Params
         ------
         p1 : float
             Param description
@@ -407,15 +407,32 @@
         if len(rule) == 1:
             identifier, condition, value = rule[0].split(' ')
             if condition == 'embedded-run':
                 # It is an embedded rule
                 self.spec_main.children[identifier].compute()
                 meta = self.spec_main.children[identifier].meta
 
-                return True, (meta is not None), meta
+                raw_rule = []
+                for meta_data in meta:
+                    line_num = parse_cvlrange(
+                        self.linenum_mapping,
+                        meta_data,
+                        abs_path=abs_path)
+
+                    int_line_num = None
+                    if line_num not in {'', None}:
+                        int_line_num = json.loads(line_num)
+                        int_line_num = int_line_num[0]
+
+                    intm_raw_rule = {'reference_path': meta_data}
+                    if int_line_num is not None:
+                        intm_raw_rule['element_line_num'] = [int_line_num]
+
+                    raw_rule.append(intm_raw_rule)
+                return True, (meta is not None), raw_rule
 
         # In every other case, return False
         return False, None, None
 
     def analyze_rule(self, rule_dict, list_node_outcomes=False, abs_path=None):
         """
         Description
@@ -432,15 +449,15 @@
         result: int
             Result desc
         """
         rule = rule_dict['rule_flt']
 
         # ipdb.set_trace()
         # Check if the rule is hard-coded
-        ran_embdr, has_violation, violating_rules = self.check_embd_rule(rule)
+        ran_embdr, has_violation, violating_rules = self.check_embd_rule(rule, abs_path)
         if ran_embdr:
             # Return False because the check_embd_rule() will add the
             # violation to meta
 
             return has_violation, violating_rules, None, None
 
         self.sanity_check(rule)
```

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/sps_spec_util.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/sps_spec_util.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/cvsvc_apirisk/score/spec_security/yaml_line.py` & `impsparc-3.0.2/cvsvc_apirisk/score/spec_security/yaml_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/impsparc.egg-info/PKG-INFO` & `impsparc-3.0.2/impsparc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 3.0.1
+Version: 3.0.2
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impsparc-3.0.1/impsparc.egg-info/SOURCES.txt` & `impsparc-3.0.2/impsparc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impsparc-3.0.1/setup.py` & `impsparc-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impsparc",
-    version=os.environ.get("VER", "3.0.1"),
+    version=os.environ.get("VER", "3.0.2"),
     author="Priyank Chheda",
     author_email="priyank.chheda@imperva.com",
     description="API Specification Analysis for Risks and Compliance",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```


# Comparing `tmp/nibabies-23.0.0.tar.gz` & `tmp/nibabies-23.1.0rc0.tar.gz`

## Comparing `nibabies-23.0.0.tar` & `nibabies-23.1.0rc0.tar`

### file list

```diff
@@ -1,128 +1,140 @@
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nibabies-23.0.0/.dockerignore
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nibabies-23.0.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 nibabies-23.0.0/.gitattributes
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 nibabies-23.0.0/.mailmap
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nibabies-23.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 nibabies-23.0.0/.readthedocs.yml
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 nibabies-23.0.0/.zenodo.json
--rw-r--r--   0        0        0    10589 2020-02-02 00:00:00.000000 nibabies-23.0.0/CHANGES.md
--rw-r--r--   0        0        0    10562 2020-02-02 00:00:00.000000 nibabies-23.0.0/Dockerfile
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 nibabies-23.0.0/Makefile
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 nibabies-23.0.0/README.md
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 nibabies-23.0.0/get_version.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 nibabies-23.0.0/.circleci/bcp_anat_outputs.txt
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 nibabies-23.0.0/.circleci/bcp_full_outputs.txt
--rw-r--r--   0        0        0    24156 2020-02-02 00:00:00.000000 nibabies-23.0.0/.circleci/config.yml
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 nibabies-23.0.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nibabies-23.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 nibabies-23.0.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nibabies-23.0.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 nibabies-23.0.0/.github/workflows/style.yml
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 nibabies-23.0.0/.maint/contributors.json
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nibabies-23.0.0/.maint/developers.json
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 nibabies-23.0.0/.maint/former.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 nibabies-23.0.0/.maint/update_changes.sh
--rwxr-xr-x   0        0        0     4572 2020-02-02 00:00:00.000000 nibabies-23.0.0/.maint/update_zenodo.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nibabies-23.0.0/docker/files/nipype.cfg
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/Makefile
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/community.md
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/conf.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/faqs.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/index.md
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/installation.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/make.bat
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/outputs.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/usage.md
--rw-r--r--   0        0        0   956500 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/_static/nibabies_anat.png
--rw-r--r--   0        0        0   879274 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/_static/nibabies_func.png
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 nibabies-23.0.0/docs/sphinxext/github_link.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/__about__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/_version.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/_warnings.py
--rw-r--r--   0        0        0    27414 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/config.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/cli/__init__.py
--rw-r--r--   0        0        0    28638 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/cli/parser.py
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/cli/run.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/cli/version.py
--rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/cli/workflow.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/FreeSurferLabelRemappings.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/FreeSurferSubcorticalLabelTableLut.txt
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/MNIInfant_to_MNI1526NLinAsym.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/antsBrainExtraction_precise.json
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/antsBrainExtraction_testing.json
--rw-r--r--   0        0        0    18142 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/boilerplate.bib
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/itkIdentityTransform.txt
--rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/reports-spec.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/sub-01_run-01_echo-1_bold.nii.gz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/sub-01_run-01_echo-2_bold.nii.gz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/sub-01_run-01_echo-3_bold.nii.gz
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/t1_to_bold.json
--rw-r--r--   0        0        0   383806 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/tpl-MNI152NLin6Asym_res-01_desc-avgwmparc_dseg.nii.gz
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/within_subject_t1t2.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/flirtsch/bbr.sch
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/data/tests/config.toml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/interfaces/__init__.py
--rw-r--r--   0        0        0    14860 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/interfaces/confounds.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/interfaces/freesurfer.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/interfaces/gifti.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/interfaces/maths.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/interfaces/multiecho.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/interfaces/nibabel.py
--rw-r--r--   0        0        0    13075 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/interfaces/reports.py
--rw-r--r--   0        0        0    48773 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/interfaces/workbench.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/interfaces/tests/__init__.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/interfaces/tests/test_nibabel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/reports/__init__.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/reports/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/tests/__init__.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/tests/test_config.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/tests/data/labelfile.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/utils/__init__.py
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/utils/bids.py
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/utils/confounds.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/utils/filtering.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/utils/misc.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/utils/patches.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/utils/telemetry.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/utils/validation.py
--rw-r--r--   0        0        0    36909 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/utils/viz.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/__init__.py
--rw-r--r--   0        0        0    18973 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/base.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/anatomical/__init__.py
--rw-r--r--   0        0        0    15681 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/anatomical/base.py
--rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/anatomical/brain_extraction.py
--rw-r--r--   0        0        0    10097 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/anatomical/norm.py
--rw-r--r--   0        0        0    25466 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/anatomical/outputs.py
--rw-r--r--   0        0        0     8142 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/anatomical/preproc.py
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/anatomical/registration.py
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/anatomical/segmentation.py
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/anatomical/surfaces.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/bold/__init__.py
--rw-r--r--   0        0        0    12562 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/bold/alignment.py
--rw-r--r--   0        0        0    51289 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/bold/base.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/bold/boldref.py
--rw-r--r--   0        0        0    33877 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/bold/confounds.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/bold/hmc.py
--rw-r--r--   0        0        0    34971 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/bold/outputs.py
--rw-r--r--   0        0        0    35715 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/bold/registration.py
--rw-r--r--   0        0        0    30348 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/bold/resampling.py
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/bold/stc.py
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 nibabies-23.0.0/nibabies/workflows/bold/t2s.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 nibabies-23.0.0/scripts/anatprep.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 nibabies-23.0.0/scripts/bold_subcortical.py
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 nibabies-23.0.0/scripts/check_outputs.py
--rwxr-xr-x   0        0        0     3440 2020-02-02 00:00:00.000000 nibabies-23.0.0/scripts/fetch_templates.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 nibabies-23.0.0/wrapper/LICENSE
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nibabies-23.0.0/wrapper/README.rst
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 nibabies-23.0.0/wrapper/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.0.0/wrapper/src/nibabies_wrapper/__init__.py
--rwxr-xr-x   0        0        0    24722 2020-02-02 00:00:00.000000 nibabies-23.0.0/wrapper/src/nibabies_wrapper/__main__.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nibabies-23.0.0/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 nibabies-23.0.0/LICENSE
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 nibabies-23.0.0/long_description.md
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 nibabies-23.0.0/pyproject.toml
--rw-r--r--   0        0        0    18123 2020-02-02 00:00:00.000000 nibabies-23.0.0/PKG-INFO
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.dockerignore
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.gitattributes
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.mailmap
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.readthedocs.yml
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.zenodo.json
+-rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/CHANGES.md
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/Dockerfile
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/Makefile
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/README.md
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/env.yml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/get_version.py
+-rw-r--r--   0        0        0     5495 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/requirements.txt
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.circleci/bcp_anat_outputs.txt
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.circleci/bcp_full_outputs.txt
+-rw-r--r--   0        0        0    22712 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.circleci/config.yml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.github/workflows/style.yml
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.maint/contributors.json
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.maint/developers.json
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.maint/former.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.maint/update_changes.sh
+-rwxr-xr-x   0        0        0     4572 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.maint/update_zenodo.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docker/files/nipype.cfg
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/Makefile
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/community.md
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/conf.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/faqs.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/index.md
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/installation.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/make.bat
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/outputs.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/requirements.txt
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/usage.md
+-rw-r--r--   0        0        0   956500 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/_static/nibabies_anat.png
+-rw-r--r--   0        0        0   879274 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/_static/nibabies_func.png
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/docs/sphinxext/github_link.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/__about__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/__init__.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/_version.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/_warnings.py
+-rw-r--r--   0        0        0    26259 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/config.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/cli/__init__.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/cli/mcribs.py
+-rw-r--r--   0        0        0    30374 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/cli/parser.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/cli/run.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/cli/version.py
+-rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/cli/workflow.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/FreeSurferLabelRemappings.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/FreeSurferSubcorticalLabelTableLut.txt
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/MNIInfant_to_MNI1526NLinAsym.mat
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/antsBrainExtraction_precise.json
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/antsBrainExtraction_testing.json
+-rw-r--r--   0        0        0    18747 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/boilerplate.bib
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/itkIdentityTransform.txt
+-rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/reports-spec.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/sub-01_run-01_echo-1_bold.nii.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/sub-01_run-01_echo-2_bold.nii.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/sub-01_run-01_echo-3_bold.nii.gz
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/t1_to_bold.json
+-rw-r--r--   0        0        0   383806 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/tpl-MNI152NLin6Asym_res-01_desc-avgwmparc_dseg.nii.gz
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/within_subject_t1t2.json
+-rw-r--r--   0        0        0   717536 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/atlases/dHCP/dHCP.week42.L.sphere.surf.gii
+-rw-r--r--   0        0        0   705029 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/atlases/dHCP/dHCP.week42.R.sphere.surf.gii
+-rw-r--r--   0        0        0  1062593 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/atlases/mcribs/lh.sphere.reg.dHCP42.surf.gii
+-rw-r--r--   0        0        0   848371 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/atlases/mcribs/lh.sphere.reg2.surf.gii
+-rw-r--r--   0        0        0  1062290 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/atlases/mcribs/rh.sphere.reg.dHCP42.surf.gii
+-rw-r--r--   0        0        0   848372 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/atlases/mcribs/rh.sphere.reg2.surf.gii
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/flirtsch/bbr.sch
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/data/tests/config.toml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/__init__.py
+-rw-r--r--   0        0        0    14860 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/confounds.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/freesurfer.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/gifti.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/maths.py
+-rw-r--r--   0        0        0    10269 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/mcribs.py
+-rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/metric.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/multiecho.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/nibabel.py
+-rw-r--r--   0        0        0    13075 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/reports.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/utils.py
+-rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/workbench.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/tests/__init__.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/interfaces/tests/test_nibabel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/reports/__init__.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/reports/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/tests/__init__.py
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/tests/test_config.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/tests/data/labelfile.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/utils/__init__.py
+-rw-r--r--   0        0        0    11369 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/utils/bids.py
+-rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/utils/confounds.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/utils/filtering.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/utils/misc.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/utils/telemetry.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/utils/validation.py
+-rw-r--r--   0        0        0    36909 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/utils/viz.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/__init__.py
+-rw-r--r--   0        0        0    22175 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/base.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/anatomical/__init__.py
+-rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/anatomical/base.py
+-rw-r--r--   0        0        0    10738 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/anatomical/brain_extraction.py
+-rw-r--r--   0        0        0    28329 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/anatomical/outputs.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/anatomical/preproc.py
+-rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/anatomical/registration.py
+-rw-r--r--   0        0        0     9949 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/anatomical/resampling.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/anatomical/segmentation.py
+-rw-r--r--   0        0        0    19105 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/anatomical/surfaces.py
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/anatomical/template.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/bold/__init__.py
+-rw-r--r--   0        0        0    12562 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/bold/alignment.py
+-rw-r--r--   0        0        0    52970 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/bold/base.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/bold/boldref.py
+-rw-r--r--   0        0        0    33877 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/bold/confounds.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/bold/hmc.py
+-rw-r--r--   0        0        0    35951 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/bold/outputs.py
+-rw-r--r--   0        0        0    35715 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/bold/registration.py
+-rw-r--r--   0        0        0    46798 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/bold/resampling.py
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/bold/stc.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/nibabies/workflows/bold/t2s.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/scripts/anatprep.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/scripts/bold_subcortical.py
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/scripts/check_outputs.py
+-rwxr-xr-x   0        0        0     3562 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/scripts/fetch_templates.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/wrapper/LICENSE
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/wrapper/README.rst
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/wrapper/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/wrapper/src/nibabies_wrapper/__init__.py
+-rwxr-xr-x   0        0        0    24722 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/wrapper/src/nibabies_wrapper/__main__.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/LICENSE
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/long_description.md
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 nibabies-23.1.0rc0/PKG-INFO
```

### Comparing `nibabies-23.0.0/.zenodo.json` & `nibabies-23.1.0rc0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/CHANGES.md` & `nibabies-23.1.0rc0/CHANGES.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+23.1.0 (TBD)
+============
+The next minor release of *NiBabies*, this release includes a number of new goodies, including:
+
+### New surface reconstruction option
+M-CRIB-S (Adamson et al., https://www.nature.com/articles/s41598-020-61326-2), has shown to improve performance in participants under 9 months. If you would like to try this method, add the following to your command: `--surface-recon-method mcribs`.
+
+Note: Currently, a pre-computed segmentation derivative must be provided to run mcribs.
+
+### Improved batch processing
+*NiBabies* now automatically parses the BIDS directory for participant ages, first searching in the
+participant's `session.tsv`, and falling back to `participants.tsv`. This simplifies batch submissions including multiple subjects & sessions. As a result, the `--age-months` flag has been deprecated, and will be removed in a later release.
+
+### Goodvoxels projection
+An option to determine and exclude high-variance voxels from being projected to the surface when creating CIFTI files. To enable this, add `--project-goodvoxels` to your command.
+
+
+## Full Changelog
+  * CI: Purge codecov python package (#282)
+  * DKR: Upgrade Docker base, c3d (#275)
+  * DKR: Add M-CRIB-S to Docker container (#283)
+  * DKR: Update dependencies, split into multi-stage build
+  * ENH: Add option to exclude projecting high variance voxels to surface (#278)
+  * ENH: Resample morphometrics to fsLR CIFTI-2 files when outputing CIFTIs (#279)
+  * ENH: Add MCRIBReconAll as alternative surface reconstruction method (#283)
+  * ENH: Reorder anatomical processsing, run ANTs DenoiseImage on anatomicals (#286)
+  * ENH: Extract participant ages from BIDS sources, deprecate `--age-months` (#287)
+  * ENH: Dilate BOLD mask by 2 voxels to prevent over-aggressive masking degrading T2star map estimation (#296)
+  * FIX: Improve free memory estimation (#284)
+  * FIX: Ensure age is extracted from sessions file (#291)
+  * FIX: Restore CIFTI medial wall masking, subcortical volume LAS reorientation (#298)
+  * FIX: Recify "goodvoxels" surface projection (#301)
+  * MAINT: Drop TemplateFlowSelect patches (#290)
+
 23.0.0 (January 23, 2023)
 =========================
 New year, new *NiBabies* minor series!
 Some of the highlights of this release include:
 - New run-wise BOLD reference generation, prioritizing single-band references if available, unless avoided with the `--ignore sbrefs` flag.
 - New output: Preprocessed T2w in T1w space.
```

### Comparing `nibabies-23.0.0/Dockerfile` & `nibabies-23.1.0rc0/Dockerfile`

 * *Files 25% similar despite different names*

```diff
@@ -1,292 +1,281 @@
-# Build wheel separately
+# NiBabies Docker Container Image distribution
+#
+# MIT License
+#
+# Copyright (c) 2023 The NiPreps Developers
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+# Ubuntu 22.04 LTS - Jammy
+ARG BASE_IMAGE=ubuntu:jammy-20230605
+
+# NiBabies wheel
 FROM python:slim AS src
 RUN pip install build
 RUN apt-get update && \
     apt-get install -y --no-install-recommends git
 COPY . /src/nibabies
 RUN python -m build /src/nibabies
 
-# Ubuntu 20.04 LTS
-FROM ubuntu:focal-20221130
+# Older Python to support legacy MCRIBS
+FROM python:3.6.15-slim as pyenv
+RUN pip install --no-cache-dir numpy nibabel scipy pandas numexpr contextlib2 \
+    && cp /usr/lib/x86_64-linux-gnu/libffi.so.7* /usr/local/lib
+
+# Intermediate step with utilities for downloading packages
+FROM ${BASE_IMAGE} as downloader
+RUN apt-get update && \
+    apt-get install -y --no-install-recommends \
+                    binutils \
+                    bzip2 \
+                    ca-certificates \
+                    curl \
+                    unzip && \
+    apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
+
+# AFNI
+FROM downloader as afni
+# The download link can point to newer releases
+# As a safeguard, take advantage of Docker caching, and
+# Bump the date to current to update AFNI
+RUN echo "2023.06.09"
+RUN mkdir -p /opt/afni-latest \
+    && curl -fsSL --retry 5 https://afni.nimh.nih.gov/pub/dist/tgz/linux_openmp_64.tgz \
+    | tar -xz -C /opt/afni-latest --strip-components 1 \
+    --exclude "linux_openmp_64/*.gz" \
+    --exclude "linux_openmp_64/funstuff" \
+    --exclude "linux_openmp_64/shiny" \
+    --exclude "linux_openmp_64/afnipy" \
+    --exclude "linux_openmp_64/lib/RetroTS" \
+    --exclude "linux_openmp_64/lib_RetroTS" \
+    --exclude "linux_openmp_64/meica.libs" \
+    # Keep only what we use
+    && find /opt/afni-latest -type f -not \( \
+        -name "3dTshift" -or \
+        -name "3dUnifize" -or \
+        -name "3dAutomask" -or \
+        -name "3dvolreg" \) -delete
+
+# ANTs 2.4.4
+FROM downloader as ants
+RUN mkdir -p /opt && \
+    curl -sSLO "https://github.com/ANTsX/ANTs/releases/download/v2.4.4/ants-2.4.4-ubuntu-22.04-X64-gcc.zip" && \
+    unzip ants-2.4.4-ubuntu-22.04-X64-gcc.zip -d /opt && \
+    rm ants-2.4.4-ubuntu-22.04-X64-gcc.zip
+
+# Connectome Workbench 1.5.0
+FROM downloader as workbench
+RUN mkdir /opt/workbench && \
+    curl -sSLO https://www.humanconnectome.org/storage/app/media/workbench/workbench-linux64-v1.5.0.zip && \
+    unzip workbench-linux64-v1.5.0.zip -d /opt && \
+    rm workbench-linux64-v1.5.0.zip && \
+    rm -rf /opt/workbench/libs_linux64_software_opengl /opt/workbench/plugins_linux64 && \
+    strip --remove-section=.note.ABI-tag /opt/workbench/libs_linux64/libQt5Core.so.5
+
+# Micromamba
+FROM downloader as micromamba
+WORKDIR /
+# Bump the date to current to force update micromamba
+RUN echo "2023.06.29"
+RUN curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba
+ENV MAMBA_ROOT_PREFIX="/opt/conda"
+COPY env.yml /tmp/env.yml
+RUN micromamba create -y -f /tmp/env.yml && \
+    micromamba clean -y -a
+ENV PATH="/opt/conda/envs/nibabies/bin:$PATH"
+RUN /opt/conda/envs/nibabies/bin/npm install -g svgo@^2.8 bids-validator@1.11.0 && \
+    rm -r ~/.npm
+COPY requirements.txt /tmp/requirements.txt
+RUN /opt/conda/envs/nibabies/bin/pip install --no-cache-dir -r /tmp/requirements.txt
+
+# Main container
+FROM ${BASE_IMAGE} as nibabies
 ENV DEBIAN_FRONTEND="noninteractive" \
     LANG="en_US.UTF-8" \
     LC_ALL="en_US.UTF-8"
 
 # Prepare environment
 RUN apt-get update && \
     apt-get install -y --no-install-recommends \
                     apt-utils \
-                    autoconf \
                     build-essential \
-                    bzip2 \
                     ca-certificates \
                     curl \
                     git \
-                    graphviz \
+                    gnupg \
                     libtool \
                     locales \
                     lsb-release \
-                    pandoc \
-                    pandoc-citeproc \
-                    pkg-config \
+                    netbase \
                     unzip \
-                    xvfb && \
-    curl -sSL https://deb.nodesource.com/setup_14.x | bash - && \
-    apt-get install -y --no-install-recommends \
-                    nodejs && \
+                    xvfb \
+                    # MCRIBS-required
+                    libboost-dev \
+                    libeigen3-dev \
+                    libflann-dev \
+                    libgl1-mesa-dev \
+                    libglu1-mesa-dev \
+                    libssl-dev \
+                    libxt-dev \
+                    zlib1g-dev && \
     locale-gen en_US.UTF-8 && \
     apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
 
-# Installing ANTs 2.3.4 (NeuroDocker build)
-ENV ANTSPATH="/usr/lib/ants" \
-    PATH="/usr/lib/ants:$PATH"
-WORKDIR $ANTSPATH
-RUN curl -sSL "https://dl.dropbox.com/s/gwf51ykkk5bifyj/ants-Linux-centos6_x86_64-v2.3.4.tar.gz" \
-    | tar -xzC $ANTSPATH --strip-components 1
+# Configure PPAs for libpng12 and libxp6
+RUN GNUPGHOME=/tmp gpg --keyserver hkps://keyserver.ubuntu.com --no-default-keyring --keyring /usr/share/keyrings/linuxuprising.gpg --recv 0xEA8CACC073C3DB2A \
+    && GNUPGHOME=/tmp gpg --keyserver hkps://keyserver.ubuntu.com --no-default-keyring --keyring /usr/share/keyrings/zeehio.gpg --recv 0xA1301338A3A48C4A \
+    && echo "deb [signed-by=/usr/share/keyrings/linuxuprising.gpg] https://ppa.launchpadcontent.net/linuxuprising/libpng12/ubuntu jammy main" > /etc/apt/sources.list.d/linuxuprising.list \
+    && echo "deb [signed-by=/usr/share/keyrings/zeehio.gpg] https://ppa.launchpadcontent.net/zeehio/libxp/ubuntu jammy main" > /etc/apt/sources.list.d/zeehio.list
 
-# # AFNI latest (neurodocker build)
+# Dependencies for AFNI; requires a discontinued multiarch-support package from bionic (18.04)
 RUN apt-get update -qq \
     && apt-get install -y -q --no-install-recommends \
            ed \
            gsl-bin \
            libglib2.0-0 \
            libglu1-mesa-dev \
            libglw1-mesa \
            libgomp1 \
            libjpeg62 \
+           libpng12-0 \
            libxm4 \
+           libxp6 \
            netpbm \
            tcsh \
            xfonts-base \
            xvfb \
-    && apt-get clean \
-    && rm -rf /var/lib/apt/lists/* \
     && curl -sSL --retry 5 -o /tmp/multiarch.deb http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/multiarch-support_2.27-3ubuntu1.5_amd64.deb \
     && dpkg -i /tmp/multiarch.deb \
     && rm /tmp/multiarch.deb \
-    && curl -sSL --retry 5 -o /tmp/libxp6.deb http://mirrors.kernel.org/debian/pool/main/libx/libxp/libxp6_1.0.2-2_amd64.deb \
-    && dpkg -i /tmp/libxp6.deb \
-    && rm /tmp/libxp6.deb \
-    && curl -sSL --retry 5 -o /tmp/libpng.deb http://snapshot.debian.org/archive/debian-security/20160113T213056Z/pool/updates/main/libp/libpng/libpng12-0_1.2.49-1%2Bdeb7u2_amd64.deb \
-    && dpkg -i /tmp/libpng.deb \
-    && rm /tmp/libpng.deb \
     && apt-get install -f \
-    && apt-get clean \
-    && rm -rf /var/lib/apt/lists/* \
+    && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* \
     && gsl2_path="$(find / -name 'libgsl.so.19' || printf '')" \
     && if [ -n "$gsl2_path" ]; then \
          ln -sfv "$gsl2_path" "$(dirname $gsl2_path)/libgsl.so.0"; \
     fi \
-    && ldconfig \
-    && echo "Downloading AFNI ..." \
-    && mkdir -p /opt/afni-latest \
-    && curl -fsSL --retry 5 https://afni.nimh.nih.gov/pub/dist/tgz/linux_openmp_64.tgz \
-    | tar -xz -C /opt/afni-latest --strip-components 1 \
-    --exclude "linux_openmp_64/*.gz" \
-    --exclude "linux_openmp_64/funstuff" \
-    --exclude "linux_openmp_64/shiny" \
-    --exclude "linux_openmp_64/afnipy" \
-    --exclude "linux_openmp_64/lib/RetroTS" \
-    --exclude "linux_openmp_64/meica.libs" \
-    # Keep only what we use
-    && find /opt/afni-latest -type f -not \( \
-        -name "3dTshift" -or \
-        -name "3dUnifize" -or \
-        -name "3dAutomask" -or \
-        -name "3dvolreg" \) -delete
+    && ldconfig
+
+COPY --from=afni /opt/afni-latest /opt/afni-latest
+COPY --from=ants /opt/ants-2.4.4 /opt/ants
+COPY --from=workbench /opt/workbench /opt/workbench
+
+# AFNI config
 ENV PATH="/opt/afni-latest:$PATH" \
     AFNI_IMSAVE_WARNINGS="NO" \
     AFNI_PLUGINPATH="/opt/afni-latest"
 
-# Install AFNI latest (neurodocker build)
-ENV AFNI_DIR="/opt/afni"
-RUN echo "Downloading AFNI ..." \
-    && mkdir -p ${AFNI_DIR} \
-    && curl -fsSL --retry 5 https://afni.nimh.nih.gov/pub/dist/tgz/linux_openmp_64.tgz \
-       | tar -xz -C ${AFNI_DIR} --strip-components 1 \
-    # Keep only what we use
-    && find ${AFNI_DIR} -type f -not \( \
-        -name "3dTshift" -or \
-        -name "3dUnifize" -or \
-        -name "3dAutomask" -or \
-        -name "3dvolreg" \) -delete
-
-# Convert3D (neurodocker build)
-RUN echo "Downloading Convert3D ..." \
-    && mkdir -p /opt/convert3d-1.0.0 \
-    && curl -fsSL --retry 5 https://sourceforge.net/projects/c3d/files/c3d/1.0.0/c3d-1.0.0-Linux-x86_64.tar.gz/download \
-    | tar -xz -C /opt/convert3d-1.0.0 --strip-components 1 \
-    --exclude "c3d-1.0.0-Linux-x86_64/lib" \
-    --exclude "c3d-1.0.0-Linux-x86_64/share" \
-    --exclude "c3d-1.0.0-Linux-x86_64/bin/c3d_gui"
-ENV C3DPATH="/opt/convert3d-1.0.0" \
-    PATH="/opt/convert3d-1.0.0/bin:$PATH"
+# ANTs config
+ENV ANTSPATH="/opt/ants" \
+    PATH="/opt/ants/bin:$PATH" \
+    LD_LIBRARY_PATH="/opt/ants/lib:$LD_LIBRARY_PATH"
 
-# FSL 6.0.5.1
-RUN apt-get update -qq \
-    && apt-get install -y -q --no-install-recommends \
-           bc \
-           dc \
-           file \
-           libfontconfig1 \
-           libfreetype6 \
-           libgl1-mesa-dev \
-           libgl1-mesa-dri \
-           libglu1-mesa-dev \
-           libgomp1 \
-           libice6 \
-           libxcursor1 \
-           libxft2 \
-           libxinerama1 \
-           libxrandr2 \
-           libxrender1 \
-           libxt6 \
-           sudo \
-           wget \
-    && apt-get clean \
-    && rm -rf /var/lib/apt/lists/* \
-    && echo "Downloading FSL ..." \
-    && mkdir -p /opt/fsl \
-    && curl -fsSL --retry 5 https://fsl.fmrib.ox.ac.uk/fsldownloads/fsl-6.0.5.1-centos7_64.tar.gz \
-    | tar -xz -C /opt/fsl --strip-components 1 \
-    --exclude "fsl/config" \
-    --exclude "fsl/data/atlases" \
-    --exclude "fsl/data/first" \
-    --exclude "fsl/data/mist" \
-    --exclude "fsl/data/possum" \
-    --exclude "fsl/data/standard/bianca" \
-    --exclude "fsl/data/standard/tissuepriors" \
-    --exclude "fsl/doc" \
-    --exclude "fsl/etc/default_flobs.flobs" \
-    --exclude "fsl/etc/fslconf" \
-    --exclude "fsl/etc/js" \
-    --exclude "fsl/etc/luts" \
-    --exclude "fsl/etc/matlab" \
-    --exclude "fsl/extras" \
-    --exclude "fsl/include" \
-    --exclude "fsl/python" \
-    --exclude "fsl/refdoc" \
-    --exclude "fsl/src" \
-    --exclude "fsl/tcl" \
-    --exclude "fsl/bin/FSLeyes" \
-    && find /opt/fsl/bin -type f -not \( \
-        -name "applywarp" -or \
-        -name "bet" -or \
-        -name "bet2" -or \
-        -name "convert_xfm" -or \
-        -name "fast" -or \
-        -name "flirt" -or \
-        -name "fsl_regfilt" -or \
-        -name "fslhd" -or \
-        -name "fslinfo" -or \
-        -name "fslmaths" -or \
-        -name "fslmerge" -or \
-        -name "fslroi" -or \
-        -name "fslsplit" -or \
-        -name "fslstats" -or \
-        -name "imtest" -or \
-        -name "mcflirt" -or \
-        -name "melodic" -or \
-        -name "prelude" -or \
-        -name "remove_ext" -or \
-        -name "susan" -or \
-        -name "topup" -or \
-        -name "zeropad" \) -delete \
-    && find /opt/fsl/data/standard -type f -not -name "MNI152_T1_2mm_brain.nii.gz" -delete
-ENV FSLDIR="/opt/fsl" \
-    PATH="/opt/fsl/bin:$PATH" \
-    FSLOUTPUTTYPE="NIFTI_GZ" \
-    FSLMULTIFILEQUIT="TRUE" \
-    FSLLOCKDIR="" \
-    FSLMACHINELIST="" \
-    FSLREMOTECALL="" \
-    FSLGECUDAQ="cuda.q" \
-    LD_LIBRARY_PATH="/opt/fsl/lib:$LD_LIBRARY_PATH"
+# Workbench config
+ENV PATH="/opt/workbench/bin_linux64:$PATH" \
+    LD_LIBRARY_PATH="/opt/workbench/lib_linux64:$LD_LIBRARY_PATH"
 
-# Install FreeSurfer
+# Install FreeSurfer (with Infant Module)
 COPY --from=nipreps/freesurfer@sha256:3b895fc732a7080374a15c4f976510f39c0c48dc76c030ab27316febd5e419ee /opt/freesurfer /opt/freesurfer
 ENV FREESURFER_HOME="/opt/freesurfer"
 ENV SUBJECTS_DIR="$FREESURFER_HOME/subjects" \
     FUNCTIONALS_DIR="$FREESURFER_HOME/sessions" \
     MNI_DIR="$FREESURFER_HOME/mni" \
     LOCAL_DIR="$FREESURFER_HOME/local" \
     MINC_BIN_DIR="$FREESURFER_HOME/mni/bin" \
     MINC_LIB_DIR="$FREESURFER_HOME/mni/lib" \
     MNI_DATAPATH="$FREESURFER_HOME/mni/data" \
-    FSL_DIR=${FSLDIR}
+    FSL_DIR=${FSLDIR} \
+    FREESURFER="/opt/freesurfer"
 ENV PERL5LIB="$MINC_LIB_DIR/perl5/5.8.5" \
     MNI_PERL5LIB="$MINC_LIB_DIR/perl5/5.8.5" \
     PATH="$FREESURFER_HOME/bin:$FREESURFER_HOME/tktools:$MINC_BIN_DIR:$PATH"
 
-# Workbench
-WORKDIR /opt
-RUN curl -sSLO https://www.humanconnectome.org/storage/app/media/workbench/workbench-linux64-v1.5.0.zip && \
-    unzip workbench-linux64-v1.5.0.zip && \
-    rm workbench-linux64-v1.5.0.zip && \
-    rm -rf /opt/workbench/libs_linux64_software_opengl /opt/workbench/plugins_linux64 && \
-    strip --remove-section=.note.ABI-tag /opt/workbench/libs_linux64/libQt5Core.so.5
-    # ABI tags can interfere when running on Singularity/Apptainer
-ENV PATH="/opt/workbench/bin_linux64:$PATH" \
-    LD_LIBRARY_PATH="/opt/workbench/lib_linux64:$LD_LIBRARY_PATH"
-
-# Installing SVGO and bids-validator
-RUN npm install -g svgo@^2.3 bids-validator@1.9.9 \
-  && rm -rf ~/.npm ~/.empty /root/.npm
-
-# ICA AROMA
-WORKDIR /opt/ICA-AROMA
-RUN curl -sSL "https://github.com/oesteban/ICA-AROMA/archive/v0.4.5.tar.gz" \
-  | tar -xzC /opt/ICA-AROMA --strip-components 1 && \
-  chmod +x /opt/ICA-AROMA/ICA_AROMA.py
-ENV PATH="/opt/ICA-AROMA:$PATH" \
-    AROMA_VERSION="0.4.5"
+# MCRIBS (required legacy python)
+COPY --from=nipreps/mcribs@sha256:6c7a8dedd61d0ead8c7c4a57ab158928c1c1d787d87dae33ab7ee43226fb1e0f /opt/MCRIBS/ /opt/MCRIBS
+COPY --from=pyenv /usr/local/lib/ /usr/local/lib/
+ENV PATH="/opt/MCRIBS/bin:/opt/MCRIBS/MIRTK/MIRTK-install/bin:/opt/MCRIBS/MIRTK/MIRTK-install/lib/tools:${PATH}" \
+    LD_LIBRARY_PATH="/opt/MCRIBS/lib:/opt/MCRIBS/ITK/ITK-install/lib:/opt/MCRIBS/VTK/VTK-install/lib:/opt/MCRIBS/MIRTK/MIRTK-install/lib:/usr/local/lib:${LD_LIBRARY_PATH}" \
+    MCRIBS_HOME="/opt/MCRIBS" \
+    PYTHONPATH="/opt/MCRIBS/lib/python:$PYTHONPATH"
 
 # Create a shared $HOME directory
-RUN useradd -m -s /bin/bash -G users nibabies
+RUN useradd -m -s /bin/bash -G users nibabies && chmod -R 777 /home/nibabies
 WORKDIR /home/nibabies
-ENV HOME="/home/nibabies"
-
-# py39_2209.01
-COPY --from=nipreps/miniconda@sha256:8894ca17e3c8ba963812a6876093463eab6b88871bcfe23f71ebc84cf38451db /opt/conda /opt/conda
+ENV HOME="/home/nibabies" \
+    LD_LIBRARY_PATH="/usr/lib/x86_64-linux-gnu:${LD_LIBRARY_PATH}"
 
-RUN ln -s /opt/conda/etc/profile.d/conda.sh /etc/profile.d/conda.sh && \
-    echo ". /opt/conda/etc/profile.d/conda.sh" >> ~/.bashrc && \
-    echo "conda activate base" >> ~/.bashrc
-
-# Set CPATH for packages relying on compiled libs (e.g. indexed_gzip)
-ENV PATH="/opt/conda/bin:$PATH" \
-    CPATH="/opt/conda/include:$CPATH" \
+COPY --from=micromamba /bin/micromamba /bin/micromamba
+COPY --from=micromamba /opt/conda/envs/nibabies /opt/conda/envs/nibabies
+ENV MAMBA_ROOT_PREFIX="/opt/conda"
+RUN micromamba shell init -s bash && \
+    echo "micromamba activate nibabies" >> $HOME/.bashrc
+ENV PATH="/opt/conda/envs/nibabies/bin:$PATH" \
+    CPATH="/opt/conda/envs/nibabies/include:$CPATH" \
+    LD_LIBRARY_PATH="/opt/conda/envs/nibabies/lib:$LD_LIBRARY_PATH" \
+    CONDA_PYTHON="/opt/conda/envs/nibabies/bin/python"
+
+# FSL environment
+ENV LANG="C.UTF-8" \
+    LC_ALL="C.UTF-8" \
     PYTHONNOUSERSITE=1 \
-    MKL_NUM_THREADS=1 \
+    FSLDIR="/opt/conda/envs/nibabies" \
+    FSLOUTPUTTYPE="NIFTI_GZ" \
+    FSLMULTIFILEQUIT="TRUE" \
+    FSLLOCKDIR="" \
+    FSLMACHINELIST="" \
+    FSLREMOTECALL="" \
+    FSLGECUDAQ="cuda.q"
+
+# Unless otherwise specified each process should only use one thread - nipype
+# will handle parallelization
+ENV MKL_NUM_THREADS=1 \
     OMP_NUM_THREADS=1 \
-    IS_DOCKER_8395080871=1 \
-    CONDA_PYTHON="/opt/conda/bin/python"
+    IS_DOCKER_8395080871=1
 
 # Precaching atlases
 COPY scripts/fetch_templates.py fetch_templates.py
-RUN ${CONDA_PYTHON} -m pip install --no-cache-dir templateflow && \
+RUN ${CONDA_PYTHON} -m pip install --no-cache-dir --upgrade templateflow && \
     ${CONDA_PYTHON} fetch_templates.py && \
     rm fetch_templates.py && \
     find $HOME/.cache/templateflow -type d -exec chmod go=u {} + && \
     find $HOME/.cache/templateflow -type f -exec chmod go=u {} +
 
 # Install pre-built wheel
 COPY --from=src /src/nibabies/dist/*.whl .
-RUN ${CONDA_PYTHON} -m pip install --no-cache-dir $( ls *.whl )[all]
+RUN ${CONDA_PYTHON} -m pip install --no-cache-dir $( ls *.whl )[telemetry,test]
+
+# Facilitate Apptainer use
+RUN find $HOME -type d -exec chmod go=u {} + && \
+    find $HOME -type f -exec chmod go=u {} + && \
+    rm -rf $HOME/.npm $HOME/.conda $HOME/.empty && \
+    ldconfig
 
-# Final settings
-RUN ldconfig
 WORKDIR /tmp
 ARG BUILD_DATE
 ARG VCS_REF
 ARG VERSION
 LABEL org.label-schema.build-date=$BUILD_DATE \
-      org.label-schema.name="nibabies" \
+      org.label-schema.name="NiBabies" \
       org.label-schema.description="NiBabies - NeuroImaging tools for babies" \
       org.label-schema.url="https://github.com/nipreps/nibabies" \
       org.label-schema.vcs-ref=$VCS_REF \
       org.label-schema.vcs-url="https://github.com/nipreps/nibabies" \
       org.label-schema.version=$VERSION \
       org.label-schema.schema-version="1.0"
 
-ENTRYPOINT ["/opt/conda/bin/nibabies"]
+ENTRYPOINT ["/opt/conda/envs/nibabies/bin/nibabies"]
```

### Comparing `nibabies-23.0.0/README.md` & `nibabies-23.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/.circleci/bcp_anat_outputs.txt` & `nibabies-23.1.0rc0/.circleci/bcp_anat_outputs.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,47 +4,52 @@
 desc-aseg_dseg.tsv
 logs
 logs/CITATION.bib
 logs/CITATION.html
 logs/CITATION.md
 logs/CITATION.tex
 sub-01
-sub-01.html
 sub-01/ses-1mo
 sub-01/ses-1mo/anat
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-aparcaseg_dseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-aseg_dseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-brain_mask.json
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-brain_mask.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-preproc_T1w.json
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-preproc_T1w.nii.gz
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-ribbon_mask.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_dseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_from-fsnative_to-T1w_mode-image_xfm.txt
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_from-MNIInfant+1_to-T1w_mode-image_xfm.h5
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_from-T1w_to-fsnative_mode-image_xfm.txt
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_from-T1w_to-MNIInfant+1_mode-image_xfm.h5
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_curv.shape.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_desc-reg_sphere.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_inflated.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_midthickness.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_pial.surf.gii
-sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_smoothwm.surf.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_space-fsLR_desc-reg_sphere.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_sulc.shape.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_thickness.shape.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_white.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_curv.shape.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_desc-reg_sphere.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_inflated.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_midthickness.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_pial.surf.gii
-sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_smoothwm.surf.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_space-fsLR_desc-reg_sphere.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_sulc.shape.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_thickness.shape.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_white.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_label-CSF_probseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_label-GM_probseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_label-WM_probseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_desc-brain_mask.json
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_desc-brain_mask.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_desc-preproc_T1w.json
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_desc-preproc_T1w.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_dseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_label-CSF_probseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_label-GM_probseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_label-WM_probseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-T1w_desc-preproc_T2w.nii.gz
+sub-01_ses-1mo.html
```

### Comparing `nibabies-23.0.0/.circleci/bcp_full_outputs.txt` & `nibabies-23.1.0rc0/.circleci/bcp_full_outputs.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,42 +4,46 @@
 desc-aseg_dseg.tsv
 logs
 logs/CITATION.bib
 logs/CITATION.html
 logs/CITATION.md
 logs/CITATION.tex
 sub-01
-sub-01.html
 sub-01/ses-1mo
 sub-01/ses-1mo/anat
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-aparcaseg_dseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-aseg_dseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-brain_mask.json
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-brain_mask.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-preproc_T1w.json
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-preproc_T1w.nii.gz
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_desc-ribbon_mask.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_dseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_from-fsnative_to-T1w_mode-image_xfm.txt
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_from-MNIInfant+1_to-T1w_mode-image_xfm.h5
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_from-T1w_to-fsnative_mode-image_xfm.txt
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_from-T1w_to-MNIInfant+1_mode-image_xfm.h5
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_curv.shape.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_desc-reg_sphere.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_inflated.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_midthickness.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_pial.surf.gii
-sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_smoothwm.surf.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_space-fsLR_desc-reg_sphere.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_sulc.shape.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_thickness.shape.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-L_white.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_curv.shape.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_desc-reg_sphere.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_inflated.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_midthickness.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_pial.surf.gii
-sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_smoothwm.surf.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_space-fsLR_desc-reg_sphere.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_sulc.shape.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_thickness.shape.gii
+sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_hemi-R_white.surf.gii
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_label-CSF_probseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_label-GM_probseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_label-WM_probseg.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_desc-brain_mask.json
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_desc-brain_mask.nii.gz
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_desc-preproc_T1w.json
 sub-01/ses-1mo/anat/sub-01_ses-1mo_run-001_space-MNIInfant_cohort-1_desc-preproc_T1w.nii.gz
@@ -67,7 +71,8 @@
 sub-01/ses-1mo/func/sub-01_ses-1mo_task-rest_acq-PA_run-001_space-MNIInfant_cohort-1_boldref.nii.gz
 sub-01/ses-1mo/func/sub-01_ses-1mo_task-rest_acq-PA_run-001_space-MNIInfant_cohort-1_desc-aparcaseg_dseg.nii.gz
 sub-01/ses-1mo/func/sub-01_ses-1mo_task-rest_acq-PA_run-001_space-MNIInfant_cohort-1_desc-aseg_dseg.nii.gz
 sub-01/ses-1mo/func/sub-01_ses-1mo_task-rest_acq-PA_run-001_space-MNIInfant_cohort-1_desc-brain_mask.json
 sub-01/ses-1mo/func/sub-01_ses-1mo_task-rest_acq-PA_run-001_space-MNIInfant_cohort-1_desc-brain_mask.nii.gz
 sub-01/ses-1mo/func/sub-01_ses-1mo_task-rest_acq-PA_run-001_space-MNIInfant_cohort-1_desc-preproc_bold.json
 sub-01/ses-1mo/func/sub-01_ses-1mo_task-rest_acq-PA_run-001_space-MNIInfant_cohort-1_desc-preproc_bold.nii.gz
+sub-01_ses-1mo.html
```

### Comparing `nibabies-23.0.0/.circleci/config.yml` & `nibabies-23.1.0rc0/.circleci/config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -91,53 +91,16 @@
           paths:
             - /tmp/docker
             - /tmp/images
       - docker/install-docker-credential-helper
       - run: *docker_auth
       - run: *setup_docker_registry
       - run:
-          name: Save Docker registry
-          command: |
-            if [[ ! -f /tmp/images/registry.tar.gz ]]; then
-              mkdir -p /tmp/images
-              docker save registry:2 | gzip > /tmp/images/registry.tar.gz
-            fi
-      - run:
-          name: Pull base image (ubuntu:focal)
-          command: |
-            set +e
-            docker pull localhost:5000/ubuntu
-            success=$?
-            set -e
-            if [[ "$success" = "0" ]]; then
-                echo "Pulling from local registry"
-                docker tag localhost:5000/ubuntu ubuntu:focal
-            else
-                echo "Pulling from Docker Hub"
-                docker pull ubuntu:focal
-                docker tag ubuntu:focal localhost:5000/ubuntu
-                docker push localhost:5000/ubuntu
-            fi
-      - run:
-          name: Pull nibabies image (nipreps/nibabies)
-          command: |
-            set +e
-            docker pull localhost:5000/nibabies
-            success=$?
-            set -e
-            if [[ "$success" = "0" ]]; then
-                echo "Pulled from local registry"
-                docker tag localhost:5000/nibabies nipreps/nibabies:dev
-                docker tag localhost:5000/nibabies nipreps/nibabies
-            else
-                echo "Pulling unstable from Docker Hub"
-                docker pull nipreps/nibabies:unstable
-                docker tag nipreps/nibabies:unstable nipreps/nibabies:dev
-                docker tag nipreps/nibabies:unstable nipreps/nibabies
-            fi
+          name: Create Docker builder
+          command: docker buildx create --use --name=builder --driver=docker-container
       - run:
           name: Clean and check images (before build)
           command: |
             docker image prune -f --filter="dangling=true" -f && docker images
       - run:
           name: Build Docker image
           no_output_timeout: 60m
@@ -151,23 +114,21 @@
             if [[ ${THISVERSION:0:1} == "0" ]] ; then
               echo "WARNING: latest git tag could not be found"
               echo "Please, make sure you fetch all tags from upstream with"
               echo "the command ``git fetch --tags --verbose`` and push"
               echo "them to your fork with ``git push origin --tags``"
             fi
             # Build docker image
-            e=1 && for i in {1..3}; do
-              docker build --rm \
-                --cache-from=nipreps/nibabies \
+            docker buildx build --load --builder builder \
+                --cache-from localhost:5000/nibabies \
+                --cache-from nipreps/nibabies:dev \
                 -t nipreps/nibabies:dev \
                 --build-arg BUILD_DATE=`date -u +"%Y-%m-%dT%H:%M:%SZ"` \
                 --build-arg VCS_REF=`git rev-parse --short HEAD` \
-                --build-arg VERSION="${CIRCLE_TAG:-$THISVERSION}" . \
-              && e=0 && break || sleep 15
-            done && [ "$e" -eq "0" ]
+                --build-arg VERSION="${CIRCLE_TAG:-$THISVERSION}" .
       - run:
           name: Check Docker images (after build)
           command: docker images
       - run:
           name: Check Docker image
           command: |
             export PY3=$(pyenv versions | grep '3\.' |
@@ -465,15 +426,15 @@
       - run: *docker_auth
       - run: *setup_docker_registry
       - run: *pull_from_registry
       - run:
           name: Deploy to Docker Hub
           no_output_timeout: 40m
           command: |
-            docker tag nipreps/nibabies nipreps/nibabies:${CIRCLE_BRANCH#docker/}
+            docker tag nipreps/nibabies:dev nipreps/nibabies:${CIRCLE_BRANCH#docker/}
             docker push nipreps/nibabies:${CIRCLE_BRANCH#docker/}
 
 
   deploy_docker:
     <<: *machine_defaults
     steps:
       - checkout:
```

### Comparing `nibabies-23.0.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `nibabies-23.1.0rc0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `nibabies-23.1.0rc0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/.github/workflows/pytest.yml` & `nibabies-23.1.0rc0/.github/workflows/pytest.yml`

 * *Files 9% similar despite different names*

```diff
@@ -41,11 +41,10 @@
         python -m pip install -U pip
         python -m pip install ".[test]"
     - name: Run Pytest
       run: |
         source /tmp/venv/bin/activate
         pytest -sv --doctest-modules --cov nibabies --cov-report xml nibabies
     - name: Submit coverage
-      run: |
-        # Pin codecov version to reduce scope for malicious updates
-        python -m pip install "codecov==2.1.11"
-        python -m codecov --file coverage.xml
+      uses: codecov/codecov-action@v3
+      with:
+        files: coverage.xml
```

### Comparing `nibabies-23.0.0/.github/workflows/style.yml` & `nibabies-23.1.0rc0/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/.maint/developers.json` & `nibabies-23.1.0rc0/.maint/developers.json`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/.maint/update_changes.sh` & `nibabies-23.1.0rc0/.maint/update_changes.sh`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/.maint/update_zenodo.py` & `nibabies-23.1.0rc0/.maint/update_zenodo.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/docs/Makefile` & `nibabies-23.1.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/docs/community.md` & `nibabies-23.1.0rc0/docs/community.md`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/docs/conf.py` & `nibabies-23.1.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/docs/faqs.md` & `nibabies-23.1.0rc0/docs/faqs.md`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/docs/installation.md` & `nibabies-23.1.0rc0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/docs/make.bat` & `nibabies-23.1.0rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/docs/usage.md` & `nibabies-23.1.0rc0/docs/usage.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,39 +4,52 @@
 
 The *NiBabies* workflow takes as principal input the path of the dataset
 that is to be processed.
 The input dataset is required to be in valid
 {abbr}`BIDS (The Brain Imaging Data Structure)` format,
 and it must include at least one T1-weighted and
 one T2-weighted structural image and
-(unless disabled with a flag) a BOLD series.
+a BOLD series (unless using the `--anat-only` flag).
+
 We highly recommend that you validate your dataset with the free, online
 [BIDS Validator](http://bids-standard.github.io/bids-validator/).
 
-The exact command to run *NiBabies* depends on the [Installation](./installation.md) method.
-The common parts of the command follow the
-[BIDS-Apps](https://github.com/BIDS-Apps) definition.
-Example:
-
-```Shell
-$ nibabies data/bids_root/ out/ participant -w work/ --participant-id 01 --age-months 12
-```
+### Participant Ages
+*NiBabies* will attempt to automatically extract participant ages (in months) from the BIDS layout.
+Specifically, these two files will be checked:
+- [Sessions file](https://bids-specification.readthedocs.io/en/stable/03-modality-agnostic-files.html#sessions-file): `<bids-root>/<subject>/subject_sessions.tsv`
+- [Participants file](https://bids-specification.readthedocs.io/en/stable/03-modality-agnostic-files.html#participants-file): `<bids-root>/participants.tsv`
 
-Further information about BIDS and BIDS-Apps can be found at the
-[NiPreps portal](https://www.nipreps.org/apps/framework/).
+Either file should include `age` (or if you wish to be more explicit: `age_months`) columns, and it is
+recommended to have an accompanying JSON file to further describe these fields, and explicitly state the values are in months.
 
 ## The FreeSurfer license
 
 *NiBabies* uses FreeSurfer tools, which require a license to run.
 
 To obtain a FreeSurfer license, simply register for free at https://surfer.nmr.mgh.harvard.edu/registration.html.
 
 FreeSurfer will search for a license key file first using the `$FS_LICENSE` environment variable and then in the default path to the license key file (`$FREESURFER_HOME`/license.txt). If `$FS_LICENSE` is set, the [`nibabies-wrapper`](#using-the-nibabies-wrapper) will automatically handle setting the license within the container.
 Otherwise, you will need to use the `--fs-license-file` flag to ensure the license is available.
 
+
+## Example command
+
+The exact command to run *NiBabies* depends on the [Installation](./installation.md) method.
+The common parts of the command follow the
+[BIDS-Apps](https://github.com/BIDS-Apps) definition.
+Example:
+
+```Shell
+$ nibabies data/bids_root/ out/ participant -w work/ --participant-id 01
+```
+
+Further information about BIDS and BIDS-Apps can be found at the
+[NiPreps portal](https://www.nipreps.org/apps/framework/).
+
 ## Command-Line Arguments
 ```{argparse}
 :ref: nibabies.cli.parser._build_parser
 :prog: nibabies
 :nodefaultconst:
 ```
 
@@ -46,29 +59,17 @@
 
 - **`bids_dir`** - the root folder of a BIDS valid dataset.
 - **`output_dir`** - folder to store outputs and reports.
 - **`level`** - processing stage to be run, currently can only be `participant`.
 
 However, as infant brains can vastly differ depending on age, providing the following arguments is highly recommended:
 
-- **`--age-months`** - participant age in months
-
-:::{admonition} Warning
-:class: warning
-
-This is required if FreeSurfer is not disabled (`--fs-no-reconall`)
-:::
-
 - **`--participant-id`** - participant ID
 
-:::{admonition} Tip
-:class: tip
-
-This is recommended when using `--age-months` if age varies across participants.
-:::
+- **`--session-id`** - session ID
 
 - **`--segmentation-atlases-dir`** - directory containing pre-labeled segmentations to use for Joint Label Fusion.
 
 :::{admonition} Tip
 :class: tip
 
 The segmentation directory layout should consist of one or more template directories containing:
@@ -81,37 +82,37 @@
 
 The wrapper will generate a Docker or Singularity command line for you, print it out for reporting purposes, and then execute it without further action needed.
 For installation instructions, please see [](installation.md#installing-the-nibabies-wrapper)
 
 ### Sample Docker usage
 
 ```
-$ nibabies-wrapper docker /path/to/data /path/to/output participant --age-months 12 --fs-license-file /usr/freesurfer/license.txt
+$ nibabies-wrapper docker /path/to/data /path/to/output participant --fs-license-file /usr/freesurfer/license.txt
 
 RUNNING: docker run --rm -e DOCKER_VERSION_8395080871=20.10.6 -it -v /path/to/data:/data:ro \
 -v /path/to/output:/out -v /usr/freesurfer/license.txt:/opt/freesurfer/license.txt:ro \
-nipreps/nibabies:21.0.0 /data /out participant --age-months 12
+nipreps/nibabies:23.0.0 /data /out participant
 ...
 ```
 
 :::{admonition} Docker usage warning
 :class: warning
 
 When using Docker, the wrapper will default to using the same version of `nibabies` as the wrapper.
 This can be overridden by using the `-i` flag to specify a particular Docker image.
 :::
 
 ### Sample Singularity usage
 
 ```
-$ nibabies-wrapper singularity /path/to/data /path/to/output participant --age-months 12 -i nibabies-21.0.0.sif --fs-license-file /usr/freesurfer/license.txt
+$ nibabies-wrapper singularity /path/to/data /path/to/output participant -i nibabies-23.0.0.sif --fs-license-file /usr/freesurfer/license.txt
 
 RUNNING: singularity run --cleanenv -B /path/to/data:/data:ro \
 -B /path/to/output:/out -B /usr/freesurfer/license.txt:/opt/freesurfer/license.txt:ro \
-nibabies-21.0.0.sif /data /out participant --age-months 12
+nibabies-23.0.0.sif /data /out participant
 ...
 ```
 
 :::{admonition} Singularity usage warning
 :class: warning
 
 Note that the `-i` flag is required when using Singularity, and should be the path to the already built Singularity image file.
```

### Comparing `nibabies-23.0.0/docs/_static/nibabies_anat.png` & `nibabies-23.1.0rc0/docs/_static/nibabies_anat.png`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/docs/_static/nibabies_func.png` & `nibabies-23.1.0rc0/docs/_static/nibabies_func.png`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/docs/sphinxext/github_link.py` & `nibabies-23.1.0rc0/docs/sphinxext/github_link.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/__about__.py` & `nibabies-23.1.0rc0/nibabies/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # emacs: -*- mode: python; py-indent-offset: 4; indent-tabs-mode: nil -*-
 # vi: set ft=python sts=4 ts=4 sw=4 et:
 """Base module variables."""
 
 try:
     from ._version import __version__
 except ImportError:
-    __version__ == "0+unknown"
+    __version__ = "0+unknown"
 
 __org__ = "nipreps"
 __packagename__ = "nibabies"
 __copyright__ = "Copyright 2023, Center for Reproducible Neuroscience, Stanford University"
 __credits__ = (
     "Contributors: please check the ``.zenodo.json`` file at the top-level folder"
     "of the repository"
```

### Comparing `nibabies-23.0.0/nibabies/_warnings.py` & `nibabies-23.1.0rc0/nibabies/_warnings.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/config.py` & `nibabies-23.1.0rc0/nibabies/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     del _fs_home
 
 _templateflow_home = Path(os.getenv("TEMPLATEFLOW_HOME", Path.home() / ".cache" / "templateflow"))
 
 try:
     from psutil import virtual_memory
 
-    _free_mem_at_start = round(virtual_memory().free / 1024**3, 1)
+    _free_mem_at_start = round(virtual_memory().available / 1024**3, 1)
 except Exception:
     _free_mem_at_start = None
 
 _oc_limit = "n/a"
 _oc_policy = "n/a"
 try:
     # Memory policy may have a large effect on types of errors experienced
@@ -390,14 +390,16 @@
     """A :py:class:`~bids.layout.BIDSLayout` object, see :py:func:`init`."""
     log_dir = None
     """The path to a directory that contains execution logs."""
     log_level = 25
     """Output verbosity."""
     low_mem = None
     """Utilize uncompressed NIfTIs and other tricks to minimize memory allocation."""
+    mcribs_dir = None
+    """M-CRIB-S processing and output directory."""
     md_only_boilerplate = False
     """Do not convert boilerplate from MarkDown to LaTex and HTML."""
     nibabies_dir = None
     """Root of NiBabies BIDS Derivatives dataset. Depends on output_layout."""
     notrack = False
     """Do not monitor *nibabies* using *migas*."""
     output_dir = None
@@ -419,14 +421,16 @@
     """List of session identifiers that are to be preprocessed."""
     participant_label = None
     """List of participant identifiers that are to be preprocessed."""
     task_id = None
     """Select a particular task from all available in the dataset."""
     templateflow_home = _templateflow_home
     """The root folder of the TemplateFlow client."""
+    unique_labels = None
+    """Combinations of subject + session identifiers to be preprocessed."""
     work_dir = Path("work").absolute()
     """Path to a working directory where intermediate results will be available."""
     write_graph = False
     """Write out the computational graph corresponding to the planned preprocessing."""
 
     _layout = None
 
@@ -435,24 +439,31 @@
         "bids_dir",
         "bids_database_dir",
         "derivatives",
         "fs_license_file",
         "fs_subjects_dir",
         "layout",
         "log_dir",
+        "mcribs_dir",
         "nibabies_dir",
         "output_dir",
         "segmentation_atlases_dir",
         "templateflow_home",
         "work_dir",
     )
 
     @classmethod
     def init(cls):
         """Create a new BIDS Layout accessible with :attr:`~execution.layout`."""
+        # Convert string literal None to NoneType
+        if cls.unique_labels:
+            cls.unique_labels = [
+                [sub, ses] if ses != 'None' else [sub, None] for sub, ses in cls.unique_labels
+            ]
+
         if cls.fs_license_file and Path(cls.fs_license_file).is_file():
             os.environ["FS_LICENSE"] = str(cls.fs_license_file)
 
         if cls._layout is None:
             import re
 
             from bids.layout import BIDSLayout, BIDSLayoutIndexer
@@ -539,24 +550,24 @@
     """Head radius in mm for framewise displacement calculation"""
     fmap_bspline = None
     """Regularize fieldmaps with a field of B-Spline basis."""
     fmap_demean = None
     """Remove the mean from fieldmaps."""
     force_syn = None
     """Run *fieldmap-less* susceptibility-derived distortions estimation."""
-    force_reconall = False
-    """Force traditional FreeSurfer surface reconstruction instead of infant version."""
     hires = None
     """Run FreeSurfer ``recon-all`` with the ``-hires`` flag."""
     ignore = None
     """Ignore particular steps for *nibabies*."""
     longitudinal = False
     """Run FreeSurfer ``recon-all`` with the ``-logitudinal`` flag."""
     medial_surface_nan = None
     """Fill medial surface with :abbr:`NaNs (not-a-number)` when sampling."""
+    project_goodvoxels = False
+    """Exclude voxels with locally high coefficient of variation from sampling."""
     regressors_all_comps = None
     """Return all CompCor components."""
     regressors_dvars_th = None
     """Threshold for DVARS."""
     regressors_fd_th = None
     """Threshold for :abbr:`FD (frame-wise displacement)`."""
     run_reconall = True
@@ -572,16 +583,16 @@
     """The time of the reference slice to correct BOLD values to, as a fraction
     acquisition time. 0 indicates the start, 0.5 the midpoint, and 1 the end
     of acquisition. The alias `start` corresponds to 0, and `middle` to 0.5.
     The default value is 0.5."""
     spaces = None
     """Keeps the :py:class:`~niworkflows.utils.spaces.SpatialReferences`
     instance keeping standard and nonstandard spaces."""
-    topup_max_vols = 5
-    """Maximum number of volumes to use with TOPUP, per-series (EPI or BOLD)."""
+    surface_recon_method = "infantfs"
+    """Method to use for surface reconstruction."""
     use_aroma = None
     """Run ICA-:abbr:`AROMA (automatic removal of motion artifacts)`."""
     use_bbr = False
     """Run boundary-based registration for BOLD-to-T1w registration."""
     use_syn_sdc = None
     """Run *fieldmap-less* susceptibility-derived distortions estimation
     in the absence of any alternatives."""
@@ -685,15 +696,14 @@
     filename = Path(filename)
     settings = loads(filename.read_text())
     for sectionname, configs in settings.items():
         if sectionname != "environment":
             section = getattr(sys.modules[__name__], sectionname)
             ignore = skip.get(sectionname)
             section.load(configs, ignore=ignore)
-    init_spaces()
 
 
 def get(flat=False):
     """Get config as a dict."""
     settings = {
         "environment": environment.get(),
         "execution": execution.get(),
@@ -720,50 +730,14 @@
 
 def to_filename(filename):
     """Write settings to file."""
     filename = Path(filename)
     filename.write_text(dumps())
 
 
-def init_spaces(checkpoint=True):
-    """Initialize the :attr:`~workflow.spaces` setting."""
-    from niworkflows.utils.spaces import Reference, SpatialReferences
-
-    spaces = execution.output_spaces or SpatialReferences()
-    if not isinstance(spaces, SpatialReferences):
-        spaces = SpatialReferences(
-            [ref for s in spaces.split(" ") for ref in Reference.from_string(s)]
-        )
-
-    if checkpoint and not spaces.is_cached():
-        spaces.checkpoint()
-
-    # Ensure user-defined spatial references for outputs are correctly parsed.
-    # Certain options require normalization to a space not explicitly defined by users.
-    # These spaces will not be included in the final outputs.
-    if workflow.use_aroma:
-        # Make sure there's a normalization to FSL for AROMA to use.
-        spaces.add(Reference("MNI152NLin6Asym", {"res": "2"}))
-
-    if workflow.cifti_output:
-        # CIFTI grayordinates to corresponding FSL-MNI resolutions.
-        vol_res = "2" if workflow.cifti_output == "91k" else "1"
-        spaces.add(Reference("fsaverage", {"den": "164k"}))
-        spaces.add(Reference("MNI152NLin6Asym", {"res": vol_res}))
-        # Ensure a non-native version of MNIInfant is added as a target
-        if workflow.age_months is not None:
-            from .utils.misc import cohort_by_months
-
-            cohort = cohort_by_months("MNIInfant", workflow.age_months)
-            spaces.add(Reference("MNIInfant", {"cohort": cohort}))
-
-    # Make the SpatialReferences object available
-    workflow.spaces = spaces
-
-
 def _process_initializer(cwd, omp_nthreads):
     """Initialize the environment of the child process."""
     os.chdir(cwd)
     os.environ["NIPYPE_NO_ET"] = "1"
     os.environ["OMP_NUM_THREADS"] = f"{omp_nthreads}"
```

### Comparing `nibabies-23.0.0/nibabies/conftest.py` & `nibabies-23.1.0rc0/nibabies/conftest.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/cli/parser.py` & `nibabies-23.1.0rc0/nibabies/cli/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -330,14 +330,23 @@
         required=False,
         action="store_true",
         default=False,
         help="Replace medial wall values with NaNs on functional GIFTI files. Only "
         "performed for GIFTI files mapped to a freesurfer subject (fsaverage or fsnative).",
     )
     g_conf.add_argument(
+        "--project-goodvoxels",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Exclude voxels whose timeseries have locally high coefficient of variation "
+        "from surface resampling. Only performed for GIFTI files mapped to a freesurfer subject "
+        "(fsaverage or fsnative).",
+    )
+    g_conf.add_argument(
         "--slice-time-ref",
         required=False,
         action="store",
         default=None,
         type=SliceTimeRef,
         help="The time of the reference slice to correct BOLD values to, as a fraction "
         "acquisition time. 0 indicates the start, 0.5 the midpoint, and 1 the end "
@@ -651,46 +660,46 @@
     )
     g_baby.add_argument(
         "--force-reconall",
         default=False,
         action="store_true",
         help="Force traditional FreeSurfer surface reconstruction.",
     )
+    g_baby.add_argument(
+        "--surface-recon-method",
+        choices=("infantfs", "freesurfer", "mcribs"),
+        default="infantfs",
+        help="Method to use for surface reconstruction",
+    )
     return parser
 
 
 def parse_args(args=None, namespace=None):
     """Parse args and run further checks on the command line."""
     import logging
 
     parser = _build_parser()
     opts = parser.parse_args(args, namespace)
 
+    # Deprecations
+    if opts.force_reconall:
+        config.loggers.cli.warning(
+            "--force-reconall is deprecated and will be removed in a future release."
+            "To run traditional `recon-all`, use `--surface-recon-method freesurfer` instead."
+        )
+        opts.surface_recon_method = "freesurfer"
+
     if opts.config_file:
         skip = {} if opts.reports_only else {"execution": ("run_uuid",)}
         config.load(opts.config_file, skip=skip)
         config.loggers.cli.info(f"Loaded previous configuration file {opts.config_file}")
 
     config.execution.log_level = int(max(25 - 5 * opts.verbose_count, logging.DEBUG))
     config.from_dict(vars(opts))
 
-    # Initialize --output-spaces if not defined
-    if config.execution.output_spaces is None:
-        from niworkflows.utils.spaces import Reference, SpatialReferences
-
-        from ..utils.misc import cohort_by_months
-
-        if config.workflow.age_months is None:
-            parser.error("--age-months must be provided if --output-spaces is not set.")
-
-        cohort = cohort_by_months("MNIInfant", config.workflow.age_months)
-        config.execution.output_spaces = SpatialReferences(
-            [Reference("MNIInfant", {"res": "native", "cohort": cohort})]
-        )
-
     # Retrieve logging level
     build_log = config.loggers.cli
 
     # Load base plugin_settings from file if --use-plugin
     if opts.use_plugin is not None:
         import yaml
 
@@ -732,22 +741,29 @@
     output_dir = config.execution.output_dir
     work_dir = config.execution.work_dir
     version = config.environment.version
     output_layout = config.execution.output_layout
 
     if config.execution.fs_subjects_dir is None:
         if output_layout == "bids":
-            config.execution.fs_subjects_dir = output_dir / "sourcedata" / "infant-freesurfer"
+            config.execution.fs_subjects_dir = output_dir / "sourcedata" / "freesurfer"
         elif output_layout == "legacy":
-            config.execution.fs_subjects_dir = output_dir / "infant-freesurfer"
+            config.execution.fs_subjects_dir = output_dir / "freesurfer"
     if config.execution.nibabies_dir is None:
         if output_layout == "bids":
             config.execution.nibabies_dir = output_dir
         elif output_layout == "legacy":
             config.execution.nibabies_dir = output_dir / "nibabies"
+    if config.workflow.surface_recon_method == "mcribs":
+        if output_layout == "bids":
+            config.execution.mcribs_dir = output_dir / "sourcedata" / "mcribs"
+        elif output_layout == "legacy":
+            config.execution.mcribs_dir = output_dir / "mcribs"
+        # Ensure the directory is created
+        config.execution.mcribs_dir.mkdir(exist_ok=True, parents=True)
 
     # Wipe out existing work_dir
     if opts.clean_workdir and work_dir.exists():
         from niworkflows.utils.misc import clean_directory
 
         build_log.info(f"Clearing previous NiBabies working directory: {work_dir}")
         if not clean_directory(work_dir):
@@ -797,12 +813,45 @@
         parser.error(
             "One or more participant labels were not found in the BIDS directory: "
             f"{', '.join(missing_subjects)}."
         )
 
     config.execution.participant_label = sorted(participant_label)
     config.workflow.skull_strip_template = config.workflow.skull_strip_template[0]
+    config.execution.unique_labels = compute_subworkflows()
 
     # finally, write config to file
     config_file = config.execution.work_dir / config.execution.run_uuid / "config.toml"
     config_file.parent.mkdir(exist_ok=True, parents=True)
     config.to_filename(config_file)
+
+
+def compute_subworkflows() -> list:
+    """
+    Query all available participants and sessions, and construct the combinations of the
+    subworkflows needed.
+    """
+    from niworkflows.utils.bids import collect_participants
+
+    from nibabies import config
+
+    # consists of (subject_id, session_id) tuples
+    subworkflows = []
+
+    subject_list = collect_participants(
+        config.execution.layout,
+        participant_label=config.execution.participant_label,
+        strict=True,
+    )
+
+    for subject in subject_list:
+        # Due to rapidly changing morphometry of the population
+        # Ensure each subject session is processed individually
+        sessions = (
+            config.execution.session_id
+            or config.execution.layout.get_sessions(scope='raw', subject=subject)
+            or [None]
+        )
+        # grab participant age per session
+        for session in sessions:
+            subworkflows.append((subject, session))
+    return subworkflows
```

### Comparing `nibabies-23.0.0/nibabies/cli/run.py` & `nibabies-23.1.0rc0/nibabies/cli/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,15 @@
         finally:
             from pkg_resources import resource_filename as pkgrf
 
             from ..reports.core import generate_reports
 
             # Generate reports phase
             generate_reports(
-                config.execution.participant_label,
-                config.execution.session_id,
+                config.execution.unique_labels,
                 config.execution.nibabies_dir,
                 config.execution.run_uuid,
                 config=pkgrf("nibabies", "data/reports-spec.yml"),
                 packagename="nibabies",
             )
             write_derivative_description(config.execution.bids_dir, config.execution.nibabies_dir)
             write_bidsignore(config.execution.nibabies_dir)
```

### Comparing `nibabies-23.0.0/nibabies/cli/version.py` & `nibabies-23.1.0rc0/nibabies/cli/version.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/cli/workflow.py` & `nibabies-23.1.0rc0/nibabies/cli/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 a hard-limited memory-scope.
 
 """
 
 
 def build_workflow(config_file):
     """Create the Nipype Workflow that supports the whole execution graph."""
-    from niworkflows.utils.bids import check_pipeline_version, collect_participants
+    from niworkflows.utils.bids import check_pipeline_version
     from niworkflows.utils.misc import check_valid_fs_license
 
     from .. import config
     from ..reports.core import generate_reports
     from ..utils.misc import check_deps
     from ..workflows.base import init_nibabies_wf
 
@@ -38,57 +38,50 @@
     dset_desc_path = config.execution.bids_dir / "dataset_description.json"
     if dset_desc_path.exists():
         from hashlib import sha256
 
         desc_content = dset_desc_path.read_bytes()
         config.execution.bids_description_hash = sha256(desc_content).hexdigest()
 
-    # First check that bids_dir looks like a BIDS folder
-    subject_list = collect_participants(
-        config.execution.layout, participant_label=config.execution.participant_label
-    )
-    subjects_sessions = {
-        subject: config.execution.session_id
-        or config.execution.layout.get_sessions(scope='raw', subject=subject)
-        or [None]
-        for subject in subject_list
-    }
-
     # Called with reports only
     if config.execution.reports_only:
         from pkg_resources import resource_filename as pkgrf
 
-        build_logger.log(25, "Running --reports-only on participants %s", ", ".join(subject_list))
+        build_logger.log(
+            25,
+            "Running --reports-only on participants %s",
+            ", ".join(config.execution.unique_labels),
+        )
         retval["return_code"] = generate_reports(
-            subject_list,
+            config.execution.unique_labels,
             nibabies_dir,
             config.execution.run_uuid,
             config=pkgrf("nibabies", "data/reports-spec.yml"),
             packagename="nibabies",
         )
         return retval
 
     # Build main workflow
     init_msg = f"""
     Running nibabies version {config.environment.version}:
       * BIDS dataset path: {config.execution.bids_dir}.
-      * Participant list: {subject_list}.
+      * Participant list: {config.execution.unique_labels}.
       * Run identifier: {config.execution.run_uuid}.
-      * Output spaces: {config.execution.output_spaces}."""
+      * Output spaces: {config.execution.output_spaces or 'MNIInfant'}."""
 
     if config.execution.anat_derivatives:
         init_msg += f"""
       * Anatomical derivatives: {config.execution.anat_derivatives}."""
 
     if config.execution.fs_subjects_dir:
         init_msg += f"""
       * Pre-run FreeSurfer's SUBJECTS_DIR: {config.execution.fs_subjects_dir}."""
     build_logger.log(25, init_msg)
 
-    retval["workflow"] = init_nibabies_wf(subjects_sessions)
+    retval["workflow"] = init_nibabies_wf(config.execution.unique_labels)
 
     # Check for FS license after building the workflow
     if not check_valid_fs_license():
         build_logger.critical(
             """\
 ERROR: a valid license file is required for FreeSurfer to run. nibabies looked for an existing \
 license file at several paths, in this order: 1) command line argument ``--fs-license-file``; \
```

### Comparing `nibabies-23.0.0/nibabies/data/FreeSurferSubcorticalLabelTableLut.txt` & `nibabies-23.1.0rc0/nibabies/data/FreeSurferSubcorticalLabelTableLut.txt`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/data/antsBrainExtraction_precise.json` & `nibabies-23.1.0rc0/nibabies/data/antsBrainExtraction_precise.json`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/data/antsBrainExtraction_testing.json` & `nibabies-23.1.0rc0/nibabies/data/antsBrainExtraction_testing.json`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/data/boilerplate.bib` & `nibabies-23.1.0rc0/nibabies/data/boilerplate.bib`

 * *Files 3% similar despite different names*

```diff
@@ -388,7 +388,20 @@
 	publisher = {Elsevier {BV}},
 	volume = {218},
 	pages = {116946},
 	author = {Lilla Zöllei and Juan Eugenio Iglesias and Yangming Ou and P. Ellen Grant and Bruce Fischl},
 	title = {Infant {FreeSurfer}: An automated segmentation and surface extraction pipeline for T1-weighted neuroimaging data of infants 0{\textendash}2 years},
 	journal = {{NeuroImage}}
 }
+
+@article{mcribs,
+	doi = {10.1038/s41598-020-61326-2},
+	url = {https://doi.org/10.1038%2Fs41598-020-61326-2},
+	year = 2020,
+	month = {mar},
+	publisher = {Springer Science and Business Media {LLC}},
+	volume = {10},
+	number = {1},
+	author = {Chris L. Adamson and Bonnie Alexander and Gareth Ball and Richard Beare and Jeanie L. Y. Cheong and Alicia J. Spittle and Lex W. Doyle and Peter J. Anderson and Marc L. Seal and Deanne K. Thompson},
+	title = {Parcellation of the neonatal cortex using Surface-based Melbourne Children's Regional Infant Brain atlases (M-{CRIB}-S)},
+	journal = {Scientific Reports}
+}
```

### Comparing `nibabies-23.0.0/nibabies/data/reports-spec.yml` & `nibabies-23.1.0rc0/nibabies/data/reports-spec.yml`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/data/t1_to_bold.json` & `nibabies-23.1.0rc0/nibabies/data/t1_to_bold.json`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/data/tpl-MNI152NLin6Asym_res-01_desc-avgwmparc_dseg.nii.gz` & `nibabies-23.1.0rc0/nibabies/data/tpl-MNI152NLin6Asym_res-01_desc-avgwmparc_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/data/within_subject_t1t2.json` & `nibabies-23.1.0rc0/nibabies/data/within_subject_t1t2.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {'delete': "['use_estimate_learning_rate_once']"}*

```diff
@@ -104,19 +104,14 @@
         ]
     ],
     "transforms": [
         "Translation",
         "Rigid",
         "SyN"
     ],
-    "use_estimate_learning_rate_once": [
-        false,
-        false,
-        true
-    ],
     "use_histogram_matching": [
         true,
         true,
         true
     ],
     "verbose": true,
     "winsorize_lower_quantile": 0.0001,
```

### Comparing `nibabies-23.0.0/nibabies/data/flirtsch/bbr.sch` & `nibabies-23.1.0rc0/nibabies/data/flirtsch/bbr.sch`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/data/tests/config.toml` & `nibabies-23.1.0rc0/nibabies/data/tests/config.toml`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 fd_radius = 45
 fmap_bspline = false
 force_syn = false
 hires = true
 ignore = [ "slicetiming",]
 longitudinal = false
 medial_surface_nan = false
+project_goodvoxels = false
 regressors_all_comps = false
 regressors_dvars_th = 1.5
 regressors_fd_th = 0.5
 run_reconall = true
 skull_strip_fixed_seed = false
 skull_strip_template = "UNCInfant:cohort-1"
 skull_strip_t1w = "force"
```

### Comparing `nibabies-23.0.0/nibabies/interfaces/confounds.py` & `nibabies-23.1.0rc0/nibabies/interfaces/confounds.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/interfaces/freesurfer.py` & `nibabies-23.1.0rc0/nibabies/interfaces/freesurfer.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/interfaces/gifti.py` & `nibabies-23.1.0rc0/nibabies/interfaces/gifti.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/interfaces/maths.py` & `nibabies-23.1.0rc0/nibabies/interfaces/maths.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/interfaces/multiecho.py` & `nibabies-23.1.0rc0/nibabies/interfaces/multiecho.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/interfaces/nibabel.py` & `nibabies-23.1.0rc0/nibabies/interfaces/nibabel.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/interfaces/reports.py` & `nibabies-23.1.0rc0/nibabies/interfaces/reports.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/interfaces/workbench.py` & `nibabies-23.1.0rc0/nibabies/interfaces/workbench.py`

 * *Files 9% similar despite different names*

```diff
@@ -1441,7 +1441,242 @@
     'wb_command -volume-label-import .../atlas.nii .../label_list.txt \
     atlas_labels.nii.gz'
     """
 
     input_spec = VolumeLabelImportInputSpec
     output_spec = VolumeLabelImportOutputSpec
     _cmd = "wb_command -volume-label-import"
+
+
+class CreateSignedDistanceVolumeInputSpec(CommandLineInputSpec):
+    surf_file = File(
+        exists=True,
+        mandatory=True,
+        argstr="%s",
+        position=0,
+        desc="Input surface GIFTI file (.surf.gii)",
+    )
+    ref_file = File(
+        exists=True,
+        mandatory=True,
+        argstr="%s",
+        position=1,
+        desc="NIfTI volume in the desired output space (dims, spacing, origin)",
+    )
+    out_file = File(
+        name_source=["surf_file"],
+        name_template="%s_distvol.nii.gz",
+        argstr="%s",
+        position=2,
+        desc="Name of output volume containing signed distances",
+    )
+    out_mask = File(
+        name_source=["surf_file"],
+        name_template="%s_distmask.nii.gz",
+        argstr="-roi-out %s",
+        desc="Name of file to store a mask where the ``out_file`` has a computed value",
+    )
+    fill_value = traits.Float(
+        0.0,
+        mandatory=False,
+        usedefault=True,
+        argstr="-fill-value %f",
+        desc="value to put in all voxels that don't get assigned a distance",
+    )
+    exact_limit = traits.Float(
+        5.0,
+        usedefault=True,
+        argstr="-exact-limit %f",
+        desc="distance for exact output in mm",
+    )
+    approx_limit = traits.Float(
+        20.0,
+        usedefault=True,
+        argstr="-approx-limit %f",
+        desc="distance for approximate output in mm",
+    )
+    approx_neighborhood = traits.Int(
+        2,
+        usedefault=True,
+        argstr="-approx-neighborhood %d",
+        desc="size of neighborhood cube measured from center to face in voxels, default 2 = 5x5x5",
+    )
+    winding_method = traits.Enum(
+        "EVEN_ODD",
+        "NEGATIVE",
+        "NONZERO",
+        "NORMALS",
+        argstr="-winding %s",
+        usedefault=True,
+        desc="winding method for point inside surface test",
+    )
+
+
+class CreateSignedDistanceVolumeOutputSpec(TraitedSpec):
+    out_file = File(desc="Name of output volume containing signed distances")
+    out_mask = File(
+        desc="Name of file to store a mask where the ``out_file`` has a computed value"
+    )
+
+
+class CreateSignedDistanceVolume(WBCommand):
+    """CREATE SIGNED DISTANCE VOLUME FROM SURFACE
+    wb_command -create-signed-distance-volume
+       <surface> - the input surface
+       <refspace> - a volume in the desired output space (dims, spacing, origin)
+       <outvol> - output - the output volume
+
+       [-roi-out] - output an roi volume of where the output has a computed
+          value
+          <roi-vol> - output - the output roi volume
+
+       [-fill-value] - specify a value to put in all voxels that don't get
+          assigned a distance
+          <value> - value to fill with (default 0)
+
+       [-exact-limit] - specify distance for exact output
+          <dist> - distance in mm (default 5)
+
+       [-approx-limit] - specify distance for approximate output
+          <dist> - distance in mm (default 20)
+
+       [-approx-neighborhood] - voxel neighborhood for approximate calculation
+          <num> - size of neighborhood cube measured from center to face, in
+             voxels (default 2 = 5x5x5)
+
+       [-winding] - winding method for point inside surface test
+          <method> - name of the method (default EVEN_ODD)
+
+       Computes the signed distance function of the surface.  Exact distance is
+       calculated by finding the closest point on any surface triangle to the
+       center of the voxel.  Approximate distance is calculated starting with
+       these distances, using dijkstra's method with a neighborhood of voxels.
+       Specifying too small of an exact distance may produce unexpected results.
+       Valid specifiers for winding methods are as follows:
+
+       EVEN_ODD (default)
+       NEGATIVE
+       NONZERO
+       NORMALS
+
+       The NORMALS method uses the normals of triangles and edges, or the
+       closest triangle hit by a ray from the point.  This method may be
+       slightly faster, but is only reliable for a closed surface that does not
+       cross through itself.  All other methods count entry (positive) and exit
+       (negative) crossings of a vertical ray from the point, then counts as
+       inside if the total is odd, negative, or nonzero, respectively.
+
+    """
+
+    input_spec = CreateSignedDistanceVolumeInputSpec
+    output_spec = CreateSignedDistanceVolumeOutputSpec
+    _cmd = "wb_command -create-signed-distance-volume"
+
+
+class SurfaceAverageInputSpec(CommandLineInputSpec):
+    out_file = File(
+        name_template="averaged.surf.gii",
+        position=0,
+        desc="output file",
+    )
+    surfaces = InputMultiObject(
+        traits.Either(
+            File(exists=True),
+            traits.Tuple(File(exists=True), traits.Float),
+        ),
+        argstr="%s",
+        position=3,
+        desc="Surface, or surface and weighted average tuple, to include in the average",
+    )
+
+
+class SurfaceAverageOutputSpec(TraitedSpec):
+    out_file = File(desc="The output averaged surface")
+    # stddev_metric = File(desc="The output metric for 3D sample standard deviation")
+    # uncert_metric = File(desc="The output metric for uncertainty")
+
+
+class SurfaceAverage(WBCommand):
+    """
+    AVERAGE SURFACE FILES TOGETHER
+    wb_command -surface-average
+      <surface-out> - output - the output averaged surface
+
+      [-stddev] - compute 3D sample standard deviation
+         <stddev-metric-out> - output - the output metric for 3D sample
+            standard deviation
+
+      [-uncertainty] - compute caret5 'uncertainty'
+         <uncert-metric-out> - output - the output metric for uncertainty
+
+      [-surf] - repeatable - specify a surface to include in the average
+         <surface> - a surface file to average
+
+         [-weight] - specify a weighted average
+            <weight> - the weight to use (default 1)
+
+      The 3D sample standard deviation is computed as
+      'sqrt(sum(squaredlength(xyz - mean(xyz)))/(n - 1))'.
+
+      Uncertainty is a legacy measure used in caret5, and is computed as
+      'sum(length(xyz - mean(xyz)))/n'.
+
+      When weights are used, the 3D sample standard deviation treats them as
+      reliability weights.
+    """
+
+    input_spec = SurfaceAverageInputSpec
+    output_spec = SurfaceAverageOutputSpec
+    _cmd = "wb_command -surface-average"
+
+    def _format_arg(self, name, trait_spec, value):
+        if name == 'surfaces':
+            cmd = []
+            for val in value:
+                if len(val) == 2:
+                    cmd.append(f"{val[0]} -weight {val[-1]}")
+                else:
+                    cmd.append(val)
+            return '-surf ' + ' -surf '.join(cmd)
+        return super()._format_arg(name, trait_spec, value)
+
+    def _list_output(self):
+        outputs = self.output_spec().get()
+        outputs["out_file"] = os.path.abspath(self.inputs.out_file)
+        return outputs
+
+
+class SurfaceVertexAreasInputSpec(CommandLineInputSpec):
+    in_file = File(
+        exists=True,
+        mandatory=True,
+        position=0,
+        argstr="%s",
+        desc="Input surface",
+    )
+    out_file = File(
+        name_template="%s.shape.gii",
+        name_source="in_file",
+        position=1,
+        argstr="%s",
+        desc="Output vertex areas",
+    )
+
+
+class SurfaceVertexAreasOutputSpec(TraitedSpec):
+    out_file = File(desc="Output vertex areas")
+
+
+class SurfaceVertexAreas(WBCommand):
+    """
+    MEASURE SURFACE AREA EACH VERTEX IS RESPONSIBLE FOR
+    wb_command -surface-vertex-areas
+      <surface> - the surface to measure
+      <metric> - output - the output metric
+
+      Each vertex gets one third of the area of each triangle it is a part of.
+      Units are mm^2.
+    """
+
+    input_spec = SurfaceVertexAreasInputSpec
+    output_spec = SurfaceVertexAreasOutputSpec
+    _cmd = "wb_command -surface-vertex-areas"
```

### Comparing `nibabies-23.0.0/nibabies/interfaces/tests/test_nibabel.py` & `nibabies-23.1.0rc0/nibabies/interfaces/tests/test_nibabel.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/reports/core.py` & `nibabies-23.1.0rc0/nibabies/reports/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -83,36 +83,31 @@
         subject_id=subject_label,
         packagename=packagename,
         reportlets_dir=reportlets_dir,
     ).generate_report()
 
 
 def generate_reports(
-    subject_list,
-    sessions_list,
+    sub_ses_list,
     output_dir,
     run_uuid,
     config=None,
     work_dir=None,
     packagename=None,
 ):
     """Execute run_reports on a list of subjects."""
     reportlets_dir = None
     if work_dir is not None:
         reportlets_dir = Path(work_dir) / "reportlets"
 
-    if sessions_list is None:
-        sessions_list = [None]
-
     report_errors = []
-    for subject_label, session in product(subject_list, sessions_list):
-        html_report = f"sub-{subject_label}"
-        if session:
-            html_report += f"_ses-{session}"
-        html_report += ".html"
+    for subject_label, session in sub_ses_list:
+        html_report = ''.join(
+            [f"sub-{subject_label}", f"_ses-{session}" if session else "", ".html"]
+        )
         report_errors.append(
             run_reports(
                 output_dir,
                 subject_label,
                 run_uuid,
                 config=config,
                 out_filename=html_report,
@@ -123,15 +118,15 @@
 
     errno = sum(report_errors)
     if errno:
         import logging
 
         logger = logging.getLogger("cli")
         error_list = ", ".join(
-            "%s (%d)" % (subid, err) for subid, err in zip(subject_list, report_errors) if err
+            "%s (%d)" % (subid, err) for subid, err in zip(sub_ses_list, report_errors) if err
         )
         logger.error(
             "Preprocessing did not finish successfully. Errors occurred while processing "
             "data from participants: %s. Check the HTML reports for details.",
             error_list,
         )
     return errno
```

### Comparing `nibabies-23.0.0/nibabies/tests/test_config.py` & `nibabies-23.1.0rc0/nibabies/tests/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,67 +62,56 @@
     settings = loads(filename.read_text())
     for sectionname, configs in settings.items():
         if sectionname != 'environment':
             section = getattr(config, sectionname)
             section.load(configs, init=False)
     config.nipype.init()
     config.loggers.init()
-    config.init_spaces()
-
-    spaces = config.workflow.spaces
+    age = 8
+    spaces = _load_spaces(age)
     assert "MNI152NLin6Asym:res-2" not in [str(s) for s in spaces.get_standard(full_spec=True)]
 
     assert "MNI152NLin6Asym_res-2" not in [
         format_reference((s.fullname, s.spec))
         for s in spaces.references
         if s.standard and s.dim == 3
     ]
 
     config.workflow.use_aroma = True
-    config.init_spaces()
-    spaces = config.workflow.spaces
+    spaces = _load_spaces(age)
 
     assert "MNI152NLin6Asym:res-2" in [str(s) for s in spaces.get_standard(full_spec=True)]
 
     assert "MNI152NLin6Asym_res-2" in [
         format_reference((s.fullname, s.spec))
         for s in spaces.references
         if s.standard and s.dim == 3
     ]
 
     config.execution.output_spaces = None
     config.workflow.use_aroma = False
-    config.workflow.age_months = None
-    config.init_spaces()
-    spaces = config.workflow.spaces
 
-    assert [str(s) for s in spaces.get_standard(full_spec=True)] == []
-    assert [
-        format_reference((s.fullname, s.spec))
-        for s in spaces.references
-        if s.standard and s.dim == 3
-    ] == []
+    with pytest.raises(RuntimeError):
+        spaces = _load_spaces(None)
 
     config.execution.output_spaces = None
     config.workflow.cifti_output = "91k"
     config.workflow.use_aroma = False
-    config.workflow.age_months = 1
-    config.init_spaces()
-    spaces = config.workflow.spaces
+    spaces = _load_spaces(1)
 
     assert [str(s) for s in spaces.get_standard(full_spec=True)] == [
-        'fsaverage:den-164k',
+        'MNIInfant:cohort-1:res-native',  # Default output space
         'MNI152NLin6Asym:res-2',
     ]
 
     assert [
         format_reference((s.fullname, s.spec))
         for s in spaces.references
         if s.standard and s.dim == 3
-    ] == ['MNI152NLin6Asym_res-2', 'MNIInfant_cohort-1']
+    ] == ['MNIInfant_cohort-1_res-native', 'MNI152NLin6Asym_res-2', 'MNIInfant_cohort-1']
     _reset_config()
 
 
 @pytest.mark.parametrize(
     "master_seed,ants_seed,numpy_seed", [(1, 17612, 8272), (100, 19094, 60232)]
 )
 def test_prng_seed(master_seed, ants_seed, numpy_seed):
@@ -134,7 +123,15 @@
         assert seeds.ants == ants_seed
         assert seeds.numpy == numpy_seed
         assert os.getenv("ANTS_RANDOM_SEED") == str(ants_seed)
 
     _reset_config()
     for seed in ('_random_seed', 'master', 'ants', 'numpy'):
         assert getattr(config.seeds, seed) is None
+
+
+def _load_spaces(age):
+    from nibabies.workflows.base import init_execution_spaces, init_workflow_spaces
+
+    # Conditional based on workflow necessities
+    spaces = init_workflow_spaces(init_execution_spaces(), age)
+    return spaces
```

### Comparing `nibabies-23.0.0/nibabies/utils/bids.py` & `nibabies-23.1.0rc0/nibabies/utils/bids.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # emacs: -*- mode: python; py-indent-offset: 4; indent-tabs-mode: nil -*-
 # vi: set ft=python sts=4 ts=4 sw=4 et:
 """Utilities to handle BIDS inputs."""
 import json
 import os
 import sys
+import warnings
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import IO, List, Union
+from typing import IO, List, Literal, Optional, Union
 
 
 @dataclass
 class BOLDGrouping:
     """This class is used to facilitate the grouping of BOLD series."""
 
     session: Union[str, None]
@@ -258,7 +259,77 @@
             continue
         if len(res) > 1:  # Some queries may want multiple results
             raise Exception(
                 f"When searching for <{deriv}>, found multiple results: {[f.path for f in res]}"
             )
         derivatives[deriv] = res[0]
     return derivatives
+
+
+def parse_bids_for_age_months(
+    bids_root: Union[str, Path],
+    subject_id: str,
+    session_id: Optional[str] = None,
+) -> Optional[int]:
+    """
+    Given a BIDS root, query the BIDS metadata files for participant age, in months.
+
+    The heuristic followed is:
+    1) Check `sub-<subject_id>/sub-<subject_id>_sessions.tsv`
+    2) Check `<root>/participants.tsv`
+    """
+    age = None
+    if subject_id.startswith('sub-'):
+        subject_id = subject_id[4:]
+    if session_id and session_id.startswith('ses-'):
+        session_id = session_id[4:]
+
+    sessions_tsv = Path(bids_root) / f'sub-{subject_id}' / f'sub-{subject_id}_sessions.tsv'
+    if sessions_tsv.exists() and session_id is not None:
+        age = _get_age_from_tsv(sessions_tsv, level='session', key=f'ses-{session_id}')
+
+    participants_tsv = Path(bids_root) / 'participants.tsv'
+    if participants_tsv.exists() and age is None:
+        age = _get_age_from_tsv(participants_tsv, level='participant', key=f'sub-{subject_id}')
+
+    return age
+
+
+def _get_age_from_tsv(
+    bids_tsv: Path, level: Literal['session', 'participant'], key: str
+) -> Optional[int]:
+    import pandas as pd
+
+    df = pd.read_csv(str(bids_tsv), sep='\t')
+    age_col = None
+    # prefer explicit "age_months" over "age"
+    for c in ('age_months', 'age'):
+        if c in df.columns:
+            age_col = c
+            break
+
+    if age_col == 'age':
+        # verify age is in months
+        bids_json = bids_tsv.with_suffix('.json')
+        if not _verify_age_json(bids_json):
+            warnings.warn(f'Could not verify age column is in months for file: {bids_tsv}')
+
+    # find the relevant row
+    if level == 'session':
+        mask = df.session_id == key
+    elif level == 'participant':
+        mask = df.participant_id == key
+
+    try:
+        # extract age value from row
+        age = int(df.loc[mask, age_col].values[0])
+    except Exception:
+        age = None
+    return age
+
+
+def _verify_age_json(bids_json: Path) -> bool:
+    try:
+        data = json.loads(bids_json.read_text())
+        return data['age']['Units'].lower() == 'months'
+    except Exception:
+        return False
```

### Comparing `nibabies-23.0.0/nibabies/utils/confounds.py` & `nibabies-23.1.0rc0/nibabies/utils/confounds.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/utils/filtering.py` & `nibabies-23.1.0rc0/nibabies/utils/filtering.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/utils/misc.py` & `nibabies-23.1.0rc0/nibabies/utils/misc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # emacs: -*- mode: python; py-indent-offset: 4; indent-tabs-mode: nil -*-
 # vi: set ft=python sts=4 ts=4 sw=4 et:
 """Miscellaneous utilities."""
 
+from pathlib import Path
+from typing import Union
+
 from .. import __version__
 
 
 def fix_multi_source_name(in_files):
     """
     Make up a generic source name when there are multiple
     >>> fix_multi_source_name([
     ...     '/path/to/sub-045_ses-test_T1w.nii.gz',
     ...     '/path/to/sub-045_ses-retest_T1w.nii.gz'])
     '/path/to/sub-045_T1w.nii.gz'
     """
     import re
-    from pathlib import Path
 
     from nipype.utils.filemanip import filename_to_list
 
     if not isinstance(in_files, (tuple, list)):
         return in_files
     elif len(in_files) == 1:
         return in_files[0]
@@ -109,7 +111,27 @@
 
     from nipype.utils.filemanip import filename_to_list
 
     base, in_file = os.path.split(filename_to_list(in_files)[0])
     entities = [ent for ent in in_file.split("_") if not ent.startswith("echo-")]
     basename = "_".join(entities)
     return os.path.join(base, basename)
+
+
+def get_file(pkg: str, src_path: Union[str, Path]) -> str:
+    """
+    Get or extract a source file.
+    Assures the file will be available until the lifetime of the current Python process.
+    """
+    import atexit
+    from contextlib import ExitStack
+
+    try:
+        from importlib.resources import as_file, files
+    except ImportError:
+        from importlib_resources import as_file, files
+
+    file_manager = ExitStack()
+    atexit.register(file_manager.close)
+    ref = files(pkg) / str(src_path)
+    fl = file_manager.enter_context(as_file(ref))
+    return str(fl)
```

### Comparing `nibabies-23.0.0/nibabies/utils/telemetry.py` & `nibabies-23.1.0rc0/nibabies/utils/telemetry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import migas
+from nibabel.optpkg import optional_package
 
 from .. import __version__, config
 
+migas = optional_package("migas")[0]
+
 
 def setup_migas(init: bool = True) -> None:
     """
     Prepare the migas python client to communicate with a migas server.
     If ``init`` is ``True``, send an initial breadcrumb.
     """
     # generate session UUID from generated run UUID
```

### Comparing `nibabies-23.0.0/nibabies/utils/validation.py` & `nibabies-23.1.0rc0/nibabies/utils/validation.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/utils/viz.py` & `nibabies-23.1.0rc0/nibabies/utils/viz.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/workflows/base.py` & `nibabies-23.1.0rc0/nibabies/workflows/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,26 +39,28 @@
 .. autofunction:: init_single_subject_wf
 
 """
 
 import os
 import sys
 from copy import deepcopy
+from typing import Optional
 
 from nipype.interfaces import utility as niu
 from nipype.pipeline import engine as pe
 from packaging.version import Version
 
-from .. import config
-from ..interfaces import DerivativesDataSink
-from ..interfaces.reports import AboutSummary, SubjectSummary
-from .bold import init_func_preproc_wf
+from nibabies import config
+from nibabies.interfaces import DerivativesDataSink
+from nibabies.interfaces.reports import AboutSummary, SubjectSummary
+from nibabies.utils.bids import parse_bids_for_age_months
+from nibabies.workflows.bold import init_func_preproc_wf
 
 
-def init_nibabies_wf(participants_table):
+def init_nibabies_wf(subworkflows_list):
     """
     Build *NiBabies*'s pipeline.
 
     This workflow organizes the execution of NiBabies, with a sub-workflow for
     each subject.
 
     If FreeSurfer's ``infant_recon_all`` is to be run, a corresponding folder is created
@@ -72,70 +74,95 @@
             from nibabies.workflows.tests import mock_config
             from nibabies.workflows.base import init_nibabies_wf
             with mock_config():
                 wf = init_nibabies_wf()
 
     Parameters
     ----------
-    participants_table: :obj:`dict`
-        Keys of participant labels and values of the sessions to process.
+    subworkflows_list: :obj:`list` of :obj:`tuple`
+        A list of the subworkflows to create.
+        Each subject session is run as an individual workflow.
     """
     from niworkflows.engine.workflows import LiterateWorkflow as Workflow
     from niworkflows.interfaces.bids import BIDSFreeSurferDir
 
     ver = Version(config.environment.version)
     nibabies_wf = Workflow(name=f"nibabies_{ver.major}_{ver.minor}_wf")
     nibabies_wf.base_dir = config.execution.work_dir
 
+    execution_spaces = init_execution_spaces()
+
     freesurfer = config.workflow.run_reconall
     if freesurfer:
         fsdir = pe.Node(
             BIDSFreeSurferDir(
                 derivatives=config.execution.output_dir,
                 freesurfer_home=os.getenv("FREESURFER_HOME"),
-                spaces=config.workflow.spaces.get_fs_spaces(),
+                spaces=execution_spaces.get_fs_spaces(),
             ),
             name=f"fsdir_run_{config.execution.run_uuid.replace('-', '_')}",
             run_without_submitting=True,
         )
         if config.execution.fs_subjects_dir is not None:
             fsdir.inputs.subjects_dir = str(config.execution.fs_subjects_dir.absolute())
 
-    for subject_id, sessions in participants_table.items():
-        for session_id in sessions:
-            single_subject_wf = init_single_subject_wf(subject_id, session_id=session_id)
-
-            bids_level = [f"sub-{subject_id}"]
-            if session_id:
-                bids_level.append(f"ses-{session_id}")
-
-            log_dir = (
-                config.execution.nibabies_dir.joinpath(*bids_level)
-                / "log"
-                / config.execution.run_uuid
+    for subject_id, session_id in subworkflows_list:
+        # Calculate the age and age-specific spaces
+        age = parse_bids_for_age_months(config.execution.bids_dir, subject_id, session_id)
+        if config.workflow.age_months:
+            config.loggers.cli.warning(
+                "`--age-months` is deprecated and will be removed in a future release."
+                "Please use a `sessions.tsv` or `participants.tsv` file to track participants age."
             )
-
-            single_subject_wf.config["execution"]["crashdump_dir"] = str(log_dir)
-            for node in single_subject_wf._get_all_nodes():
-                node.config = deepcopy(single_subject_wf.config)
-            if freesurfer:
-                nibabies_wf.connect(
-                    fsdir, "subjects_dir", single_subject_wf, "inputnode.subjects_dir"
+            age = config.workflow.age_months
+        if age is None:
+            raise RuntimeError(
+                "Could not find age for sub-{subject}{session}".format(
+                    subject=subject_id, session=f'_ses-{session_id}' if session_id else ''
                 )
-            else:
-                nibabies_wf.add_nodes([single_subject_wf])
+            )
+        output_spaces = init_workflow_spaces(execution_spaces, age)
+
+        # skull strip template cohort
+        single_subject_wf = init_single_subject_wf(
+            subject_id,
+            session_id=session_id,
+            age=age,
+            spaces=output_spaces,
+        )
+
+        bids_level = [f"sub-{subject_id}"]
+        if session_id:
+            bids_level.append(f"ses-{session_id}")
+
+        log_dir = (
+            config.execution.nibabies_dir.joinpath(*bids_level) / "log" / config.execution.run_uuid
+        )
 
-            # Dump a copy of the config file into the log directory
-            log_dir.mkdir(exist_ok=True, parents=True)
-            config.to_filename(log_dir / "nibabies.toml")
+        single_subject_wf.config["execution"]["crashdump_dir"] = str(log_dir)
+        for node in single_subject_wf._get_all_nodes():
+            node.config = deepcopy(single_subject_wf.config)
+        if freesurfer:
+            nibabies_wf.connect(fsdir, "subjects_dir", single_subject_wf, "inputnode.subjects_dir")
+        else:
+            nibabies_wf.add_nodes([single_subject_wf])
+
+        # Dump a copy of the config file into the log directory
+        log_dir.mkdir(exist_ok=True, parents=True)
+        config.to_filename(log_dir / "nibabies.toml")
 
     return nibabies_wf
 
 
-def init_single_subject_wf(subject_id, session_id=None):
+def init_single_subject_wf(
+    subject_id: str,
+    session_id: Optional[str] = None,
+    age: Optional[int] = None,
+    spaces=None,
+):
     """
     Organize the preprocessing pipeline for a single subject, at a single session.
 
     It collects and reports information about the subject, and prepares
     sub-workflows to perform anatomical and functional preprocessing.
     Anatomical preprocessing is performed in a single workflow, regardless of
     the number of sessions.
@@ -154,14 +181,16 @@
 
     Parameters
     ----------
     subject_id : :obj:`str`
         Subject label for this single-subject workflow.
     session_id : :obj:`str` or None
         Session identifier.
+    age: :obj:`int` or None
+        Age (in months) of subject.
 
     Inputs
     ------
     subjects_dir : :obj:`str`
         FreeSurfer's ``$SUBJECTS_DIR``.
 
     """
@@ -192,15 +221,14 @@
         subject_data["flair"] = []
     if "t2w" in config.workflow.ignore:
         subject_data["t2w"] = []
 
     anat_only = config.workflow.anat_only
     derivatives = config.execution.derivatives or {}
     anat_modality = "t1w" if subject_data["t1w"] else "t2w"
-    spaces = config.workflow.spaces
     # Make sure we always go through these two checks
     if not anat_only and not subject_data["bold"]:
         task_id = config.execution.task_id
         raise RuntimeError(
             "No BOLD images found for participant {} and task {}. "
             "All workflows require BOLD images.".format(
                 subject_id, task_id if task_id else "<all>"
@@ -311,15 +339,15 @@
         name="ds_report_about",
         run_without_submitting=True,
     )
 
     # Preprocessing of anatomical (includes registration to UNCInfant)
     anat_preproc_wf = init_infant_anat_wf(
         ants_affine_init=True,
-        age_months=config.workflow.age_months,
+        age_months=age,
         anat_modality=anat_modality,
         t1w=subject_data["t1w"],
         t2w=subject_data["t2w"],
         bids_root=config.execution.bids_dir,
         existing_derivatives=derivatives,
         freesurfer=config.workflow.run_reconall,
         hires=config.workflow.hires,
@@ -327,14 +355,15 @@
         omp_nthreads=config.nipype.omp_nthreads,
         output_dir=nibabies_dir,
         segmentation_atlases=config.execution.segmentation_atlases_dir,
         skull_strip_mode=config.workflow.skull_strip_t1w,
         skull_strip_template=Reference.from_string(config.workflow.skull_strip_template)[0],
         sloppy=config.execution.sloppy,
         spaces=spaces,
+        cifti_output=config.workflow.cifti_output,
     )
 
     # fmt: off
     workflow.connect([
         (inputnode, anat_preproc_wf, [
             ('subjects_dir', 'inputnode.subjects_dir'),
         ]),
@@ -414,15 +443,15 @@
 
 : For each of the {len(subject_data['bold'])} BOLD runs found per subject (across all
 tasks and sessions), the following preprocessing was performed."""
 
     func_preproc_wfs = []
     has_fieldmap = bool(fmap_estimators)
     for bold_file in subject_data['bold']:
-        func_preproc_wf = init_func_preproc_wf(bold_file, has_fieldmap=has_fieldmap)
+        func_preproc_wf = init_func_preproc_wf(bold_file, spaces, has_fieldmap=has_fieldmap)
         if func_preproc_wf is None:
             continue
 
         func_preproc_wf.__desc__ = func_pre_desc + (getattr(func_preproc_wf, '__desc__') or '')
         # fmt:off
         workflow.connect([
             (anat_preproc_wf, func_preproc_wf, [
@@ -437,14 +466,19 @@
                 ('outputnode.anat2std_xfm', 'inputnode.anat2std_xfm'),
                 ('outputnode.std2anat_xfm', 'inputnode.std2anat_xfm'),
                 # Undefined if --fs-no-reconall, but this is safe
                 ('outputnode.subjects_dir', 'inputnode.subjects_dir'),
                 ('outputnode.subject_id', 'inputnode.subject_id'),
                 ('outputnode.t1w2fsnative_xfm', 'inputnode.t1w2fsnative_xfm'),
                 ('outputnode.fsnative2t1w_xfm', 'inputnode.fsnative2t1w_xfm'),
+                ('outputnode.surfaces', 'inputnode.surfaces'),
+                ('outputnode.morphometrics', 'inputnode.morphometrics'),
+                ('outputnode.anat_ribbon', 'inputnode.anat_ribbon'),
+                ('outputnode.sphere_reg_fsLR', 'inputnode.sphere_reg_fsLR'),
+                ('outputnode.midthickness_fsLR', 'inputnode.midthickness_fsLR'),
             ]),
         ])
         # fmt:on
         func_preproc_wfs.append(func_preproc_wf)
 
     if not has_fieldmap:
         config.loggers.workflow.warning(
@@ -520,12 +554,57 @@
     return workflow
 
 
 def _prefix(subid):
     return subid if subid.startswith("sub-") else f"sub-{subid}"
 
 
-def _select_iter_idx(in_list, idx):
-    """Returns a specific index of a list/tuple"""
-    if isinstance(in_list, (tuple, list)):
-        return in_list[idx]
-    raise AttributeError(f"Input {in_list} is incompatible type: {type(in_list)}")
+def init_workflow_spaces(execution_spaces, age_months):
+    """
+    Create output spaces at a per-subworkflow level.
+
+    This address the case where a multi-session subject is run, and requires separate template cohorts.
+    """
+    from niworkflows.utils.spaces import Reference
+
+    from nibabies.utils.misc import cohort_by_months
+
+    spaces = deepcopy(execution_spaces)
+
+    if age_months is None:
+        raise RuntimeError("Participant age (in months) is required.")
+
+    if not spaces.references:
+        # Ensure age specific template is added if nothing is present
+        cohort = cohort_by_months("MNIInfant", age_months)
+        spaces.add(("MNIInfant", {"res": "native", "cohort": cohort}))
+
+    if not spaces.is_cached():
+        spaces.checkpoint()
+
+    # Ensure user-defined spatial references for outputs are correctly parsed.
+    # Certain options require normalization to a space not explicitly defined by users.
+    # These spaces will not be included in the final outputs.
+    if config.workflow.use_aroma:
+        # Make sure there's a normalization to FSL for AROMA to use.
+        spaces.add(Reference("MNI152NLin6Asym", {"res": "2"}))
+
+    if config.workflow.cifti_output:
+        # CIFTI grayordinates to corresponding FSL-MNI resolutions.
+        vol_res = "2" if config.workflow.cifti_output == "91k" else "1"
+        spaces.add(Reference("MNI152NLin6Asym", {"res": vol_res}))
+        # Ensure a non-native version of MNIInfant is added as a target
+        cohort = cohort_by_months("MNIInfant", age_months)
+        spaces.add(Reference("MNIInfant", {"cohort": cohort}))
+
+    return spaces
+
+
+def init_execution_spaces():
+    from niworkflows.utils.spaces import Reference, SpatialReferences
+
+    spaces = config.execution.output_spaces or SpatialReferences()
+    if not isinstance(spaces, SpatialReferences):
+        spaces = SpatialReferences(
+            [ref for s in spaces.split(" ") for ref in Reference.from_string(s)]
+        )
+    return spaces
```

### Comparing `nibabies-23.0.0/nibabies/workflows/anatomical/base.py` & `nibabies-23.1.0rc0/nibabies/workflows/anatomical/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 """Base anatomical preprocessing."""
+import warnings
+from pathlib import Path
+from typing import Literal, Optional, Union
+
 from nipype.interfaces import utility as niu
 from nipype.pipeline import engine as pe
+from niworkflows.engine.workflows import LiterateWorkflow
+from niworkflows.utils.spaces import Reference, SpatialReferences
 
 from ... import config
 
 
 def init_infant_anat_wf(
     *,
-    age_months,
-    ants_affine_init,
-    t1w,
-    t2w,
-    anat_modality,
-    bids_root,
-    existing_derivatives,
-    freesurfer,
-    hires,
-    longitudinal,
-    omp_nthreads,
-    output_dir,
-    segmentation_atlases,
-    skull_strip_mode,
-    skull_strip_template,
-    sloppy,
-    spaces,
-    name="infant_anat_wf",
-):
+    age_months: Optional[int],
+    ants_affine_init: bool,
+    t1w: list,
+    t2w: list,
+    anat_modality: str,
+    bids_root: Optional[Union[str, Path]],
+    existing_derivatives: dict,
+    freesurfer: bool,
+    hires: Optional[bool],
+    longitudinal: bool,
+    omp_nthreads: int,
+    output_dir: Union[str, Path],
+    segmentation_atlases: Optional[Union[str, Path]],
+    skull_strip_mode: str,
+    skull_strip_template: Reference,
+    sloppy: bool,
+    spaces: Optional[SpatialReferences],
+    cifti_output: Optional[Literal['91k', '170k']],
+    name: str = "infant_anat_wf",
+) -> LiterateWorkflow:
     """
 
       - T1w reference: realigning and then averaging anatomical images.
       - Brain extraction and INU (bias field) correction.
       - Brain tissue segmentation.
       - Spatial normalization to standard spaces.
       - Surface reconstruction with FreeSurfer_.
@@ -72,52 +79,57 @@
     fsnative2t1w_xfm
         LTA-style affine matrix translating from FreeSurfer-conformed
         subject space to T1w
     surfaces
         GIFTI surfaces (gray/white boundary, midthickness, pial, inflated)
     """
     from nipype.interfaces.ants.base import Info as ANTsInfo
-    from niworkflows.engine.workflows import LiterateWorkflow as Workflow
-    from sdcflows.workflows.ancillary import (
-        init_brainextraction_wf as init_sdc_brain_extraction_wf,
-    )
+    from smriprep.workflows.norm import init_anat_norm_wf
 
     from ...utils.misc import fix_multi_source_name
-    from .brain_extraction import (
-        init_infant_brain_extraction_wf,
-        init_precomputed_mask_wf,
-    )
-    from .norm import init_anat_norm_wf
+    from .brain_extraction import init_infant_brain_extraction_wf
     from .outputs import (
         init_anat_derivatives_wf,
         init_anat_reports_wf,
         init_coreg_report_wf,
     )
-    from .preproc import init_anat_average_wf
+    from .preproc import init_anat_preproc_wf
     from .registration import init_coregistration_wf
     from .segmentation import init_anat_segmentations_wf
+    from .surfaces import init_anat_ribbon_wf
+    from .template import init_anat_template_wf
 
     # for now, T1w only
     num_t1w = len(t1w) if t1w else 0
     num_t2w = len(t2w) if t2w else 0
 
     precomp_mask = existing_derivatives.get("anat_mask")
     precomp_aseg = existing_derivatives.get("anat_aseg")
 
     # verify derivatives are relatively similar to T1w
     if precomp_mask or precomp_aseg:
-        from ...utils.validation import validate_t1w_derivatives
-
-        validated_derivatives = validate_t1w_derivatives(  # compare derivatives to the first T1w
-            t1w[0], anat_mask=precomp_mask, anat_aseg=precomp_aseg
-        )
-        precomp_mask = validated_derivatives.get("anat_mask")
-        precomp_aseg = validated_derivatives.get("anat_aseg")
+        if num_t1w > 1:
+            precomp_mask = None
+            precomp_aseg = None
+            warnings.warn(
+                "Multiple T1w files were found; precomputed derivatives will not be used."
+            )
+
+        else:
+            from ...utils.validation import validate_t1w_derivatives
+
+            validated_derivatives = (
+                validate_t1w_derivatives(  # compare derivatives to the first T1w
+                    t1w[0], anat_mask=precomp_mask, anat_aseg=precomp_aseg
+                )
+            )
+            precomp_mask = validated_derivatives.get("anat_mask")
+            precomp_aseg = validated_derivatives.get("anat_aseg")
 
-    wf = Workflow(name=name)
+    wf = LiterateWorkflow(name=name)
     desc = f"""\n
 Anatomical data preprocessing
 
 : A total of {num_t1w} T1w and {num_t2w} T2w images were found within the input
 BIDS dataset."""
 
     inputnode = pe.Node(
@@ -142,27 +154,33 @@
                 "anat2std_xfm",
                 "std2anat_xfm",
                 "t1w2fsnative_xfm",
                 "fsnative2t1w_xfm",
                 "surfaces",
                 "morphometrics",
                 "anat_aseg",
+                "anat_mcrib",
                 "anat_aparc",
+                "anat_ribbon",
                 "template",
+                # registration sphere space is dependent on surface recon method
+                "sphere_reg",
+                "sphere_reg_fsLR",
+                "midthickness_fsLR",
             ]
         ),
         name="outputnode",
     )
 
     desc += (
         """\
-All of the T1-weighted images were corrected for intensity non-uniformity (INU)"""
+All of the T1-weighted images were denoised and corrected for intensity non-uniformity (INU)"""
         if num_t1w > 1
         else """\
-The T1-weighted (T1w) image was corrected for intensity non-uniformity (INU)"""
+The T1-weighted (T1w) image was denoised and corrected for intensity non-uniformity (INU)"""
     )
 
     desc += """\
 with `N4BiasFieldCorrection` [@n4], distributed with ANTs {ants_ver} \
 [@ants, RRID:SCR_004757]"""
     desc += ".\n" if num_t1w > 1 else ", and used as T1w-reference throughout the workflow.\n"
 
@@ -189,63 +207,61 @@
 
     anat_derivatives_wf = init_anat_derivatives_wf(
         bids_root=bids_root,
         freesurfer=freesurfer,
         num_t1w=num_t1w,
         output_dir=output_dir,
         spaces=spaces,
+        cifti_output=cifti_output,
     )
 
-    # Multiple T1w files -> generate average reference
-    t1w_template_wf = init_anat_average_wf(
+    # Multiple anatomical files -> generate average reference
+    t1w_template_wf = init_anat_template_wf(
+        contrast="T1w",
+        num_files=num_t1w,
         longitudinal=longitudinal,
         omp_nthreads=omp_nthreads,
-        num_maps=num_t1w,
+        sloppy=sloppy,
         name="t1w_template_wf",
     )
 
-    t2w_template_wf = init_anat_average_wf(
+    t2w_template_wf = init_anat_template_wf(
+        contrast="T2w",
+        num_files=num_t2w,
         longitudinal=longitudinal,
         omp_nthreads=omp_nthreads,
-        num_maps=num_t2w,
+        sloppy=sloppy,
         name="t2w_template_wf",
     )
 
-    # INU + Brain Extraction
+    # Clean up each anatomical template
+    # Denoise, INU, + Clipping
+    t1w_preproc_wf = init_anat_preproc_wf(
+        precomputed_mask=bool(precomp_mask),
+        precomputed_aseg=bool(precomp_aseg),
+        name="t1w_preproc_wf",
+    )
+    t2w_preproc_wf = init_anat_preproc_wf(name="t2w_preproc_wf")
+
     if skull_strip_mode != "force":
         raise NotImplementedError("Skull stripping is currently required.")
 
-    if precomp_mask:
-        precomp_mask_wf = init_precomputed_mask_wf(omp_nthreads=omp_nthreads)
-        precomp_mask_wf.inputs.inputnode.t1w_mask = precomp_mask
-        sdc_brain_extraction_wf = init_sdc_brain_extraction_wf(
-            name="sdc_brain_extraction_wf",
-        )
-    brain_extraction_wf = init_infant_brain_extraction_wf(
-        age_months=age_months,
-        ants_affine_init=ants_affine_init,
-        skull_strip_template=skull_strip_template.space,
-        template_specs=skull_strip_template.spec,
-        omp_nthreads=omp_nthreads,
-        sloppy=sloppy,
-        debug="registration" in config.execution.debug,
-    )
     coregistration_wf = init_coregistration_wf(
         omp_nthreads=omp_nthreads,
         sloppy=sloppy,
         debug="registration" in config.execution.debug,
+        precomputed_mask=bool(precomp_mask),
     )
     coreg_report_wf = init_coreg_report_wf(
         output_dir=output_dir,
     )
-    t1w_preproc_wf = precomp_mask_wf if precomp_mask else coregistration_wf
 
     # Segmentation - initial implementation should be simple: JLF
     anat_seg_wf = init_anat_segmentations_wf(
-        anat_modality=anat_modality.capitalize(),
+        anat_modality=anat_modality.capitalize(),  # TODO: Revisit this option
         template_dir=segmentation_atlases,
         sloppy=sloppy,
         omp_nthreads=omp_nthreads,
         precomp_aseg=precomp_aseg,
     )
 
     # Spatial normalization (requires segmentation)
@@ -253,195 +269,273 @@
         sloppy=sloppy,
         omp_nthreads=omp_nthreads,
         templates=spaces.get_spaces(nonstandard=False, dim=(3,)),
     )
 
     # fmt:off
     wf.connect([
-        (inputnode, t1w_template_wf, [("t1w", "inputnode.in_files")]),
+        (inputnode, t1w_template_wf, [("t1w", "inputnode.anat_files")]),
+        (inputnode, t2w_template_wf, [("t2w", "inputnode.anat_files")]),
+        (inputnode, anat_reports_wf, [("t1w", "inputnode.source_file")]),
+        (inputnode, coreg_report_wf, [("t1w", "inputnode.source_file")]),
+        (inputnode, anat_norm_wf, [(("t1w", fix_multi_source_name), "inputnode.orig_t1w")]),
+
         (t1w_template_wf, outputnode, [
-            ("outputnode.realign_xfms", "anat_ref_xfms"),
+            ("outputnode.anat_realign_xfm", "anat_ref_xfms")]),
+        (t1w_template_wf, t1w_preproc_wf, [("outputnode.anat_ref", "inputnode.in_anat")]),
+        (t1w_template_wf, anat_derivatives_wf, [
+            ("outputnode.anat_valid_list", "inputnode.source_files"),
+            ("outputnode.anat_realign_xfm", "inputnode.t1w_ref_xfms")]),
+        (t1w_template_wf, anat_reports_wf, [
+            ("outputnode.out_report", "inputnode.t1w_conform_report")]),
+
+        (t2w_template_wf, t2w_preproc_wf, [("outputnode.anat_ref", "inputnode.in_anat")]),
+        (t2w_template_wf, anat_derivatives_wf, [
+            ("outputnode.anat_valid_list", "inputnode.t2w_source_files")]),
+
+        (t1w_preproc_wf, coregistration_wf, [("outputnode.anat_preproc", "inputnode.in_t1w")]),
+        (t1w_preproc_wf, coreg_report_wf, [("outputnode.anat_preproc", "inputnode.t1w_preproc")]),
+
+        (coregistration_wf, coreg_report_wf, [
+            ("outputnode.t1w_mask", "inputnode.in_mask"),
+            ("outputnode.t2w_preproc", "inputnode.t2w_preproc")]),
+        (coregistration_wf, anat_norm_wf, [
+            ("outputnode.t1w_preproc", "inputnode.moving_image"),
+            ("outputnode.t1w_mask", "inputnode.moving_mask")]),
+        (coregistration_wf, anat_seg_wf, [("outputnode.t1w_brain", "inputnode.anat_brain")]),
+        (coregistration_wf, anat_derivatives_wf, [
+            ("outputnode.t1w_mask", "inputnode.t1w_mask"),
+            ("outputnode.t1w_preproc", "inputnode.t1w_preproc"),
+            ("outputnode.t2w_preproc", "inputnode.t2w_preproc"),
+         ]),
+        (coregistration_wf, outputnode, [
+            ("outputnode.t1w_preproc", "anat_preproc"),
+            ("outputnode.t1w_brain", "anat_brain"),
+            ("outputnode.t1w_mask", "anat_mask"),
         ]),
+
         (anat_seg_wf, outputnode, [
             ("outputnode.anat_dseg", "anat_dseg"),
-            ("outputnode.anat_tpms", "anat_tpms"),
+            ("outputnode.anat_tpms", "anat_tpms")]),
+        (anat_seg_wf, anat_derivatives_wf, [
+            ("outputnode.anat_dseg", "inputnode.t1w_dseg"),
+            ("outputnode.anat_tpms", "inputnode.t1w_tpms"),
         ]),
         (anat_seg_wf, anat_norm_wf, [
             ("outputnode.anat_dseg", "inputnode.moving_segmentation"),
-            ("outputnode.anat_tpms", "inputnode.moving_tpms"),
-        ]),
+            ("outputnode.anat_tpms", "inputnode.moving_tpms")]),
+
+        (anat_norm_wf, anat_reports_wf, [("poutputnode.template", "inputnode.template")]),
         (anat_norm_wf, outputnode, [
             ("poutputnode.standardized", "std_preproc"),
             ("poutputnode.std_mask", "std_mask"),
             ("poutputnode.std_dseg", "std_dseg"),
             ("poutputnode.std_tpms", "std_tpms"),
             ("outputnode.template", "template"),
             ("outputnode.anat2std_xfm", "anat2std_xfm"),
-            ("outputnode.std2anat_xfm", "std2anat_xfm"),
-        ]),
-        (inputnode, anat_norm_wf, [
-            (("t1w", fix_multi_source_name), "inputnode.orig_t1w"),  # anat_validate? not used...
-        ]),
-        (t1w_preproc_wf, anat_norm_wf, [
-            ("outputnode.t1w_preproc", "inputnode.moving_image"),
-            ("outputnode.t1w_mask", "inputnode.moving_mask"),
-        ]),
-        (t1w_preproc_wf, anat_derivatives_wf, [
-            ("outputnode.t1w_mask", "inputnode.t1w_mask"),
-            ("outputnode.t1w_preproc", "inputnode.t1w_preproc"),
-        ]),
-        (coregistration_wf, anat_derivatives_wf, [
-            ("outputnode.t2w_preproc", "inputnode.t2w_preproc")
-         ]),
-        (t1w_preproc_wf, outputnode, [
-            ("outputnode.t1w_preproc", "anat_preproc"),
-            ("outputnode.t1w_brain", "anat_brain"),
-            ("outputnode.t1w_mask", "anat_mask"),
+            ("outputnode.std2anat_xfm", "std2anat_xfm")]),
+        (anat_norm_wf, anat_derivatives_wf, [
+            ("outputnode.template", "inputnode.template"),
+            ("outputnode.anat2std_xfm", "inputnode.anat2std_xfm"),
+            ("outputnode.std2anat_xfm", "inputnode.std2anat_xfm")]),
+
+        (outputnode, anat_reports_wf, [
+            ("anat_preproc", "inputnode.t1w_preproc"),
+            ("anat_mask", "inputnode.t1w_mask"),
+            ("anat_dseg", "inputnode.t1w_dseg"),
+            ("std_preproc", "inputnode.std_t1w"),
+            ("std_mask", "inputnode.std_mask"),
         ]),
     ])
 
-    if not precomp_aseg:
-        wf.connect([
-            (t1w_preproc_wf, anat_seg_wf, [("outputnode.t1w_brain", "inputnode.anat_brain")]),
-        ])
-    wf.connect([
-        (inputnode, t2w_template_wf, [("t2w", "inputnode.in_files")]),
-    ])
     if precomp_mask:
+        # Ensure the mask is conformed along with the T1w
+        t1w_preproc_wf.inputs.inputnode.in_mask = precomp_mask
+        # fmt:off
         wf.connect([
-            (t1w_template_wf, precomp_mask_wf, [
-                ("outputnode.out_file", "inputnode.t1w"),
-            ]),
-            (t2w_template_wf, sdc_brain_extraction_wf, [
-                ("outputnode.out_file", "inputnode.in_file"),
-            ]),
-            (sdc_brain_extraction_wf, coregistration_wf, [
-                ("outputnode.out_file", "inputnode.in_t2w_preproc"),
-                ("outputnode.out_mask", "inputnode.in_mask"),
-                ("outputnode.out_probseg", "inputnode.in_probmap"),
-            ]),
+            (t1w_preproc_wf, coregistration_wf, [("outputnode.anat_mask", "inputnode.in_mask")]),
+            (t2w_preproc_wf, coregistration_wf, [("outputnode.anat_preproc", "inputnode.in_t2w")])
         ])
+        # fmt:on
     else:
+        # Run brain extraction on the T2w
+        brain_extraction_wf = init_infant_brain_extraction_wf(
+            age_months=age_months,
+            ants_affine_init=ants_affine_init,
+            skull_strip_template=skull_strip_template.space,
+            template_specs=skull_strip_template.spec,
+            omp_nthreads=omp_nthreads,
+            sloppy=sloppy,
+            debug="registration" in config.execution.debug,
+        )
+        # fmt:off
         wf.connect([
-            (t2w_template_wf, brain_extraction_wf, [
-                ("outputnode.out_file", "inputnode.in_t2w"),
-            ]),
+            (t2w_preproc_wf, brain_extraction_wf, [
+                ("outputnode.anat_preproc", "inputnode.t2w_preproc")]),
             (brain_extraction_wf, coregistration_wf, [
-                ("outputnode.t2w_preproc", "inputnode.in_t2w_preproc"),
+                ("outputnode.t2w_preproc", "inputnode.in_t2w"),
                 ("outputnode.out_mask", "inputnode.in_mask"),
-                ("outputnode.out_probmap", "inputnode.in_probmap"),
-            ]),
+                ("outputnode.out_probmap", "inputnode.in_probmap")]),
         ])
-    wf.connect([
-        (t1w_template_wf, coregistration_wf, [
-            ("outputnode.out_file", "inputnode.in_t1w"),
-        ]),
-
-        (inputnode, coreg_report_wf, [
-            ("t1w", "inputnode.source_file"),
-        ]),
-        (t1w_preproc_wf, coreg_report_wf, [
-            ("outputnode.t1w_preproc", "inputnode.t1w_preproc"),
-            ("outputnode.t1w_mask", "inputnode.in_mask"),
-        ]),
-        (coregistration_wf, coreg_report_wf, [
-            ("outputnode.t2w_preproc", "inputnode.t2w_preproc")
-        ]),
-    ])
+        # fmt:on
 
-    wf.connect([
-        # reports
-        (inputnode, anat_reports_wf, [
-            ("t1w", "inputnode.source_file"),
-        ]),
-        (outputnode, anat_reports_wf, [
-            ("anat_preproc", "inputnode.t1w_preproc"),
-            ("anat_mask", "inputnode.t1w_mask"),
-            ("anat_dseg", "inputnode.t1w_dseg"),
-            ("std_preproc", "inputnode.std_t1w"),
-            ("std_mask", "inputnode.std_mask"),
-        ]),
-        (t1w_template_wf, anat_reports_wf, [
-            ("outputnode.out_report", "inputnode.t1w_conform_report"),
-        ]),
-        (anat_norm_wf, anat_reports_wf, [
-            ("poutputnode.template", "inputnode.template"),
-        ]),
-        # derivatives
-        (t1w_template_wf, anat_derivatives_wf, [
-            ("outputnode.valid_list", "inputnode.source_files"),
-            ("outputnode.realign_xfms", "inputnode.t1w_ref_xfms"),
-        ]),
-        (t2w_template_wf, anat_derivatives_wf, [
-            ("outputnode.valid_list", "inputnode.t2w_source_files"),
-        ]),
-        (anat_norm_wf, anat_derivatives_wf, [
-            ("outputnode.template", "inputnode.template"),
-            ("outputnode.anat2std_xfm", "inputnode.anat2std_xfm"),
-            ("outputnode.std2anat_xfm", "inputnode.std2anat_xfm"),
-        ]),
-        (anat_seg_wf, anat_derivatives_wf, [
-            ("outputnode.anat_dseg", "inputnode.t1w_dseg"),
-            ("outputnode.anat_tpms", "inputnode.t1w_tpms"),
-        ]),
-    ])
-    # fmt:on
+    if precomp_aseg:
+        # Ensure the segmentation is conformed along with the T1w
+        t1w_preproc_wf.inputs.inputnode.in_aseg = precomp_aseg
+        wf.connect(t1w_preproc_wf, "outputnode.anat_aseg", anat_seg_wf, "inputnode.anat_aseg")
 
     if not freesurfer:
         return wf
 
-    if config.workflow.force_reconall:
+    if config.workflow.surface_recon_method == 'freesurfer':
         from smriprep.workflows.surfaces import init_surface_recon_wf
 
         surface_recon_wf = init_surface_recon_wf(omp_nthreads=omp_nthreads, hires=hires)
-    else:
-        from .surfaces import init_infant_surface_recon_wf
+    elif config.workflow.surface_recon_method == 'infantfs':
+        from .surfaces import init_infantfs_surface_recon_wf
 
         # if running with precomputed aseg, or JLF, pass the aseg along to FreeSurfer
         use_aseg = bool(precomp_aseg or segmentation_atlases)
-        surface_recon_wf = init_infant_surface_recon_wf(
+        surface_recon_wf = init_infantfs_surface_recon_wf(
             age_months=age_months,
             use_aseg=use_aseg,
         )
 
+    elif config.workflow.surface_recon_method == 'mcribs':
+        from nipype.interfaces.ants import DenoiseImage
+
+        from .surfaces import init_mcribs_sphere_reg_wf, init_mcribs_surface_recon_wf
+
+        # Denoise raw T2w, since using the template / preproc resulted in intersection errors
+        denoise_raw_t2w = pe.Node(
+            DenoiseImage(dimension=3, noise_model="Rician"), name='denoise_raw_t2w'
+        )
+
+        surface_recon_wf = init_mcribs_surface_recon_wf(
+            omp_nthreads=omp_nthreads,
+            use_aseg=bool(precomp_aseg),
+            use_mask=bool(precomp_mask),
+            mcribs_dir=str(config.execution.mcribs_dir),  # Needed to preserve runs
+        )
+
+        # M-CRIB-S to dHCP42week (32k)
+        sphere_reg_wf = init_mcribs_sphere_reg_wf()
+
+        # Transformed gives
+        if precomp_aseg:
+            surface_recon_wf.inputs.inputnode.ants_segs = precomp_aseg
+        if precomp_mask:
+            surface_recon_wf.inputs.inputnode.anat_mask = precomp_mask
+        # fmt:off
+        wf.connect([
+            (inputnode, denoise_raw_t2w, [('t2w', 'input_image')]),
+            (denoise_raw_t2w, surface_recon_wf, [('output_image', 'inputnode.t2w')]),
+        ])
+        # fmt:on
+    else:
+        raise NotImplementedError
+
+    if config.workflow.surface_recon_method in ('freesurfer', 'infantfs'):
+        from smriprep.workflows.surfaces import init_sphere_reg_wf
+
+        # fsaverage to fsLR
+        sphere_reg_wf = init_sphere_reg_wf()
+
+        # fmt:off
+        wf.connect([
+            (t2w_preproc_wf, surface_recon_wf, [
+                ("outputnode.anat_preproc", "inputnode.t2w")]),
+            (anat_seg_wf, surface_recon_wf, [
+                ("outputnode.anat_aseg", "inputnode.ants_segs")]),
+        ])
+        # fmt:on
+
+    # Anatomical ribbon file using HCP signed-distance volume method
+    anat_ribbon_wf = init_anat_ribbon_wf()
+
     # fmt:off
     wf.connect([
         (inputnode, surface_recon_wf, [
             ("subject_id", "inputnode.subject_id"),
-            ("subjects_dir", "inputnode.subjects_dir"),
-            ("t2w", "inputnode.t2w"),
-        ]),
-        (anat_seg_wf, surface_recon_wf, [
-            ("outputnode.anat_aseg", "inputnode.ants_segs"),
-        ]),
+            ("subjects_dir", "inputnode.subjects_dir")]),
         (t1w_template_wf, surface_recon_wf, [
-            ("outputnode.out_file", "inputnode.t1w"),
+            ("outputnode.anat_ref", "inputnode.t1w"),
         ]),
-        (t1w_preproc_wf, surface_recon_wf, [
+        (coregistration_wf, surface_recon_wf, [
             ("outputnode.t1w_brain", "inputnode.skullstripped_t1"),
             ("outputnode.t1w_preproc", "inputnode.corrected_t1"),
         ]),
         (surface_recon_wf, outputnode, [
             ("outputnode.subjects_dir", "subjects_dir"),
             ("outputnode.subject_id", "subject_id"),
             ("outputnode.t1w2fsnative_xfm", "t1w2fsnative_xfm"),
             ("outputnode.fsnative2t1w_xfm", "fsnative2t1w_xfm"),
             ("outputnode.surfaces", "surfaces"),
             ("outputnode.morphometrics", "morphometrics"),
             ("outputnode.out_aparc", "anat_aparc"),
             ("outputnode.out_aseg", "anat_aseg"),
         ]),
+        (coregistration_wf, anat_ribbon_wf, [
+            ("outputnode.t1w_mask", "inputnode.t1w_mask"),
+        ]),
+        (surface_recon_wf, anat_ribbon_wf, [
+            ("outputnode.surfaces", "inputnode.surfaces"),
+        ]),
+        (anat_ribbon_wf, outputnode, [
+            ("outputnode.anat_ribbon", "anat_ribbon")
+        ]),
+        (anat_ribbon_wf, anat_derivatives_wf, [
+            ("outputnode.anat_ribbon", "inputnode.anat_ribbon"),
+        ]),
+        (surface_recon_wf, sphere_reg_wf, [
+            ('outputnode.subject_id', 'inputnode.subject_id'),
+            ('outputnode.subjects_dir', 'inputnode.subjects_dir'),
+        ]),
         (surface_recon_wf, anat_reports_wf, [
             ("outputnode.subject_id", "inputnode.subject_id"),
             ("outputnode.subjects_dir", "inputnode.subjects_dir"),
         ]),
         (surface_recon_wf, anat_derivatives_wf, [
             ("outputnode.out_aseg", "inputnode.t1w_fs_aseg"),
             ("outputnode.out_aparc", "inputnode.t1w_fs_aparc"),
             ("outputnode.t1w2fsnative_xfm", "inputnode.t1w2fsnative_xfm"),
             ("outputnode.fsnative2t1w_xfm", "inputnode.fsnative2t1w_xfm"),
             ("outputnode.surfaces", "inputnode.surfaces"),
             ("outputnode.morphometrics", "inputnode.morphometrics"),
         ]),
+        (sphere_reg_wf, outputnode, [
+            ('outputnode.sphere_reg', 'sphere_reg'),
+            ('outputnode.sphere_reg_fsLR', 'sphere_reg_fsLR')]),
+        (sphere_reg_wf, anat_derivatives_wf, [
+            ('outputnode.sphere_reg', 'inputnode.sphere_reg'),
+            ('outputnode.sphere_reg_fsLR', 'inputnode.sphere_reg_fsLR')]),
     ])
     # fmt: on
+
+    if cifti_output:
+        from nibabies.workflows.anatomical.resampling import (
+            init_anat_fsLR_resampling_wf,
+        )
+
+        is_mcribs = config.workflow.surface_recon_method == "mcribs"
+        # handles morph_grayords_wf
+        anat_fsLR_resampling_wf = init_anat_fsLR_resampling_wf(cifti_output, mcribs=is_mcribs)
+        anat_derivatives_wf.get_node('inputnode').inputs.cifti_density = cifti_output
+        # fmt:off
+        wf.connect([
+            (sphere_reg_wf, anat_fsLR_resampling_wf, [
+                ('outputnode.sphere_reg', 'inputnode.sphere_reg'),
+                ('outputnode.sphere_reg_fsLR', 'inputnode.sphere_reg_fsLR')]),
+            (surface_recon_wf, anat_fsLR_resampling_wf, [
+                ('outputnode.subject_id', 'inputnode.subject_id'),
+                ('outputnode.subjects_dir', 'inputnode.subjects_dir'),
+                ('outputnode.surfaces', 'inputnode.surfaces'),
+                ('outputnode.morphometrics', 'inputnode.morphometrics')]),
+            (anat_fsLR_resampling_wf, anat_derivatives_wf, [
+                ("outputnode.cifti_morph", "inputnode.cifti_morph"),
+                ("outputnode.cifti_metadata", "inputnode.cifti_metadata")]),
+            (anat_fsLR_resampling_wf, outputnode, [
+                ("outputnode.midthickness_fsLR", "midthickness_fsLR")])
+        ])
+        # fmt:on
+
     return wf
```

### Comparing `nibabies-23.0.0/nibabies/workflows/anatomical/brain_extraction.py` & `nibabies-23.1.0rc0/nibabies/workflows/anatomical/brain_extraction.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,16 +56,16 @@
     omp_nthreads : :obj:`int`
         The number of threads for individual processes in this workflow.
     debug : :obj:`bool`
         Produce intermediate registration files
 
     Inputs
     ------
-    in_t2w : :obj:`str`
-        The unprocessed input T2w image.
+    t2w_preproc : :obj:`str`
+        The preprocessed T2w image (Denoising/INU/N4)
 
     Outputs
     -------
     t2w_preproc : :obj:`str`
         The preprocessed T2w image (INU and clipping).
     t2w_brain : :obj:`str`
         The preprocessed, brain-extracted T2w image.
@@ -83,81 +83,61 @@
     # niworkflows
     from niworkflows.interfaces.nibabel import (
         ApplyMask,
         Binarize,
         BinaryDilation,
         IntensityClip,
     )
-    from templateflow.api import get as get_template
 
     from ...utils.misc import cohort_by_months
 
     # handle template specifics
     template_specs = template_specs or {}
     if skull_strip_template == "MNIInfant":
         template_specs["resolution"] = 2 if sloppy else 1
 
     if not template_specs.get("cohort"):
         if age_months is None:
             raise KeyError(f"Age or cohort for {skull_strip_template} must be provided!")
         template_specs["cohort"] = cohort_by_months(skull_strip_template, age_months)
 
-    tpl_target_path = get_template(
-        skull_strip_template,
-        suffix="T1w",  # no T2w template
-        desc=None,
-        **template_specs,
-    )
-    if not tpl_target_path:
-        raise RuntimeError(
-            f"An instance of template <tpl-{skull_strip_template}> with T1w suffix "
-            "could not be found."
-        )
-
-    tpl_brainmask_path = get_template(
-        skull_strip_template, label="brain", suffix="probseg", **template_specs
-    ) or get_template(skull_strip_template, desc="brain", suffix="mask", **template_specs)
-
-    tpl_regmask_path = get_template(
-        skull_strip_template,
-        label="BrainCerebellumExtraction",
-        suffix="mask",
-        **template_specs,
-    )
+    template_files = fetch_templates(skull_strip_template, template_specs)
 
     # main workflow
     workflow = pe.Workflow(name)
 
-    inputnode = pe.Node(niu.IdentityInterface(fields=["in_t2w"]), name="inputnode")
+    inputnode = pe.Node(niu.IdentityInterface(fields=["t2w_preproc"]), name="inputnode")
     outputnode = pe.Node(
         niu.IdentityInterface(fields=["t2w_preproc", "t2w_brain", "out_mask", "out_probmap"]),
         name="outputnode",
     )
 
     # Ensure template comes with a range of intensities ANTs will like
     clip_tmpl = pe.Node(IntensityClip(p_max=99), name="clip_tmpl")
-    clip_tmpl.inputs.in_file = _pop(tpl_target_path)
+    clip_tmpl.inputs.in_file = _pop(template_files['anat'])
 
     # Generate laplacian registration targets
     lap_tmpl = pe.Node(ImageMath(operation="Laplacian", op2="0.4 1"), name="lap_tmpl")
     lap_t2w = pe.Node(ImageMath(operation="Laplacian", op2="0.4 1"), name="lap_t2w")
     norm_lap_tmpl = pe.Node(niu.Function(function=_norm_lap), name="norm_lap_tmpl")
     norm_lap_t2w = pe.Node(niu.Function(function=_norm_lap), name="norm_lap_t2w")
 
     # Merge image nodes
     mrg_tmpl = pe.Node(niu.Merge(2), name="mrg_tmpl", run_without_submitting=True)
     mrg_t2w = pe.Node(niu.Merge(2), name="mrg_t2w", run_without_submitting=True)
     bin_regmask = pe.Node(Binarize(thresh_low=0.20), name="bin_regmask")
-    bin_regmask.inputs.in_file = str(tpl_brainmask_path)
+    bin_regmask.inputs.in_file = str(template_files['mask'])
     refine_mask = pe.Node(BinaryDilation(radius=3, iterations=2), name="refine_mask")
 
     fixed_masks = pe.Node(niu.Merge(4), name="fixed_masks", run_without_submitting=True)
     fixed_masks.inputs.in1 = "NULL"
     fixed_masks.inputs.in2 = "NULL"
-    fixed_masks.inputs.in3 = "NULL" if not tpl_regmask_path else _pop(tpl_regmask_path)
+    fixed_masks.inputs.in3 = (
+        "NULL" if not template_files['regmask'] else _pop(template_files['regmask'])
+    )
 
     # Set up initial spatial normalization
     ants_params = "testing" if sloppy else "precise"
     norm = pe.Node(
         Registration(
             from_file=pkgr_fn("nibabies.data", f"antsBrainExtraction_{ants_params}.json")
         ),
@@ -172,15 +152,15 @@
     map_mask_t2w = pe.Node(
         ApplyTransforms(interpolation="Gaussian", float=True),
         name="map_mask_t2w",
         mem_gb=1,
     )
 
     # map template brainmask to t2w space
-    map_mask_t2w.inputs.input_image = str(tpl_brainmask_path)
+    map_mask_t2w.inputs.input_image = str(template_files['mask'])
 
     thr_t2w_mask = pe.Node(Binarize(thresh_low=0.80), name="thr_t2w_mask")
 
     # Refine INU correction
     final_n4 = pe.Node(
         N4BiasFieldCorrection(
             dimension=3,
@@ -196,19 +176,19 @@
         name="final_n4",
     )
     final_clip = pe.Node(IntensityClip(p_min=5.0, p_max=99.5), name="final_clip")
     apply_mask = pe.Node(ApplyMask(), name="apply_mask")
 
     # fmt:off
     workflow.connect([
-        (inputnode, final_n4, [("in_t2w", "input_image")]),
+        (inputnode, final_n4, [("t2w_preproc", "input_image")]),
         # 1. Massage T2w
-        (inputnode, mrg_t2w, [("in_t2w", "in1")]),
-        (inputnode, lap_t2w, [("in_t2w", "op1")]),
-        (inputnode, map_mask_t2w, [("in_t2w", "reference_image")]),
+        (inputnode, mrg_t2w, [("t2w_preproc", "in1")]),
+        (inputnode, lap_t2w, [("t2w_preproc", "op1")]),
+        (inputnode, map_mask_t2w, [("t2w_preproc", "reference_image")]),
         (bin_regmask, refine_mask, [("out_file", "in_file")]),
         (refine_mask, fixed_masks, [("out_file", "in4")]),
         (lap_t2w, norm_lap_t2w, [("output_image", "in_file")]),
         (norm_lap_t2w, mrg_t2w, [("out", "in2")]),
         # 2. Prepare template
         (clip_tmpl, lap_tmpl, [("out_file", "op1")]),
         (lap_tmpl, norm_lap_tmpl, [("output_image", "in_file")]),
@@ -225,15 +205,15 @@
         ]),
         (map_mask_t2w, thr_t2w_mask, [("output_image", "in_file")]),
         (thr_t2w_mask, apply_mask, [("out_mask", "in_mask")]),
         (final_n4, apply_mask, [("output_image", "in_file")]),
         # 5. Refine T2w INU correction with brain mask
         (map_mask_t2w, final_n4, [("output_image", "weight_image")]),
         (final_n4, final_clip, [("output_image", "in_file")]),
-        # 9. Outputs
+        # 6. Outputs
         (final_clip, outputnode, [("out_file", "t2w_preproc")]),
         (map_mask_t2w, outputnode, [("output_image", "out_probmap")]),
         (thr_t2w_mask, outputnode, [("out_mask", "out_mask")]),
         (apply_mask, outputnode, [("out_file", "t2w_brain")]),
     ])
     # fmt:on
 
@@ -251,79 +231,28 @@
         )
 
         init_aff = pe.Node(
             AI(**ants_kwargs),
             name="init_aff",
             n_procs=omp_nthreads,
         )
-        if tpl_regmask_path:
-            init_aff.inputs.fixed_image_mask = _pop(tpl_regmask_path)
+        if template_files['regmask']:
+            init_aff.inputs.fixed_image_mask = _pop(template_files['regmask'])
 
         # fmt:off
         workflow.connect([
             (clip_tmpl, init_aff, [("out_file", "fixed_image")]),
-            (inputnode, init_aff, [("in_t2w", "moving_image")]),
+            (inputnode, init_aff, [("t2w_preproc", "moving_image")]),
             (init_aff, norm, [("output_transform", "initial_moving_transform")]),
         ])
         # fmt:on
 
     return workflow
 
 
-def init_precomputed_mask_wf(
-    bspline_fitting_distance=200, omp_nthreads=None, name="precomputed_mask_wf"
-):
-    from nipype.interfaces.ants import N4BiasFieldCorrection
-    from niworkflows.interfaces.header import CopyXForm, ValidateImage
-    from niworkflows.interfaces.nibabel import ApplyMask, IntensityClip
-
-    workflow = pe.Workflow(name=name)
-    inputnode = pe.Node(niu.IdentityInterface(fields=["t1w", "t1w_mask"]), name="inputnode")
-    outputnode = pe.Node(
-        niu.IdentityInterface(fields=["t1w_preproc", "t1w_mask", "t1w_brain"]),
-        name="outputnode",
-    )
-
-    validate_mask = pe.Node(ValidateImage(), name="validate_mask")
-    fix_hdr = pe.Node(CopyXForm(), mem_gb=0.1, name="fix_hdr")
-    final_n4 = pe.Node(
-        N4BiasFieldCorrection(
-            dimension=3,
-            bspline_fitting_distance=bspline_fitting_distance,
-            save_bias=True,
-            copy_header=True,
-            n_iterations=[50] * 5,
-            convergence_threshold=1e-7,
-            rescale_intensities=True,
-            shrink_factor=4,
-        ),
-        n_procs=omp_nthreads,
-        name="final_n4",
-    )
-    final_clip = pe.Node(IntensityClip(p_min=5.0, p_max=99.5), name="final_clip")
-    apply_mask = pe.Node(ApplyMask(), name="apply_mask")
-
-    # fmt:off
-    workflow.connect([
-        (inputnode, validate_mask, [("t1w_mask", "in_file")]),
-        (validate_mask, fix_hdr, [("out_file", "in_file")]),
-        (inputnode, fix_hdr, [("t1w", "hdr_file")]),
-        (inputnode, final_n4, [("t1w", "input_image")]),
-        (fix_hdr, final_n4, [("out_file", "weight_image")]),
-        (fix_hdr, apply_mask, [("out_file", "in_mask")]),
-        (final_n4, apply_mask, [("output_image", "in_file")]),
-        (final_n4, final_clip, [("output_image", "in_file")]),
-        (fix_hdr, outputnode, [("out_file", "t1w_mask")]),
-        (final_clip, outputnode, [("out_file", "t1w_preproc")]),
-        (apply_mask, outputnode, [("out_file", "t1w_brain")]),
-    ])
-    # fmt:on
-    return workflow
-
-
 def _pop(in_files):
     if isinstance(in_files, (list, tuple)):
         return in_files[0]
     return in_files
 
 
 def _norm_lap(in_file):
@@ -345,7 +274,24 @@
     out_file = fname_presuffix(
         Path(in_file).name, suffix="_norm", newpath=str(Path.cwd().absolute())
     )
     hdr = img.header.copy()
     hdr.set_data_dtype("float32")
     img.__class__(data.astype("float32"), img.affine, hdr).to_filename(out_file)
     return out_file
+
+
+def fetch_templates(template: str, specs: dict) -> dict:
+    from templateflow.api import get
+
+    template_files = {}
+    # Anatomical reference
+    template_files['anat'] = get(template, suffix="T1w", desc=None, raise_empty=True, **specs)
+    # Anatomical mask, prefer probseg if available
+    template_files['mask'] = get(template, label="brain", suffix="probseg", **specs) or get(
+        template, desc="brain", suffix="mask", **specs
+    )
+    # More dilated mask to facilitate registration
+    template_files['regmask'] = get(
+        template, label="BrainCerebellumExtraction", suffix="mask", **specs
+    )
+    return template_files
```

### Comparing `nibabies-23.0.0/nibabies/workflows/anatomical/norm.py` & `nibabies-23.1.0rc0/nibabies/workflows/anatomical/resampling.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,263 +1,298 @@
-"""Patched version of smriprep's spatial normalization workflow."""
-from collections import defaultdict
+import typing as ty
 
-from nipype.interfaces import ants
-from nipype.interfaces import utility as niu
-from nipype.interfaces.ants.base import Info as ANTsInfo
-from nipype.pipeline import engine as pe
-from niworkflows.engine.workflows import LiterateWorkflow as Workflow
-from niworkflows.interfaces.fixes import FixHeaderApplyTransforms as ApplyTransforms
-from niworkflows.interfaces.norm import SpatialNormalization
-from smriprep.interfaces.templateflow import TemplateDesc, TemplateFlowSelect
-from templateflow.api import get_metadata
-
-
-def init_anat_norm_wf(
-    *,
-    sloppy,
-    omp_nthreads,
-    templates,
-    name="anat_norm_wf",
+import nipype.interfaces.utility as niu
+import nipype.pipeline.engine as pe
+import templateflow.api as tf
+from niworkflows.engine.workflows import LiterateWorkflow
+from smriprep.interfaces.workbench import SurfaceResample
+from smriprep.workflows.surfaces import _collate, init_morph_grayords_wf
+
+from nibabies.config import DEFAULT_MEMORY_MIN_GB
+from nibabies.data import load_resource
+from nibabies.interfaces.utils import CiftiSelect
+
+
+def init_anat_fsLR_resampling_wf(
+    grayord_density: ty.Literal["91k"], mcribs: bool, name="anat_fsLR_resampling_wf"
+) -> LiterateWorkflow:
+    """Resample the surfaces into fsLR space"""
+    workflow = LiterateWorkflow(name=name)
+    fslr_density = "32k" if grayord_density == "91k" else "59k"
+
+    workflow.__desc__ = """\
+The BOLD time-series were resampled onto the left/right-symmetric template
+"fsLR" [@hcppipelines].
+"""
+
+    inputnode = pe.Node(
+        niu.IdentityInterface(
+            fields=[
+                'subject_id',
+                'subjects_dir',
+                'surfaces',
+                'morphometrics',
+                'sphere_reg',
+                'sphere_reg_fsLR',
+            ]
+        ),
+        name='inputnode',
+    )
+
+    itersource = pe.Node(
+        niu.IdentityInterface(fields=['hemi']),
+        name='itersource',
+        iterables=[('hemi', ['L', 'R'])],
+    )
+
+    outputnode = pe.Node(
+        niu.IdentityInterface(
+            fields=[
+                'midthickness_fsLR',
+                'cifti_morph',
+                'cifti_metadata',
+            ]
+        ),
+        name='outputnode',
+    )
+
+    # select white, midthickness and pial surfaces based on hemi
+    select_surfaces = pe.Node(CiftiSelect(), name='select_surfaces')
+
+    if mcribs:
+        atlases = load_resource('atlases')
+        # use dHCP 32k fsLR instead
+        select_surfaces.inputs.template_spheres = [
+            str(atlases / 'dHCP' / 'dHCP.week42.L.sphere.surf.gii'),
+            str(atlases / 'dHCP' / 'dHCP.week42.R.sphere.surf.gii'),
+        ]
+    else:
+        select_surfaces.inputs.template_spheres = [
+            str(sphere)
+            for sphere in tf.get(
+                template='fsLR',
+                density=fslr_density,
+                suffix='sphere',
+                space=None,
+                extension='.surf.gii',
+            )
+        ]
+
+    # Line 393 of FreeSurfer2CaretConvertAndRegisterNonlinear.sh
+    downsampled_midthickness = pe.Node(
+        SurfaceResample(method="BARYCENTRIC"),
+        name="downsampled_midthickness",
+        mem_gb=DEFAULT_MEMORY_MIN_GB,
+    )
+
+    joinnode = pe.JoinNode(
+        niu.IdentityInterface(fields=['midthickness_fsLR']),
+        name='joinnode',
+        joinsource='itersource',
+    )
+
+    # resample surfaces / morphometrics to 32k
+    if mcribs:
+        morph_grayords_wf = init_mcribs_morph_grayords_wf(grayord_density)
+        # fmt:off
+        workflow.connect([
+            (inputnode, morph_grayords_wf, [
+                ("morphometrics", "inputnode.morphometrics"),
+                ("surfaces", "inputnode.surfaces"),
+                ("sphere_reg", "inputnode.sphere_reg")]),
+            (joinnode, morph_grayords_wf, [
+                ("midthickness_fsLR", "inputnode.midthickness_fsLR")]),
+        ])
+        # fmt:on
+    else:
+        morph_grayords_wf = init_morph_grayords_wf(grayord_density)
+
+    # fmt:off
+    workflow.connect([
+        (inputnode, select_surfaces, [
+            ("surfaces", "surfaces"),
+            ("sphere_reg_fsLR", "spherical_registrations")]),
+        (itersource, select_surfaces, [("hemi", "hemi")]),
+        # Downsample midthickness to fsLR density
+        (select_surfaces, downsampled_midthickness, [
+            ("midthickness", "surface_in"),
+            ("sphere_reg", "current_sphere"),
+            ("template_sphere", "new_sphere")]),
+        (downsampled_midthickness, joinnode, [("surface_out", "midthickness_fsLR")]),
+        (joinnode, outputnode, [("midthickness_fsLR", "midthickness_fsLR")]),
+        # resample morphometrics to fsLR 32k
+        (inputnode, morph_grayords_wf, [
+            ("subject_id", "inputnode.subject_id"),
+            ("subjects_dir", "inputnode.subjects_dir")]),
+        (morph_grayords_wf, outputnode, [
+            ("outputnode.cifti_morph", "cifti_morph"),
+            ("outputnode.cifti_metadata", "cifti_metadata")]),
+    ])
+    # fmt:on
+    return workflow
+
+
+def init_mcribs_morph_grayords_wf(
+    grayord_density: ty.Literal['91k'],  # Only 91k supported ATM
+    name: str = "morph_grayords_wf",
 ):
     """
-    Build an individual spatial normalization workflow using ``antsRegistration``.
+    Sample Grayordinates files onto the fsLR atlas.
+
+    If `mcribs` is disabled (default), the fsaverage sphere will be resampled to fsLR.
+    If `mcribs` is enabled, the M-CRIB-S sphere will be resampled to dHCP 42 week.
+
+    Outputs are in CIFTI2 format.
+
     Workflow Graph
-        .. workflow ::
-            :graph2use: orig
+        .. workflow::
+            :graph2use: colored
             :simple_form: yes
-            from smriprep.workflows.norm import init_anat_norm_wf
-            wf = init_anat_norm_wf(
-                debug=False,
-                omp_nthreads=1,
-                templates=['MNI152NLin2009cAsym', 'MNI152NLin6Asym'],
-            )
-    .. important::
-        This workflow defines an iterable input over the input parameter ``templates``,
-        so Nipype will produce one copy of the downstream workflows which connect
-        ``poutputnode.template`` or ``poutputnode.template_spec`` to their inputs
-        (``poutputnode`` stands for *parametric output node*).
-        Nipype refers to this expansion of the graph as *parameterized execution*.
-        If a joint list of values is required (and thus cutting off parameterization),
-        please use the equivalent outputs of ``outputnode`` (which *joins* all the
-        parameterized execution paths).
+
+            from smriprep.workflows.surfaces import init_morph_grayords_wf
+            wf = init_morph_grayords_wf(grayord_density="91k")
+
     Parameters
     ----------
-    debug : :obj:`bool`
-        Apply sloppy arguments to speed up processing. Use with caution,
-        registration processes will be very inaccurate.
-    omp_nthreads : :obj:`int`
-        Maximum number of threads an individual process may use.
-    templates : :obj:`list` of :obj:`str`
-        List of standard space fullnames (e.g., ``MNI152NLin6Asym``
-        or ``MNIPediatricAsym:cohort-4``) which are targets for spatial
-        normalization.
+    grayord_density : :obj:`str`
+        Either `91k` or `170k`, representing the total of vertices or *grayordinates*.
+    name : :obj:`str`
+        Unique name for the subworkflow (default: ``"morph_grayords_wf"``)
+
     Inputs
     ------
-    moving_image
-        The input image that will be normalized to standard space.
-    moving_mask
-        A precise brain mask separating skull/skin/fat from brain
-        structures.
-    moving_segmentation
-        A brain tissue segmentation of the ``moving_image``.
-    moving_tpms
-        tissue probability maps (TPMs) corresponding to the
-        ``moving_segmentation``.
-    lesion_mask
-        (optional) A mask to exclude regions from the cost-function
-        input domain to enable standardization of lesioned brains.
-    orig_t1w
-        The original T1w image from the BIDS structure.
-    template
-        Template name and specification
+    subject_id : :obj:`str`
+        FreeSurfer subject ID
+    subjects_dir : :obj:`str`
+        FreeSurfer SUBJECTS_DIR
+
     Outputs
     -------
-    standardized
-        The T1w after spatial normalization, in template space.
-    anat2std_xfm
-        The T1w-to-template transform.
-    std2anat_xfm
-        The template-to-T1w transform.
-    std_mask
-        The ``moving_mask`` in template space (matches ``standardized`` output).
-    std_dseg
-        The ``moving_segmentation`` in template space (matches ``standardized``
-        output).
-    std_tpms
-        The ``moving_tpms`` in template space (matches ``standardized`` output).
-    template
-        Template name extracted from the input parameter ``template``, for further
-        use in downstream nodes.
-    template_spec
-        Template specifications extracted from the input parameter ``template``, for
-        further use in downstream nodes.
+    cifti_morph : :obj:`list` of :obj:`str`
+        Paths of CIFTI dscalar files
+    cifti_metadata : :obj:`list` of :obj:`str`
+        Paths to JSON files containing metadata corresponding to ``cifti_morph``
+
     """
-    from ...utils.patches import set_reg_resolution, set_tf_resolution
+    from nipype.interfaces.workbench import MetricResample
+    from niworkflows.engine.workflows import LiterateWorkflow as Workflow
+    from smriprep.interfaces.cifti import GenerateDScalar
 
-    ntpls = len(templates)
-    workflow = Workflow(name=name)
+    from nibabies.interfaces.workbench import SurfaceVertexAreas
 
-    if templates:
-        workflow.__desc__ = """\
-Volume-based spatial normalization to {targets} ({targets_id}) was performed through
-nonlinear registration with `antsRegistration` (ANTs {ants_ver}),
-using brain-extracted versions of both T1w reference and the T1w template.
-The following template{tpls} selected for spatial normalization:
-""".format(
-            ants_ver=ANTsInfo.version() or "(version unknown)",
-            targets="%s standard space%s"
-            % (
-                defaultdict("several".format, {1: "one", 2: "two", 3: "three", 4: "four"})[ntpls],
-                "s" * (ntpls != 1),
-            ),
-            targets_id=", ".join(templates),
-            tpls=(" was", "s were")[ntpls != 1],
-        )
-
-        # Append template citations to description
-        for template in templates:
-            template_meta = get_metadata(template.split(":")[0])
-            template_refs = ["@%s" % template.split(":")[0].lower()]
-
-            if template_meta.get("RRID", None):
-                template_refs += ["RRID:%s" % template_meta["RRID"]]
-
-            workflow.__desc__ += """\
-*{template_name}* [{template_refs}; TemplateFlow ID: {template}]""".format(
-                template=template,
-                template_name=template_meta["Name"],
-                template_refs=", ".join(template_refs),
-            )
-            workflow.__desc__ += (", ", ".")[template == templates[-1][0]]
+    workflow = Workflow(name=name)
+    workflow.__desc__ = f"""\
+*Grayordinate* "dscalar" files [@hcppipelines] containing {grayord_density} samples were
+also generated using `M-CRIB-S` as an intermediate standardized
+surface space.
+"""
 
     inputnode = pe.Node(
         niu.IdentityInterface(
             fields=[
-                "lesion_mask",
-                "moving_image",
-                "moving_mask",
-                "moving_segmentation",
-                "moving_tpms",
-                "orig_t1w",
-                "template",
+                "subject_id",
+                "subjects_dir",
+                "surfaces",
+                "morphometrics",
+                "sphere_reg",
+                "midthickness_fsLR",
             ]
         ),
         name="inputnode",
     )
-    inputnode.iterables = [("template", templates)]
-
-    out_fields = [
-        "anat2std_xfm",
-        "standardized",
-        "std2anat_xfm",
-        "std_dseg",
-        "std_mask",
-        "std_tpms",
-        "template",
-        "template_spec",
-    ]
-    poutputnode = pe.Node(niu.IdentityInterface(fields=out_fields), name="poutputnode")
 
-    split_desc = pe.Node(TemplateDesc(), run_without_submitting=True, name="split_desc")
+    outputnode = pe.Node(
+        niu.IdentityInterface(fields=["cifti_morph", "cifti_metadata"]),
+        name="outputnode",
+    )
 
-    # Nibabies hacks
-    set_tf_res = pe.Node(niu.Function(function=set_tf_resolution), name="set_tf_res")
-    set_tf_res.inputs.sloppy = sloppy
-    set_reg_res = pe.Node(niu.Function(function=set_reg_resolution), name="set_reg_res")
-
-    tf_select = pe.Node(
-        TemplateFlowSelect(),
-        name="tf_select",
+    surfmorph_list = pe.Node(
+        niu.Merge(3, ravel_inputs=True),
+        name="surfmorph_list",
         run_without_submitting=True,
     )
 
-    # With the improvements from nipreps/niworkflows#342 this truncation is now necessary
-    trunc_mov = pe.Node(
-        ants.ImageMath(operation="TruncateImageIntensity", op2="0.01 0.999 256"),
-        name="trunc_mov",
+    subject_midthickness = pe.Node(
+        niu.Function(function=_get_surf),
+        name="get_midthickness",
+        run_without_submitting=True,
     )
+    subject_midthickness.inputs.name = "midthickness"
+    subject_midthickness.inputs.mult = 3
 
-    registration = pe.Node(
-        SpatialNormalization(
-            float=True,
-            flavor=["precise", "testing"][sloppy],
-        ),
-        name="registration",
-        n_procs=omp_nthreads,
-        mem_gb=2,
-    )
+    template_midthickness = subject_midthickness.clone("get_new_midthickness")
 
-    # Resample T1w-space inputs
-    tpl_moving = pe.Node(
-        ApplyTransforms(
-            dimension=3,
-            default_value=0,
-            float=True,
-            interpolation="LanczosWindowedSinc",
-        ),
-        name="tpl_moving",
+    # Create Vertex Areas from midthickness surfaces
+    subject_va = pe.MapNode(SurfaceVertexAreas(), iterfield="in_file", name="subject_va")
+    template_va = subject_va.clone("template_va")
+
+    # Setup Workbench command. LR ordering for hemi can be assumed, as it is imposed
+    # by the iterfield of the MapNode in the surface sampling workflow above.
+    resample = pe.MapNode(
+        MetricResample(method="ADAP_BARY_AREA", area_metrics=True),
+        name="resample",
+        iterfield=[
+            "in_file",
+            "out_file",
+            "new_sphere",
+            "new_area",
+            "current_sphere",
+            "current_area",
+        ],
     )
 
-    std_mask = pe.Node(ApplyTransforms(interpolation="MultiLabel"), name="std_mask")
-    std_dseg = pe.Node(ApplyTransforms(interpolation="MultiLabel"), name="std_dseg")
+    atlases = load_resource('atlases')
+    resample.inputs.new_sphere = [  # 32k
+        str(atlases / 'dHCP' / 'dHCP.week42.L.sphere.surf.gii'),
+        str(atlases / 'dHCP' / 'dHCP.week42.R.sphere.surf.gii'),
+    ] * 3
+    resample.inputs.out_file = [
+        f"space-fsLR_hemi-{h}_den-{grayord_density}_{morph}.shape.gii"
+        # Order: curv-L, curv-R, sulc-L, sulc-R, thickness-L, thickness-R
+        for morph in ('curv', 'sulc', 'thickness')
+        for h in "LR"
+    ]
 
-    std_tpms = pe.MapNode(
-        ApplyTransforms(dimension=3, default_value=0, float=True, interpolation="Gaussian"),
-        iterfield=["input_image"],
-        name="std_tpms",
+    gen_cifti = pe.MapNode(
+        GenerateDScalar(
+            grayordinates=grayord_density,
+        ),
+        iterfield=['scalar_name', 'scalar_surfs'],
+        name="gen_cifti",
     )
+    gen_cifti.inputs.scalar_name = ['curv', 'sulc', 'thickness']
 
-    # fmt:off
+    # fmt: off
     workflow.connect([
-        (inputnode, split_desc, [('template', 'template')]),
-        (inputnode, poutputnode, [('template', 'template')]),
-        (inputnode, trunc_mov, [('moving_image', 'op1')]),
-        (inputnode, registration, [
-            ('moving_mask', 'moving_mask'),
-            ('lesion_mask', 'lesion_mask')]),
-        (inputnode, tpl_moving, [('moving_image', 'input_image')]),
-        (inputnode, std_mask, [('moving_mask', 'input_image')]),
-        (split_desc, set_tf_res, [('name', 'template')]),
-        (split_desc, tf_select, [('name', 'template'),
-                                 ('spec', 'template_spec')]),
-        (set_tf_res, tf_select, [('out', 'resolution')]),
-        (split_desc, set_reg_res, [('name', 'template')]),
-        (set_reg_res, registration, [('out', 'template_resolution')]),
-        (split_desc, registration, [('name', 'template'),
-                                    ('spec', 'template_spec')]),
-        (tf_select, tpl_moving, [('t1w_file', 'reference_image')]),
-        (tf_select, std_mask, [('t1w_file', 'reference_image')]),
-        (tf_select, std_dseg, [('t1w_file', 'reference_image')]),
-        (tf_select, std_tpms, [('t1w_file', 'reference_image')]),
-        (trunc_mov, registration, [
-            ('output_image', 'moving_image')]),
-        (registration, tpl_moving, [('composite_transform', 'transforms')]),
-        (registration, std_mask, [('composite_transform', 'transforms')]),
-        (inputnode, std_dseg, [('moving_segmentation', 'input_image')]),
-        (registration, std_dseg, [('composite_transform', 'transforms')]),
-        (inputnode, std_tpms, [('moving_tpms', 'input_image')]),
-        (registration, std_tpms, [('composite_transform', 'transforms')]),
-        (registration, poutputnode, [
-            ('composite_transform', 'anat2std_xfm'),
-            ('inverse_composite_transform', 'std2anat_xfm')]),
-        (tpl_moving, poutputnode, [('output_image', 'standardized')]),
-        (std_mask, poutputnode, [('output_image', 'std_mask')]),
-        (std_dseg, poutputnode, [('output_image', 'std_dseg')]),
-        (std_tpms, poutputnode, [('output_image', 'std_tpms')]),
-        (split_desc, poutputnode, [('spec', 'template_spec')]),
+        (inputnode, resample, [(("sphere_reg", _triple), "current_sphere")]),
+        (inputnode, subject_midthickness, [("surfaces", "surfaces")]),
+        (inputnode, template_midthickness, [("midthickness_fsLR", "surfaces")]),
+        (subject_midthickness, subject_va, [("out", "in_file")]),
+        (template_midthickness, template_va, [("out", "in_file")]),
+        (subject_va, resample, [("out_file", "current_area")]),
+        (template_va, resample, [("out_file", "new_area")]),
+        (inputnode, surfmorph_list, [
+            (('morphometrics', _get_surf, "curv"), "in1"),
+            (('morphometrics', _get_surf, "sulc"), "in2"),
+            (('morphometrics', _get_surf, "thickness"), "in3"),
+        ]),
+        (surfmorph_list, resample, [('out', 'in_file')]),
+        (resample, gen_cifti, [
+            (("out_file", _collate), "scalar_surfs")]),
+        (gen_cifti, outputnode, [("out_file", "cifti_morph"),
+                                 ("out_metadata", "cifti_metadata")]),
     ])
-    # fmt:on
+    # fmt: on
+    return workflow
 
-    # Provide synchronized output
-    outputnode = pe.JoinNode(
-        niu.IdentityInterface(fields=out_fields),
-        name="outputnode",
-        joinsource="inputnode",
-    )
-    # fmt:off
-    workflow.connect([
-        (poutputnode, outputnode, [(f, f) for f in out_fields]),
-    ])
-    # fmt:on
 
-    return workflow
+def _get_surf(surfaces, name, mult=1):
+    from smriprep.workflows.surfaces import _sorted_by_basename
+
+    "Select a specific surface by name, and optionally multiple it."
+    if not surfaces:
+        return surfaces
+    return [surf for surf in _sorted_by_basename(surfaces) if name in surf] * mult
+
+
+def _triple(in_list):
+    return in_list * 3
```

### Comparing `nibabies-23.0.0/nibabies/workflows/anatomical/outputs.py` & `nibabies-23.1.0rc0/nibabies/workflows/anatomical/outputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -119,16 +119,14 @@
         _drop_cohort,
         _empty_report,
         _fmt,
         _pick_cohort,
         _rpt_masks,
     )
 
-    from ...utils.patches import set_tf_resolution
-
     workflow = Workflow(name=name)
 
     inputfields = [
         "source_file",
         "t1w_conform_report",
         "t1w_preproc",
         "t1w_dseg",
@@ -173,18 +171,19 @@
                               ('t1w_mask', 'in_mask'),
                               ('t1w_dseg', 'in_rois')]),
         (seg_rpt, ds_t1w_dseg_mask_report, [('out_report', 'in_file')]),
     ])
     # fmt: on
 
     # Generate reportlets showing spatial normalization
-    tf_select = pe.Node(TemplateFlowSelect(), name="tf_select", run_without_submitting=True)
-
-    set_tf_res = pe.Node(niu.Function(function=set_tf_resolution), name="set_tf_res")
-    set_tf_res.inputs.sloppy = sloppy
+    tf_select = pe.Node(
+        TemplateFlowSelect(resolution=1),
+        name="tf_select",
+        run_without_submitting=True,
+    )
 
     norm_msk = pe.Node(
         niu.Function(
             function=_rpt_masks,
             output_names=["before", "after"],
             input_names=["mask_file", "before", "after", "after_mask"],
         ),
@@ -197,16 +196,14 @@
         DerivativesDataSink(base_directory=output_dir, suffix="T1w", datatype="figures"),
         name="ds_std_t1w_report",
         run_without_submitting=True,
     )
 
     # fmt: off
     workflow.connect([
-        (inputnode, set_tf_res, [(('template', _drop_cohort), 'template')]),
-        (set_tf_res, tf_select, [('out', 'resolution')]),
         (inputnode, tf_select, [(('template', _drop_cohort), 'template'),
                                 (('template', _pick_cohort), 'cohort')]),
         (inputnode, norm_rpt, [('template', 'before_label')]),
         (inputnode, norm_msk, [('std_t1w', 'after'),
                                ('std_mask', 'after_mask')]),
         (tf_select, norm_msk, [('t1w_file', 'before'),
                                ('brain_mask', 'mask_file')]),
@@ -245,14 +242,15 @@
 def init_anat_derivatives_wf(
     *,
     bids_root,
     freesurfer,
     num_t1w,
     output_dir,
     spaces,
+    cifti_output,
     name="anat_derivatives_wf",
     tpm_labels=BIDS_TISSUE_ORDER,
 ):
     """
     Set up a battery of datasinks to store derivatives in the right location.
     Parameters
     ----------
@@ -310,14 +308,20 @@
         FreeSurfer's aseg segmentation, in native T1w space
     t1w_fs_aparc
         FreeSurfer's aparc+aseg segmentation, in native T1w space
     t2w_source_files
         List of input T2w images
     t2w_preproc
         The T2w image in T1w space.
+    cifti_morph
+        Morphometric CIFTI-2 dscalar files
+    cifti_density
+        Grayordinate density
+    cifti_metadata
+        JSON files containing metadata dictionaries
     """
     from niworkflows.interfaces.nibabel import ApplyMask
     from niworkflows.interfaces.utility import KeySelect
     from smriprep.workflows.outputs import (
         _bids_relative,
         _combine_cohort,
         _drop_path,
@@ -343,14 +347,20 @@
                 "fsnative2t1w_xfm",
                 "surfaces",
                 "morphometrics",
                 "t1w_fs_aseg",
                 "t1w_fs_aparc",
                 "t2w_source_files",
                 "t2w_preproc",
+                "anat_ribbon",
+                "cifti_metadata",
+                "cifti_density",
+                "cifti_morph",
+                "sphere_reg",
+                "sphere_reg_fsLR",
             ]
         ),
         name="inputnode",
     )
 
     raw_sources = pe.Node(niu.Function(function=_bids_relative), name="raw_sources")
     raw_sources.inputs.bids_root = bids_root
@@ -358,14 +368,26 @@
     ds_t1w_preproc = pe.Node(
         DerivativesDataSink(base_directory=output_dir, desc="preproc", compress=True),
         name="ds_t1w_preproc",
         run_without_submitting=True,
     )
     ds_t1w_preproc.inputs.SkullStripped = False
 
+    ds_anat_ribbon = pe.Node(
+        DerivativesDataSink(
+            base_directory=output_dir,
+            desc="ribbon",
+            suffix="mask",
+            extension=".nii.gz",
+            compress=True,
+        ),
+        name="ds_anat_ribbon",
+        run_without_submitting=True,
+    )
+
     ds_t1w_mask = pe.Node(
         DerivativesDataSink(base_directory=output_dir, desc="brain", suffix="mask", compress=True),
         name="ds_t1w_mask",
         run_without_submitting=True,
     )
     ds_t1w_mask.inputs.Type = "Brain"
 
@@ -399,14 +421,16 @@
                                      ('t2w_source_files', 'source_file')]),
         (inputnode, ds_t1w_mask, [('t1w_mask', 'in_file'),
                                   ('source_files', 'source_file')]),
         (inputnode, ds_t1w_tpms, [('t1w_tpms', 'in_file'),
                                   ('source_files', 'source_file')]),
         (inputnode, ds_t1w_dseg, [('t1w_dseg', 'in_file'),
                                   ('source_files', 'source_file')]),
+        (inputnode, ds_anat_ribbon, [('anat_ribbon', 'in_file'),
+                                     ('source_files', 'source_file')]),
         (raw_sources, ds_t1w_mask, [('out', 'RawSources')]),
     ])
     # fmt: on
 
     # Transforms
     if spaces.get_spaces(nonstandard=False, dim=(3,)):
         ds_std2t1w_xfm = pe.MapNode(
@@ -651,14 +675,43 @@
     )
     ds_surfs = pe.MapNode(
         DerivativesDataSink(base_directory=output_dir, extension=".surf.gii"),
         iterfield=["in_file", "hemi", "suffix"],
         name="ds_surfs",
         run_without_submitting=True,
     )
+    name_regs = pe.MapNode(
+        Path2BIDS(), iterfield="in_file", name="name_regs", run_without_submitting=True
+    )
+    ds_regs = pe.MapNode(
+        DerivativesDataSink(
+            base_directory=output_dir,
+            desc="reg",
+            suffix="sphere",
+            extension=".surf.gii",
+        ),
+        iterfield=["in_file", "hemi"],
+        name="ds_regs",
+        run_without_submitting=True,
+    )
+    name_reg_fsLR = pe.MapNode(
+        Path2BIDS(), iterfield="in_file", name="name_reg_fsLR", run_without_submitting=True
+    )
+    ds_reg_fsLR = pe.MapNode(
+        DerivativesDataSink(
+            base_directory=output_dir,
+            space="fsLR",
+            desc="reg",
+            suffix="sphere",
+            extension=".surf.gii",
+        ),
+        iterfield=["in_file", "hemi"],
+        name="ds_reg_fsLR",
+        run_without_submitting=True,
+    )
     # Morphometrics
     name_morphs = pe.MapNode(
         Path2BIDS(),
         iterfield="in_file",
         name="name_morphs",
         run_without_submitting=True,
     )
@@ -691,30 +744,65 @@
         (inputnode, ds_fsnative_t1w, [('source_files', 'source_file')]),
         (lta2itk_inv, ds_fsnative_t1w, [('out_xfm', 'in_file')]),
         (inputnode, name_surfs, [('surfaces', 'in_file')]),
         (inputnode, ds_surfs, [('surfaces', 'in_file'),
                                ('source_files', 'source_file')]),
         (name_surfs, ds_surfs, [('hemi', 'hemi'),
                                 ('suffix', 'suffix')]),
+        (inputnode, name_regs, [('sphere_reg', 'in_file')]),
+        (inputnode, ds_regs, [('sphere_reg', 'in_file'),
+                              ('source_files', 'source_file')]),
+        (name_regs, ds_regs, [('hemi', 'hemi')]),
+        (inputnode, name_reg_fsLR, [('sphere_reg_fsLR', 'in_file')]),
+        (inputnode, ds_reg_fsLR, [('sphere_reg_fsLR', 'in_file'),
+                                  ('source_files', 'source_file')]),
+        (name_reg_fsLR, ds_reg_fsLR, [('hemi', 'hemi')]),
         (inputnode, name_morphs, [('morphometrics', 'in_file')]),
         (inputnode, ds_morphs, [('morphometrics', 'in_file'),
                                 ('source_files', 'source_file')]),
         (name_morphs, ds_morphs, [('hemi', 'hemi'),
                                   ('suffix', 'suffix')]),
         (inputnode, ds_t1w_fsaseg, [('t1w_fs_aseg', 'in_file'),
                                     ('source_files', 'source_file')]),
         (inputnode, ds_t1w_fsparc, [('t1w_fs_aparc', 'in_file'),
                                     ('source_files', 'source_file')]),
     ])
     # fmt: on
+    if cifti_output:
+        ds_cifti_morph = pe.MapNode(
+            DerivativesDataSink(
+                base_directory=output_dir,
+                suffix=['curv', 'sulc', 'thickness'],
+                compress=False,
+                space='fsLR',
+            ),
+            name='ds_cifti_morph',
+            run_without_submitting=True,
+            iterfield=["in_file", "meta_dict", "suffix"],
+        )
+        # fmt:off
+        workflow.connect([
+            (inputnode, ds_cifti_morph, [('cifti_morph', 'in_file'),
+                                         ('source_files', 'source_file'),
+                                         ('cifti_density', 'density'),
+                                         (('cifti_metadata', _read_jsons), 'meta_dict')])
+        ])
+        # fmt:on
     return workflow
 
 
 def _set_tpl_res(space, resolution):
     if space in ("UNCInfant", "Fischer344"):
         from nipype.interfaces.base import Undefined
 
         return Undefined
     try:
         return int(resolution)
     except ValueError:
         return 1
+
+
+def _read_jsons(in_file):
+    from json import loads
+    from pathlib import Path
+
+    return [loads(Path(f).read_text()) for f in in_file]
```

### Comparing `nibabies-23.0.0/nibabies/workflows/anatomical/preproc.py` & `nibabies-23.1.0rc0/nibabies/workflows/anatomical/template.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,183 +1,175 @@
 """Prepare anatomical images for processing."""
 from nipype.interfaces import utility as niu
 from nipype.pipeline import engine as pe
+from niworkflows.engine.workflows import LiterateWorkflow
 
 
-def init_anat_average_wf(
+def init_anat_template_wf(
     *,
-    bspline_fitting_distance=200,
-    longitudinal=False,
-    name="anat_average_wf",
-    num_maps=1,
-    omp_nthreads=None,
-    sloppy=False,
-):
+    contrast: str,
+    num_files: int,
+    omp_nthreads: int,
+    longitudinal: bool = False,
+    bspline_fitting_distance: int = 200,
+    sloppy: bool = False,
+    name: str = "anat_template_wf",
+) -> LiterateWorkflow:
     """
-    Create an average from several images of the same modality.
-
-    Each image undergoes a clipping step, removing background noise and
-    high-intensity outliers, which is required by INU correction with the
-    N4 algorithm.
-    Then INU correction is performed for each of the inputs and the range
-    of the image clipped again to fit within uint8.
-    Finally, each image is reoriented to have RAS+ data matrix and, if
-    more than one inputs, aligned and averaged with FreeSurfer's
-    ``mri_robust_template``.
-
+    Generate a canonically-oriented, structural average from all input images.
+    Workflow Graph
+        .. workflow::
+            :graph2use: orig
+            :simple_form: yes
+            from nibabies.workflows.anatomical.template import init_anat_template_wf
+            wf = init_anat_template_wf(
+                longitudinal=False, omp_nthreads=1, num_files=1, contrast="T1w"
+            )
     Parameters
     ----------
-    bspline_fitting_distance : :obj:`float`
-        Distance in mm between B-Spline control points for N4 INU estimation.
+    contrast : :obj:`str`
+        Name of contrast, for reporting purposes, e.g., T1w, T2w, PDw
+    num_files : :obj:`int`
+        Number of images
     longitudinal : :obj:`bool`
-        Whether an unbiased middle point should be calculated.
-    name : :obj:`str`
-        This particular workflow's unique name (Nipype requirement).
-    num_maps : :obj:`int`
-        Then number of input 3D volumes to be averaged.
+        Create unbiased structural average, regardless of number of inputs
+        (may increase runtime)
     omp_nthreads : :obj:`int`
-        The number of threads for individual processes in this workflow.
+        Maximum number of threads an individual process may use
+    bspline_fitting_distance : :obj:`float`
+        Distance in mm between B-Spline control points for N4 INU estimation.
     sloppy : :obj:`bool`
         Run in *sloppy* mode.
-
+    name : :obj:`str`, optional
+        Workflow name (default: anat_template_wf)
     Inputs
     ------
-    in_files : :obj:`list`
-        A list of one or more input files. They can be 3D or 4D.
-
+    anat_files
+        List of structural images
     Outputs
     -------
-    out_file : :obj:`str`
-        The output averaged reference file.
-    valid_list : :obj:`list`
-        A list of accepted/discarded volumes from the input list.
-    realign_xfms : :obj:`list`
-        List of rigid-body transformation matrices that bring every volume
-        into alignment with the average reference.
-    out_report : :obj:`str`
-        Path to a reportlet summarizing what happened in this workflow.
-
+    anat_ref
+        Structural reference averaging input images
+    anat_valid_list
+        List of structural images accepted for combination
+    anat_realign_xfm
+        List of affine transforms to realign input images to final reference
+    out_report
+        Conformation report
     """
     from nipype.interfaces.ants import N4BiasFieldCorrection
     from nipype.interfaces.image import Reorient
-    from niworkflows.engine.workflows import LiterateWorkflow as Workflow
     from niworkflows.interfaces.freesurfer import PatchedLTAConvert as LTAConvert
     from niworkflows.interfaces.freesurfer import StructuralReference
     from niworkflows.interfaces.header import ValidateImage
     from niworkflows.interfaces.images import Conform, TemplateDimensions
-    from niworkflows.interfaces.nibabel import IntensityClip, SplitSeries
+    from niworkflows.interfaces.nibabel import IntensityClip
     from niworkflows.interfaces.nitransforms import ConcatenateXFMs
     from niworkflows.utils.misc import add_suffix
-    from pkg_resources import resource_filename as pkgr
 
-    wf = Workflow(name=name)
+    from nibabies.utils.misc import get_file
 
-    inputnode = pe.Node(niu.IdentityInterface(fields=["in_files"]), name="inputnode")
-    outputnode = pe.Node(
-        niu.IdentityInterface(fields=["out_file", "valid_list", "realign_xfms", "out_report"]),
-        name="outputnode",
-    )
+    wf = LiterateWorkflow(name=name)
+    if num_files > 1:
+        import nipype.interfaces.freesurfer as fs
+
+        fs_ver = fs.Info().looseversion() or "<ver>"
+        wf.__desc__ = f"""\
+An anatomical {contrast}-reference map was computed after registration of
+{num_files} {contrast} images (after INU-correction) using
+`mri_robust_template` [FreeSurfer {fs_ver}, @fs_template].
+"""
 
-    # 1. Validate each of the input images
-    validate = pe.MapNode(
-        ValidateImage(),
-        iterfield="in_file",
-        name="validate",
-        run_without_submitting=True,
+    inputnode = pe.Node(
+        niu.IdentityInterface(fields=["anat_files", "anat_mask", "anat_aseg"]), name="inputnode"
     )
-
-    # 2. Ensure we don't have two timepoints and implicitly squeeze image
-    split = pe.MapNode(SplitSeries(), iterfield="in_file", name="split")
-
-    # 3. INU correction of all independent volumes
-    clip_preinu = pe.MapNode(IntensityClip(p_min=50), iterfield="in_file", name="clip_preinu")
-    correct_inu = pe.MapNode(
-        N4BiasFieldCorrection(
-            dimension=3,
-            save_bias=False,
-            copy_header=True,
-            n_iterations=[50] * (5 - 2 * sloppy),
-            convergence_threshold=1e-7,
-            shrink_factor=4,
-            bspline_fitting_distance=bspline_fitting_distance,
+    outputnode = pe.Node(
+        niu.IdentityInterface(
+            fields=[
+                "anat_ref",
+                "anat_valid_list",
+                "anat_realign_xfm",
+                "out_report",
+            ],
         ),
-        iterfield="input_image",
-        n_procs=omp_nthreads,
-        name="correct_inu",
-    )
-    clip_postinu = pe.MapNode(
-        IntensityClip(p_min=10.0, p_max=99.5), iterfield="in_file", name="clip_postinu"
+        name="outputnode",
     )
 
-    # 4. Reorient T2w image(s) to RAS and resample to common voxel space
-    ref_dimensions = pe.Node(TemplateDimensions(), name="ref_dimensions")
-    conform = pe.MapNode(Conform(), iterfield="in_file", name="conform")
+    # 0. Reorient anatomical image(s) to RAS and resample to common voxel space
+    anat_ref_dimensions = pe.Node(TemplateDimensions(), name="anat_ref_dimensions")
+    anat_conform = pe.MapNode(Conform(), iterfield="in_file", name="anat_conform")
+
     # fmt:off
     wf.connect([
-        (inputnode, ref_dimensions, [("in_files", "t1w_list")]),
-        (inputnode, validate, [("in_files", "in_file")]),
-        (validate, split, [("out_file", "in_file")]),
-        (split, clip_preinu, [(("out_files", _flatten), "in_file")]),
-        (clip_preinu, correct_inu, [("out_file", "input_image")]),
-        (correct_inu, clip_postinu, [("output_image", "in_file")]),
-        (ref_dimensions, conform, [
-            ("t1w_valid_list", "in_file"),
-            ("target_zooms", "target_zooms"),
-            ("target_shape", "target_shape")]),
-        (ref_dimensions, outputnode, [("out_report", "out_report"),
-                                      ("t1w_valid_list", "valid_list")]),
+        (inputnode, anat_ref_dimensions, [('anat_files', 't1w_list')]),
+        (anat_ref_dimensions, anat_conform, [
+            ('t1w_valid_list', 'in_file'),
+            ('target_zooms', 'target_zooms'),
+            ('target_shape', 'target_shape')]),
+        (anat_ref_dimensions, outputnode, [('out_report', 'out_report'),
+                                           ('t1w_valid_list', 'anat_valid_list')]),
     ])
     # fmt:on
 
-    # 5. Reorient template to RAS, if needed (mri_robust_template may set to LIA)
-    ensure_ras = pe.Node(Reorient(), name="ensure_ras")
-
-    if num_maps == 1:
+    if num_files == 1:
         get1st = pe.Node(niu.Select(index=[0]), name="get1st")
-        outputnode.inputs.realign_xfms = [pkgr("smriprep", "data/itkIdentityTransform.txt")]
+        outputnode.inputs.anat_realign_xfm = [
+            get_file("smriprep", "data/itkIdentityTransform.txt")
+        ]
+
         # fmt:off
         wf.connect([
-            (conform, get1st, [("out_file", "inlist")]),
-            (get1st, ensure_ras, [("out", "in_file")]),
-            (ensure_ras, outputnode, [("out_file", "out_file")]),
+            (anat_conform, get1st, [('out_file', 'inlist')]),
+            (get1st, outputnode, [('out', 'anat_ref')]),
         ])
         # fmt:on
         return wf
 
-    from nipype.interfaces import freesurfer as fs
-
-    wf.__desc__ = f"""\
-An anatomical reference-map was computed after registration of
-{num_maps} images (after INU-correction) using
-`mri_robust_template` [FreeSurfer {fs.Info().looseversion() or "<ver>"}, @fs_template].
-"""
-
-    conform_xfm = pe.MapNode(
+    anat_conform_xfm = pe.MapNode(
         LTAConvert(in_lta="identity.nofile", out_lta=True),
         iterfield=["source_file", "target_file"],
-        name="conform_xfm",
+        name="anat_conform_xfm",
     )
-
-    # 6. StructuralReference is fs.RobustTemplate if > 1 volume, copying otherwise
-    merge = pe.Node(
+    # 1. Template (only if several anatomical images)
+    # 1a. Correct for bias field: the bias field is an additive factor
+    #     in log-transformed intensity units. Therefore, it is not a linear
+    #     combination of fields and N4 fails with merged images.
+    # 1b. Align and merge if several anatomical images are provided
+    clip_preinu = pe.MapNode(IntensityClip(p_min=50), iterfield="in_file", name="clip_preinu")
+    n4_correct = pe.MapNode(
+        N4BiasFieldCorrection(
+            dimension=3,
+            save_bias=False,
+            copy_header=True,
+            n_iterations=[50] * (5 - 2 * sloppy),
+            convergence_threshold=1e-7,
+            shrink_factor=4,
+            bspline_fitting_distance=bspline_fitting_distance,
+        ),
+        iterfield="input_image",
+        name="n4_correct",
+        n_procs=1,
+    )
+    # StructuralReference is fs.RobustTemplate if > 1 volume, copying otherwise
+    anat_merge = pe.Node(
         StructuralReference(
             auto_detect_sensitivity=True,
             initial_timepoint=1,  # For deterministic behavior
             intensity_scaling=True,  # 7-DOF (rigid + intensity)
             subsample_threshold=200,
             fixed_timepoint=not longitudinal,
             no_iteration=not longitudinal,
             transform_outputs=True,
         ),
-        mem_gb=2 * num_maps - 1,
-        name="merge",
+        mem_gb=2 * num_files - 1,
+        name="anat_merge",
     )
 
-    # 7. Final intensity equalization/conformation
-    clip_final = pe.Node(IntensityClip(p_min=2.0, p_max=99.9), name="clip_final")
+    # 2. Reorient template to RAS, if needed (mri_robust_template may set to LIA)
+    anat_reorient = pe.Node(Reorient(), name="anat_reorient")
 
     merge_xfm = pe.MapNode(
         niu.Merge(2),
         name="merge_xfm",
         iterfield=["in1", "in2"],
         run_without_submitting=True,
     )
@@ -189,32 +181,26 @@
     )
 
     def _set_threads(in_list, maximum):
         return min(len(in_list), maximum)
 
     # fmt:off
     wf.connect([
-        (ref_dimensions, conform_xfm, [("t1w_valid_list", "source_file")]),
-        (conform, conform_xfm, [("out_file", "target_file")]),
-        (conform, merge, [
-            ("out_file", "in_files"),
-            (("out_file", _set_threads, omp_nthreads), "num_threads"),
-            (("out_file", add_suffix, "_template"), "out_file")]),
-        (merge, ensure_ras, [("out_file", "in_file")]),
+        (anat_ref_dimensions, anat_conform_xfm, [('t1w_valid_list', 'source_file')]),
+        (anat_conform, anat_conform_xfm, [('out_file', 'target_file')]),
+        (anat_conform, clip_preinu, [('out_file', 'in_file')]),
+        (anat_conform, anat_merge, [
+            (('out_file', _set_threads, omp_nthreads), 'num_threads'),
+            (('out_file', add_suffix, '_template'), 'out_file')]),
+        (clip_preinu, n4_correct, [('out_file', 'input_image')]),
+        (n4_correct, anat_merge, [('output_image', 'in_files')]),
+        (anat_merge, anat_reorient, [('out_file', 'in_file')]),
         # Combine orientation and template transforms
-        (conform_xfm, merge_xfm, [("out_lta", "in1")]),
-        (merge, merge_xfm, [("transform_outputs", "in2")]),
-        (merge_xfm, concat_xfms, [("out", "in_xfms")]),
+        (anat_conform_xfm, merge_xfm, [('out_lta', 'in1')]),
+        (anat_merge, merge_xfm, [('transform_outputs', 'in2')]),
+        (merge_xfm, concat_xfms, [('out', 'in_xfms')]),
         # Output
-        (ensure_ras, clip_final, [("out_file", "in_file")]),
-        (clip_final, outputnode, [("out_file", "out_file")]),
-        (concat_xfms, outputnode, [("out_xfm", "realign_xfms")]),
+        (anat_reorient, outputnode, [('out_file', 'anat_ref')]),
+        (concat_xfms, outputnode, [('out_xfm', 'anat_realign_xfm')]),
     ])
     # fmt:on
-
     return wf
-
-
-def _flatten(inlist):
-    from bids.utils import listify
-
-    return [el for items in listify(inlist) for el in listify(items)]
```

### Comparing `nibabies-23.0.0/nibabies/workflows/anatomical/registration.py` & `nibabies-23.1.0rc0/nibabies/workflows/anatomical/registration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # emacs: -*- mode: python; py-indent-offset: 4; indent-tabs-mode: nil -*-
 # vi: set ft=python sts=4 ts=4 sw=4 et:
 """Within-baby registration of a T1w into a T2w image."""
+from typing import Optional
+
 from nipype.interfaces import utility as niu
 from nipype.pipeline import engine as pe
 from pkg_resources import resource_filename as pkgr_fn
 
 
 def init_coregistration_wf(
     *,
-    bspline_fitting_distance=200,
-    mem_gb=3.0,
-    name="coregistration_wf",
-    omp_nthreads=None,
-    sloppy=False,
-    debug=False,
+    bspline_fitting_distance: int = 200,
+    mem_gb: float = 3.0,
+    omp_nthreads: Optional[int] = None,
+    sloppy: bool = False,
+    debug: bool = False,
+    precomputed_mask: bool = False,
+    name: str = "coregistration_wf",
 ):
     """
     Set-up a T2w-to-T1w within-baby co-registration framework.
 
     See the ANTs' registration config file (under ``nibabies/data``) for further
     details.
     The main surprise in it is that, for some participants, accurate registration
@@ -45,50 +48,58 @@
         This particular workflow's unique name (Nipype requirement).
     omp_nthreads : :obj:`int`
         The number of threads for individual processes in this workflow.
     sloppy : :obj:`bool`
         Run in *sloppy* mode.
     debug : :obj:`bool`
         Produce intermediate registration files
+    precomputed_mask : :obj:`bool`
+        A precomputed mask for the T1w is available. In this case, generate a
+        quick mask to assist in coregistration, but use the precomputed mask
+        as the final output.
 
 
     Inputs
     ------
     in_t1w : :obj:`str`
-        The unprocessed input T1w image.
-    in_t2w_preproc : :obj:`str`
-        The preprocessed input T2w image, from the brain extraction workflow.
+        The preprocessed input T1w image (Denoising/INU/Clipping)
+    in_t2w : :obj:`str`
+        The preprocessed input T2w image (Denoising/INU/Clipping)
     in_mask : :obj:`str`
-        The brainmask, as obtained in T2w space.
+        The brainmask.
+        If `precomputed_mask` is False, will be in T2w space.
+        If `precomputed_mask` is True, will be in T1w space.
     in_probmap : :obj:`str`
         The probabilistic brainmask, as obtained in T2w space.
 
     Outputs
     -------
-    t1w_preproc : :obj:`str`
-        The preprocessed T1w image (INU and clipping).
-    t2w_preproc : :obj:`str`
+    t1w_coreg : :obj:`str`
+        The preprocessed T1w image (INU and clipping), in its native space.
+    t2w_coreg : :obj:`str`
         The preprocessed T2w image (INU and clipping), aligned into the T1w's space.
     t1w_brain : :obj:`str`
         The preprocessed, brain-extracted T1w image.
     t1w_mask : :obj:`str`
-        The binary brainmask projected from the T2w.
+        The binary brainmask in T1w space.
     t1w2t2w_xfm : :obj:`str`
         The T1w-to-T2w mapping.
 
     """
     from nipype.interfaces.ants import N4BiasFieldCorrection
     from niworkflows.interfaces.fixes import FixHeaderApplyTransforms as ApplyTransforms
     from niworkflows.interfaces.fixes import FixHeaderRegistration as Registration
     from niworkflows.interfaces.nibabel import ApplyMask, Binarize, BinaryDilation
 
+    from nibabies.utils.misc import get_file
+
     workflow = pe.Workflow(name)
 
     inputnode = pe.Node(
-        niu.IdentityInterface(fields=["in_t1w", "in_t2w_preproc", "in_mask", "in_probmap"]),
+        niu.IdentityInterface(fields=["in_t1w", "in_t2w", "in_mask", "in_probmap"]),
         name="inputnode",
     )
     outputnode = pe.Node(
         niu.IdentityInterface(
             fields=[
                 "t1w_preproc",
                 "t1w_brain",
@@ -96,81 +107,104 @@
                 "t1w2t2w_xfm",
                 "t2w_preproc",
             ]
         ),
         name="outputnode",
     )
 
-    fixed_masks_arg = pe.Node(niu.Merge(3), name="fixed_masks_arg", run_without_submitting=True)
-
     # Dilate t2w mask for easier t1->t2 registration
+    fixed_masks_arg = pe.Node(niu.Merge(3), name="fixed_masks_arg", run_without_submitting=True)
     reg_mask = pe.Node(BinaryDilation(radius=8, iterations=3), name="reg_mask")
     refine_mask = pe.Node(BinaryDilation(radius=8, iterations=1), name="refine_mask")
 
-    # Set up T2w -> T1w within-subject registration
+    # Set up T1w -> T2w within-subject registration
     coreg = pe.Node(
-        Registration(from_file=pkgr_fn("nibabies.data", "within_subject_t1t2.json")),
+        Registration(from_file=get_file("nibabies", "data/within_subject_t1t2.json")),
         name="coreg",
         n_procs=omp_nthreads,
         mem_gb=mem_gb,
     )
     coreg.inputs.float = sloppy
     if debug:
         coreg.inputs.args = "--write-interval-volumes 5"
         coreg.inputs.output_inverse_warped_image = sloppy
         coreg.inputs.output_warped_image = sloppy
 
-    map_mask = pe.Node(ApplyTransforms(interpolation="Gaussian"), name="map_mask", mem_gb=1)
-    map_t2w = pe.Node(ApplyTransforms(interpolation="BSpline"), name="map_t2w", mem_gb=1)
-    thr_mask = pe.Node(Binarize(thresh_low=0.80), name="thr_mask")
-
     final_n4 = pe.Node(
         N4BiasFieldCorrection(
             dimension=3,
             bspline_fitting_distance=bspline_fitting_distance,
             save_bias=True,
             copy_header=True,
             n_iterations=[50] * 5,
             convergence_threshold=1e-7,
             rescale_intensities=True,
             shrink_factor=4,
         ),
         n_procs=omp_nthreads,
         name="final_n4",
     )
+    # Move the T2w into T1w space, and apply the mask to the T1w
+    map_t2w = pe.Node(ApplyTransforms(interpolation="BSpline"), name="map_t2w", mem_gb=1)
     apply_mask = pe.Node(ApplyMask(), name="apply_mask")
 
     # fmt: off
     workflow.connect([
-        (inputnode, map_mask, [("in_t1w", "reference_image")]),
         (inputnode, final_n4, [("in_t1w", "input_image")]),
         (inputnode, coreg, [("in_t1w", "moving_image"),
-                            ("in_t2w_preproc", "fixed_image")]),
-        (inputnode, map_mask, [("in_probmap", "input_image")]),
-        (inputnode, reg_mask, [("in_mask", "in_file")]),
-        (inputnode, refine_mask, [("in_mask", "in_file")]),
-        (reg_mask, fixed_masks_arg, [("out_file", "in1")]),
-        (reg_mask, fixed_masks_arg, [("out_file", "in2")]),
+                            ("in_t2w", "fixed_image")]),
+        (reg_mask, fixed_masks_arg, [
+            ("out_file", "in1"),
+            ("out_file", "in2")]),
         (refine_mask, fixed_masks_arg, [("out_file", "in3")]),
-        (inputnode, map_t2w, [("in_t1w", "reference_image")]),
-        (inputnode, map_t2w, [("in_t2w_preproc", "input_image")]),
+        (inputnode, map_t2w, [
+            ("in_t1w", "reference_image"),
+            ("in_t2w", "input_image")]),
         (fixed_masks_arg, coreg, [("out", "fixed_image_masks")]),
-        (coreg, map_mask, [
-            ("reverse_transforms", "transforms"),
-            ("reverse_invert_flags", "invert_transform_flags"),
-        ]),
         (coreg, map_t2w, [
             ("reverse_transforms", "transforms"),
             ("reverse_invert_flags", "invert_transform_flags"),
         ]),
-        (map_mask, thr_mask, [("output_image", "in_file")]),
-        (map_mask, final_n4, [("output_image", "weight_image")]),
         (final_n4, apply_mask, [("output_image", "in_file")]),
-        (thr_mask, apply_mask, [("out_mask", "in_mask")]),
         (final_n4, outputnode, [("output_image", "t1w_preproc")]),
         (map_t2w, outputnode, [("output_image", "t2w_preproc")]),
-        (thr_mask, outputnode, [("out_mask", "t1w_mask")]),
         (apply_mask, outputnode, [("out_file", "t1w_brain")]),
         (coreg, outputnode, [("forward_transforms", "t1w2t2w_xfm")]),
     ])
     # fmt: on
+
+    if precomputed_mask:
+        # The input mask is already in T1w space.
+        # Generate a quick, rough mask of the T2w to be used to facilitate co-registration.
+        from sdcflows.interfaces.brainmask import BrainExtraction
+
+        masker = pe.Node(BrainExtraction(), name="t2w_masker")
+        # fmt:off
+        workflow.connect([
+            (inputnode, masker, [("in_t2w", "in_file")]),
+            (masker, reg_mask, [("out_mask", "in_file")]),
+            (masker, refine_mask, [("out_mask", "in_file")]),
+            (inputnode, apply_mask, [("in_mask", "in_mask")]),
+            (inputnode, outputnode, [("in_mask", "t1w_mask")]),
+        ])
+        # fmt:on
+    else:
+        # The T2w mask from the brain extraction workflow will be mapped to T1w space
+        map_mask = pe.Node(ApplyTransforms(interpolation="Gaussian"), name="map_mask", mem_gb=1)
+        thr_mask = pe.Node(Binarize(thresh_low=0.80), name="thr_mask")
+        # fmt:off
+        workflow.connect([
+            (inputnode, map_mask, [
+                ("in_t1w", "reference_image"),
+                ("in_probmap", "input_image")]),
+            (inputnode, reg_mask, [("in_mask", "in_file")]),
+            (inputnode, refine_mask, [("in_mask", "in_file")]),
+            (coreg, map_mask, [
+                ("reverse_transforms", "transforms"),
+                ("reverse_invert_flags", "invert_transform_flags")]),
+            (map_mask, thr_mask, [("output_image", "in_file")]),
+            (map_mask, final_n4, [("output_image", "weight_image")]),
+            (thr_mask, outputnode, [("out_mask", "t1w_mask")]),
+            (thr_mask, apply_mask, [("out_mask", "in_mask")]),
+        ])
+        # fmt:on
     return workflow
```

### Comparing `nibabies-23.0.0/nibabies/workflows/anatomical/segmentation.py` & `nibabies-23.1.0rc0/nibabies/workflows/anatomical/segmentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from nipype.interfaces import fsl
 from nipype.interfaces import utility as niu
 from nipype.interfaces.ants.segmentation import JointFusion
 from nipype.pipeline import engine as pe
 from niworkflows.interfaces.fixes import FixHeaderApplyTransforms as ApplyTransforms
 from niworkflows.interfaces.fixes import FixHeaderRegistration as Registration
+from niworkflows.interfaces.nibabel import MapLabels
 from pkg_resources import resource_filename as pkgr_fn
 from smriprep.utils.misc import apply_lut as _apply_bids_lut
 from smriprep.workflows.anatomical import (
     _aseg_to_three,
     _probseg_fast2bids,
     _split_segments,
 )
@@ -50,14 +51,15 @@
         niu.IdentityInterface(fields=["anat_brain", "anat_aseg"]),
         name="inputnode",
     )
     outputnode = pe.Node(
         niu.IdentityInterface(fields=["anat_aseg", "anat_dseg", "anat_tpms"]),
         name="outputnode",
     )
+    buffernode = pe.Node(niu.IdentityInterface(fields=["final_aseg"]), name='buffernode')
 
     wf.__desc__ = """Brain tissue segmentation of cerebrospinal fluid (CSF),
 white-matter (WM) and gray-matter (GM) was performed on """
 
     # Coerce segmentation labels to BIDS
     lut_anat_dseg = pe.Node(niu.Function(function=_apply_bids_lut), name="lut_anat_dseg")
 
@@ -155,39 +157,38 @@
             (inputnode, apply_atlas, [('anat_brain', 'reference_image')]),
             (norm, apply_seg, [('forward_transforms', 'transforms')]),
             (inputnode, apply_seg, [('anat_brain', 'reference_image')]),
             (inputnode, jointfusion, [(('anat_brain', listify), 'target_image')]),
             (apply_atlas, jointfusion, [('output_image', 'atlas_image')]),
             (apply_seg, jointfusion, [('output_image', 'atlas_segmentation_image')]),
             (jointfusion, jf_label, [('out_label_fusion', 'in_file')]),
+            (jf_label, buffernode, [('out_file', 'final_aseg')]),
         ])
         # fmt:on
 
     elif precomp_aseg:
         wf.__desc__ += "a pre-computed segmentation."
-        from niworkflows.interfaces.header import ValidateImage
 
-        inputnode.inputs.anat_aseg = precomp_aseg
-        validate_aseg = pe.Node(ValidateImage(), name="validate_aseg")
-        wf.connect(inputnode, "anat_aseg", validate_aseg, "in_file")
+        wf.connect(inputnode, "anat_aseg", buffernode, "final_aseg")
 
     # Otherwise, the final aseg will be split into three tissue classes
     # regardless if it was precomputed or generated via JLF
     lut_anat_dseg.inputs.lut = _aseg_to_three()
     split_seg = pe.Node(niu.Function(function=_split_segments), name="split_seg")
-    out_aseg = validate_aseg if precomp_aseg else jf_label
+
     # fmt: off
     wf.connect([
-        (out_aseg, outputnode, [('out_file', 'anat_aseg')]),
-        (out_aseg, lut_anat_dseg, [('out_file', 'in_dseg')]),
+        (buffernode, outputnode, [('final_aseg', 'anat_aseg')]),
+        (buffernode, lut_anat_dseg, [('final_aseg', 'in_dseg')]),
         (lut_anat_dseg, outputnode, [('out', 'anat_dseg')]),
         (lut_anat_dseg, split_seg, [('out', 'in_file')]),
         (split_seg, outputnode, [('out', 'anat_tpms')]),
     ])
     # fmt: on
+
     return wf
 
 
 def _parse_segmentation_atlases(anat_modality, template_dir):
     """
     Parse segmentation templates directory for anatomical and segmentation files.
```

### Comparing `nibabies-23.0.0/nibabies/workflows/bold/alignment.py` & `nibabies-23.1.0rc0/nibabies/workflows/bold/alignment.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/workflows/bold/base.py` & `nibabies-23.1.0rc0/nibabies/workflows/bold/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     init_bold_std_trans_wf,
     init_bold_surf_wf,
 )
 from .stc import init_bold_stc_wf
 from .t2s import init_bold_t2s_wf, init_t2s_reporting_wf
 
 
-def init_func_preproc_wf(bold_file, has_fieldmap=False, existing_derivatives=None):
+def init_func_preproc_wf(bold_file, spaces, has_fieldmap=False, existing_derivatives=None):
     """
     This workflow controls the functional preprocessing stages of *NiBabies*.
 
     Workflow Graph
         .. workflow::
             :graph2use: orig
             :simple_form: yes
@@ -187,16 +187,17 @@
 
     mem_gb = {"filesize": 1, "resampled": 1, "largemem": 1}
     bold_tlen = 10
 
     # Have some options handy
     omp_nthreads = config.nipype.omp_nthreads
     freesurfer = config.workflow.run_reconall
-    spaces = config.workflow.spaces
     nibabies_dir = str(config.execution.nibabies_dir)
+    freesurfer_spaces = spaces.get_fs_spaces()
+    project_goodvoxels = config.workflow.project_goodvoxels and config.workflow.cifti_output
 
     # Extract BIDS entities and metadata from BOLD file(s)
     entities = extract_entities(bold_file)
     layout = config.execution.layout
 
     # Extract metadata
     all_metadata = [layout.get_metadata(fname) for fname in listify(bold_file)]
@@ -297,16 +298,15 @@
 All resamplings can be performed with *a single interpolation
 step* by composing all the pertinent transformations (i.e. head-motion
 transform matrices, susceptibility distortion correction when available,
 and co-registrations to anatomical and output spaces).
 Gridded (volumetric) resamplings were performed using `antsApplyTransforms` (ANTs),
 configured with Lanczos interpolation to minimize the smoothing
 effects of other kernels [@lanczos].
-Non-gridded (surface) resamplings were performed using `mri_vol2surf`
-(FreeSurfer).
+Non-gridded (surface) resamplings were performed using `mri_vol2surf` (FreeSurfer)
 """
 
     inputnode = pe.Node(
         niu.IdentityInterface(
             fields=[
                 "bold_file",
                 # from smriprep
@@ -316,26 +316,35 @@
                 "anat_dseg",
                 "anat_tpms",
                 "anat_aseg",
                 "anat_aparc",
                 "anat2std_xfm",
                 "std2anat_xfm",
                 "template",
+                "anat_ribbon",
+                # from bold reference workflow
+                "bold_ref",
+                "bold_ref_xfm",
+                "n_dummy_scans",
                 # from sdcflows (optional)
                 "fmap",
                 "fmap_ref",
                 "fmap_coeff",
                 "fmap_mask",
                 "fmap_id",
                 "sdc_method",
                 # if reconstructing with FreeSurfer (optional)
                 "t1w2fsnative_xfm",
                 "fsnative2t1w_xfm",
                 "subject_id",
                 "subjects_dir",
+                "surfaces",
+                "morphometrics",
+                "sphere_reg_fsLR",
+                "midthickness_fsLR",
             ]
         ),
         name="inputnode",
     )
     inputnode.inputs.bold_file = bold_file
 
     outputnode = pe.Node(
@@ -411,14 +420,15 @@
     )
     summary.inputs.dummy_scans = config.workflow.dummy_scans
 
     func_derivatives_wf = init_func_derivatives_wf(
         bids_root=layout.root,
         cifti_output=config.workflow.cifti_output,
         freesurfer=freesurfer,
+        project_goodvoxels=project_goodvoxels,
         all_metadata=all_metadata,
         multiecho=multiecho,
         output_dir=nibabies_dir,
         spaces=spaces,
         use_aroma=config.workflow.use_aroma,
     )
     func_derivatives_wf.inputs.inputnode.all_source_files = bold_file
@@ -912,14 +922,15 @@
     freesurfer_spaces = spaces.get_fs_spaces()
     if freesurfer and freesurfer_spaces:
         config.loggers.workflow.debug("Creating BOLD surface-sampling workflow.")
         bold_surf_wf = init_bold_surf_wf(
             mem_gb=mem_gb["resampled"],
             surface_spaces=freesurfer_spaces,
             medial_surface_nan=config.workflow.medial_surface_nan,
+            surface_recon_method=config.workflow.surface_recon_method,
             name="bold_surf_wf",
         )
         # fmt:off
         workflow.connect([
             (inputnode, bold_surf_wf, [
                 ('subjects_dir', 'inputnode.subjects_dir'),
                 ('subject_id', 'inputnode.subject_id'),
@@ -927,63 +938,90 @@
             (bold_t1_trans_wf, bold_surf_wf, [('outputnode.bold_t1', 'inputnode.source_file')]),
             (bold_surf_wf, outputnode, [('outputnode.surfaces', 'surfaces')]),
             (bold_surf_wf, func_derivatives_wf, [
                 ('outputnode.target', 'inputnode.surf_refs')]),
         ])
         # fmt:on
 
-        # CIFTI output
-        if config.workflow.cifti_output:
-            from .alignment import (
-                init_subcortical_mni_alignment_wf,
-                init_subcortical_rois_wf,
-            )
-            from .resampling import init_bold_grayords_wf
+    # CIFTI output
+    if config.workflow.cifti_output:
+        from .alignment import (
+            init_subcortical_mni_alignment_wf,
+            init_subcortical_rois_wf,
+        )
+        from .resampling import init_bold_fsLR_resampling_wf, init_bold_grayords_wf
 
-            key = get_MNIInfant_key(spaces)
+        # Anatomical -> fsLR surfaces
 
-            # BOLD/ROIs should be in MNIInfant space
-            cifti_select_std = pe.Node(
-                KeySelect(fields=["bold_std", "bold_aseg_std"], key=key),
-                name="cifti_select_std",
-                run_without_submitting=True,
-            )
+        bold_fsLR_resampling_wf = init_bold_fsLR_resampling_wf(
+            estimate_goodvoxels=project_goodvoxels,
+            grayord_density=config.workflow.cifti_output,
+            omp_nthreads=omp_nthreads,
+            mcribs=config.workflow.surface_recon_method == "mcribs",
+            mem_gb=mem_gb["resampled"],
+        )
 
-            subcortical_rois_wf = init_subcortical_rois_wf()
-            subcortical_mni_alignment_wf = init_subcortical_mni_alignment_wf()
-            bold_grayords_wf = init_bold_grayords_wf(
-                grayord_density=config.workflow.cifti_output,
-                mem_gb=mem_gb["resampled"],
-                repetition_time=metadata["RepetitionTime"],
-            )
+        subcortical_rois_wf = init_subcortical_rois_wf()
+        subcortical_mni_alignment_wf = init_subcortical_mni_alignment_wf()
+        bold_grayords_wf = init_bold_grayords_wf(
+            grayord_density=config.workflow.cifti_output,
+            mem_gb=mem_gb["resampled"],
+            repetition_time=metadata["RepetitionTime"],
+        )
 
-            # fmt:off
-            workflow.connect([
-                (bold_std_trans_wf, cifti_select_std, [
-                    ("outputnode.bold_std", "bold_std"),
-                    ("outputnode.bold_aseg_std", "bold_aseg_std"),
-                    ("outputnode.spatial_reference", "keys")]),
-                (cifti_select_std, subcortical_rois_wf, [
-                    ("bold_aseg_std", "inputnode.MNIInfant_aseg")]),
-                (cifti_select_std, subcortical_mni_alignment_wf, [
-                    ("bold_std", "inputnode.MNIInfant_bold")]),
-                (subcortical_rois_wf, subcortical_mni_alignment_wf, [
-                    ("outputnode.MNIInfant_rois", "inputnode.MNIInfant_rois"),
-                    ("outputnode.MNI152_rois", "inputnode.MNI152_rois")]),
-                (subcortical_mni_alignment_wf, bold_grayords_wf, [
-                    ("outputnode.subcortical_volume", "inputnode.subcortical_volume"),
-                    ("outputnode.subcortical_labels", "inputnode.subcortical_labels")]),
-                (bold_surf_wf, bold_grayords_wf, [
-                    ('outputnode.surfaces', 'inputnode.surf_files'),
-                    ('outputnode.target', 'inputnode.surf_refs')]),
-                (bold_grayords_wf, outputnode, [
-                    ('outputnode.cifti_bold', 'bold_cifti'),
-                    ('outputnode.cifti_metadata', 'cifti_metadata')]),
-            ])
-            # fmt:on
+        key = get_MNIInfant_key(spaces)
+        # BOLD/ROIs should be in MNIInfant space
+        cifti_select_std = pe.Node(
+            KeySelect(fields=["bold_std", "bold_aseg_std"], key=key),
+            name="cifti_select_std",
+            run_without_submitting=True,
+        )
+
+        # fmt:off
+        workflow.connect([
+            # select the MNIInfant standard
+            # CIFTI subcortical volumetric re
+            (bold_std_trans_wf, cifti_select_std, [
+                ("outputnode.bold_std", "bold_std"),
+                ("outputnode.bold_aseg_std", "bold_aseg_std"),
+                ("outputnode.spatial_reference", "keys")]),
+            (cifti_select_std, subcortical_rois_wf, [
+                ("bold_aseg_std", "inputnode.MNIInfant_aseg")]),
+            (cifti_select_std, subcortical_mni_alignment_wf, [
+                ("bold_std", "inputnode.MNIInfant_bold")]),
+            (subcortical_rois_wf, subcortical_mni_alignment_wf, [
+                ("outputnode.MNIInfant_rois", "inputnode.MNIInfant_rois"),
+                ("outputnode.MNI152_rois", "inputnode.MNI152_rois")]),
+
+            # CIFTI surface sampling
+            (inputnode, bold_fsLR_resampling_wf, [
+                ("surfaces", "inputnode.surfaces"),
+                ("morphometrics", "inputnode.morphometrics"),
+                ("sphere_reg_fsLR", "inputnode.sphere_reg_fsLR"),
+                ("midthickness_fsLR", "inputnode.midthickness_fsLR"),
+                ("anat_ribbon", "inputnode.anat_ribbon")]),
+            (bold_t1_trans_wf, bold_fsLR_resampling_wf, [
+                ("outputnode.bold_t1", "inputnode.bold_file")]),
+            (bold_fsLR_resampling_wf, func_derivatives_wf, [
+                ("outputnode.goodvoxels_mask", "inputnode.goodvoxels_mask"),
+            ]),
+
+            # combine surface + volume into dtseries
+            (subcortical_mni_alignment_wf, bold_grayords_wf, [
+                ("outputnode.subcortical_volume", "inputnode.subcortical_volume"),
+                ("outputnode.subcortical_labels", "inputnode.subcortical_labels")]),
+            (bold_fsLR_resampling_wf, bold_grayords_wf, [
+                ("outputnode.bold_fsLR", "inputnode.bold_fsLR"),
+            ]),
+            (bold_grayords_wf, outputnode, [
+                ("outputnode.cifti_bold", "bold_cifti"),
+                ("outputnode.cifti_metadata", "cifti_metadata"),
+            ]),
+        ])
+        # fmt:on
 
     if spaces.get_spaces(nonstandard=False, dim=(3,)):
         if not config.workflow.cifti_output:
             config.loggers.workflow.critical("The carpetplot requires CIFTI outputs")
         else:
             carpetplot_wf = init_carpetplot_wf(
                 mem_gb=mem_gb["resampled"],
@@ -1133,14 +1171,17 @@
             ("fmap_coeff", "inputnode.fmap_coeff"),
             ("fmap_mask", "inputnode.fmap_mask")]),
         (output_select, summary, [("sdc_method", "distortion_correction")]),
         (initial_boldref_wf, coeff2epi_wf, [
             ("outputnode.boldref_file", "inputnode.target_ref")]),
         (initial_boldref_wf, coeff2epi_wf, [
             ("outputnode.boldref_mask", "inputnode.target_mask")]),  # skull-stripped brain
+        (initial_boldref_wf, unwarp_wf, [
+            ("outputnode.boldref_file", "inputnode.distorted_ref"),
+        ]),
         (coeff2epi_wf, unwarp_wf, [
             ("outputnode.fmap_coeff", "inputnode.fmap_coeff")]),
         (initial_boldref_wf, sdc_report, [("outputnode.boldref_file", "before")]),
         (bold_hmc_wf, unwarp_wf, [
             ("outputnode.xforms", "inputnode.hmc_xforms")]),
         (bold_split, unwarp_wf, [
             ("out_files", "inputnode.distorted")]),
@@ -1158,19 +1199,19 @@
             (unwarp_wf, bold_final, [("outputnode.corrected", "bold")]),
             # remaining workflow connections
             (unwarp_wf, final_boldref_wf, [
                 ("outputnode.corrected", "inputnode.in_files"),
             ]),
             (unwarp_wf, bold_t1_trans_wf, [
                 # TEMPORARY: For the moment we can't use frame-wise fieldmaps
-                (("outputnode.fieldwarp", pop_file), "inputnode.fieldwarp"),
+                (("outputnode.fieldwarp_ref", pop_file), "inputnode.fieldwarp"),
             ]),
             (unwarp_wf, bold_std_trans_wf, [
                 # TEMPORARY: For the moment we can't use frame-wise fieldmaps
-                (("outputnode.fieldwarp", pop_file), "inputnode.fieldwarp"),
+                (("outputnode.fieldwarp_ref", pop_file), "inputnode.fieldwarp"),
             ]),
         ])
         # fmt:on
         return workflow
 
     # Finalize connections if ME-EPI
     join_sdc_echos = pe.JoinNode(
```

### Comparing `nibabies-23.0.0/nibabies/workflows/bold/boldref.py` & `nibabies-23.1.0rc0/nibabies/workflows/bold/boldref.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     To account for potential increased motion on the start of image acquisition, this
     workflow discards a bigger chunk of the initial frames.
 
     Parameters
     ----------
     omp_nthreads
         Maximum number of threads an individual process may use
-    has_sbref
+    is_sbref
         A single-band reference is provided.
     start_frame
         BOLD frame to start creating the reference map from. Any earlier frames are discarded.
 
     Inputs
     ------
     bold_file
@@ -53,15 +53,15 @@
         name='inputnode',
     )
     outputnode = pe.Node(
         niu.IdentityInterface(fields=['boldref_file', 'boldref_mask']),
         name='outputnode',
     )
 
-    epi_reference_wf = init_epi_reference_wf(omp_nthreads)
+    epi_reference_wf = init_epi_reference_wf(omp_nthreads, auto_bold_nss=False)
 
     boldref_mask = pe.Node(BrainExtraction(), name='boldref_mask')
 
     # fmt:off
     wf.connect([
         (inputnode, epi_reference_wf, [('epi_file', 'inputnode.in_files')]),
         (epi_reference_wf, boldref_mask, [('outputnode.epi_ref_file', 'in_file')]),
@@ -77,14 +77,18 @@
         select_frames.inputs.start_frame = start_frame
         # fmt:off
         wf.connect([
             (inputnode, select_frames, [('epi_file', 'in_file')]),
             (select_frames, epi_reference_wf, [('t_masks', 'inputnode.t_masks')]),
         ])
         # fmt:on
+    else:
+        # Won't be used but needed to placate iternode
+        # To consider: Add a check to ensure this is a 3D file
+        epi_reference_wf.inputs.inputnode.t_masks = [True]
     return wf
 
 
 def _select_frames(in_file: str, start_frame: int) -> list:
     import nibabel as nb
     import numpy as np
```

### Comparing `nibabies-23.0.0/nibabies/workflows/bold/confounds.py` & `nibabies-23.1.0rc0/nibabies/workflows/bold/confounds.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/workflows/bold/hmc.py` & `nibabies-23.1.0rc0/nibabies/workflows/bold/hmc.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/workflows/bold/outputs.py` & `nibabies-23.1.0rc0/nibabies/workflows/bold/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
     return timing_parameters
 
 
 def init_func_derivatives_wf(
     bids_root,
     cifti_output,
     freesurfer,
+    project_goodvoxels,
     all_metadata,
     multiecho,
     output_dir,
     spaces,
     use_aroma,
     name="func_derivatives_wf",
 ):
@@ -137,14 +138,18 @@
     ----------
     bids_root : :obj:`str`
         Original BIDS dataset path.
     cifti_output : :obj:`bool`
         Whether the ``--cifti-output`` flag was set.
     freesurfer : :obj:`bool`
         Whether FreeSurfer anatomical processing was run.
+    project_goodvoxels : :obj:`bool`
+        Whether the option was used to exclude voxels with
+        locally high coefficient of variation, or that lie outside the
+        cortical surfaces, from the surface projection.
     metadata : :obj:`dict`
         Metadata dictionary associated to the BOLD run.
     multiecho : :obj:`bool`
         Derivatives were generated from multi-echo time series.
     output_dir : :obj:`str`
         Where derivatives should be written out to.
     spaces : :py:class:`~niworkflows.utils.spaces.SpatialReferences`
@@ -202,14 +207,15 @@
                 "bold_native",
                 "bold_native_ref",
                 "bold_mask_native",
                 "cifti_metadata",
                 "cifti_density",
                 "confounds",
                 "confounds_metadata",
+                "goodvoxels_mask",
                 "melodic_mix",
                 "nonaggr_denoised_file",
                 "source_file",
                 "surf_files",
                 "surf_refs",
                 "template",
                 "spatial_reference",
@@ -775,14 +781,36 @@
             (inputnode, ds_bold_surfs, [('source_file', 'source_file')]),
             (select_fs_surf, ds_bold_surfs, [('surfaces', 'in_file'),
                                              ('key', 'space')]),
             (name_surfs, ds_bold_surfs, [('hemi', 'hemi')]),
         ])
         # fmt: on
 
+    if freesurfer and project_goodvoxels:
+        ds_goodvoxels_mask = pe.Node(
+            DerivativesDataSink(
+                base_directory=output_dir,
+                space='T1w',
+                desc='goodvoxels',
+                suffix='mask',
+                compress=True,
+                dismiss_entities=("echo",),
+            ),
+            name='ds_goodvoxels_mask',
+            run_without_submitting=True,
+            mem_gb=config.DEFAULT_MEMORY_MIN_GB,
+        )
+        # fmt:off
+        workflow.connect([
+            (inputnode, ds_goodvoxels_mask, [
+                ('source_file', 'source_file'),
+                ('goodvoxels_mask', 'in_file')]),
+        ])
+        # fmt:on
+
     # CIFTI output
     if cifti_output:
         ds_bold_cifti = pe.Node(
             DerivativesDataSink(
                 base_directory=output_dir,
                 suffix="bold",
                 compress=False,
```

### Comparing `nibabies-23.0.0/nibabies/workflows/bold/registration.py` & `nibabies-23.1.0rc0/nibabies/workflows/bold/registration.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/workflows/bold/stc.py` & `nibabies-23.1.0rc0/nibabies/workflows/bold/stc.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/nibabies/workflows/bold/t2s.py` & `nibabies-23.1.0rc0/nibabies/workflows/bold/t2s.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     Outputs
     -------
     bold
         the optimally combined time series for all supplied echos
 
     """
     from niworkflows.engine.workflows import LiterateWorkflow as Workflow
+    from niworkflows.interfaces.morphology import BinaryDilation
 
     workflow = Workflow(name=name)
     workflow.__desc__ = """\
 A T2\\* map was estimated from the preprocessed BOLD by fitting to a monoexponential signal
 decay model with nonlinear regression, using T2\\*/S0 estimates from a log-linear
 regression fit as initial values.
 For each voxel, the maximal number of echoes with reliable signal in that voxel were
@@ -72,20 +73,23 @@
 
     inputnode = pe.Node(niu.IdentityInterface(fields=["bold_file", "bold_mask"]), name="inputnode")
 
     outputnode = pe.Node(niu.IdentityInterface(fields=["bold", "t2star_map"]), name="outputnode")
 
     LOGGER.log(25, "Generating T2* map and optimally combined ME-EPI time series.")
 
+    dilate_mask = pe.Node(BinaryDilation(radius=2), name='dilate_mask')
+
     t2smap_node = pe.Node(T2SMap(echo_times=list(echo_times)), name="t2smap_node")
 
     # fmt: off
     workflow.connect([
-        (inputnode, t2smap_node, [('bold_file', 'in_files'),
-                                  ('bold_mask', 'mask_file')]),
+        (inputnode, dilate_mask, [('bold_mask', 'in_mask')]),
+        (inputnode, t2smap_node, [('bold_file', 'in_files')]),
+        (dilate_mask, t2smap_node, [('out_mask', 'mask_file')]),
         (t2smap_node, outputnode, [('optimal_comb', 'bold'),
                                    ('t2star_map', 't2star_map')]),
     ])
     # fmt: on
 
     return workflow
```

### Comparing `nibabies-23.0.0/scripts/anatprep.py` & `nibabies-23.1.0rc0/scripts/anatprep.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/scripts/bold_subcortical.py` & `nibabies-23.1.0rc0/scripts/bold_subcortical.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/scripts/check_outputs.py` & `nibabies-23.1.0rc0/scripts/check_outputs.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/scripts/fetch_templates.py` & `nibabies-23.1.0rc0/scripts/fetch_templates.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     tpl-fsLR/tpl-fsLR_hemi-R_den-32k_desc-nomedialwall_dparc.label.gii
     tpl-fsLR/tpl-fsLR_hemi-R_den-32k_desc-vaavg_midthickness.shape.gii
     tpl-fsLR/tpl-fsLR_hemi-R_den-32k_sphere.surf.gii
     tpl-fsLR/tpl-fsLR_space-fsaverage_hemi-L_den-32k_sphere.surf.gii
     tpl-fsLR/tpl-fsLR_space-fsaverage_hemi-R_den-32k_sphere.surf.gii
     """
     tf.get('fsLR', density='32k')
+    tf.get('fsLR', density="164k", desc="std", suffix="sphere")
+    tf.get('fsLR', density="164k", suffix="midthickness")
 
 
 def fetch_MNIInfant(cohort=1):
     """
     Expected templates:
 
     tpl-MNIInfant/cohort-1/tpl-MNIInfant_cohort-1_res-1_T1w.nii.gz
```

### Comparing `nibabies-23.0.0/wrapper/LICENSE` & `nibabies-23.1.0rc0/wrapper/LICENSE`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/wrapper/README.rst` & `nibabies-23.1.0rc0/wrapper/README.rst`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/wrapper/pyproject.toml` & `nibabies-23.1.0rc0/wrapper/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/wrapper/src/nibabies_wrapper/__main__.py` & `nibabies-23.1.0rc0/wrapper/src/nibabies_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/.gitignore` & `nibabies-23.1.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/LICENSE` & `nibabies-23.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/long_description.md` & `nibabies-23.1.0rc0/long_description.md`

 * *Files identical despite different names*

### Comparing `nibabies-23.0.0/pyproject.toml` & `nibabies-23.1.0rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,31 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 dependencies = [
-    "migas >= 0.3.0",
+    'importlib_resources; python_version < "3.9"',
     "nibabel >= 5.0.0",
-    "nipype >= 1.8.1",
+    "nipype >= 1.8.5",
     "nitime",
     "nitransforms >= 21.0.0",
-    "niworkflows ~= 1.7.1",
+    "niworkflows >= 1.8.1",
+#    "niworkflows @ git+https://github.com/nipreps/niworkflows.git@master",
     "numpy >= 1.21.0",
     "packaging",
     "pandas",
     "psutil >= 5.4",
     "pybids >= 0.15.0",
     "requests",
-    "sdcflows ~= 2.2.2",
-    "smriprep ~= 0.10.0",
+    "sdcflows >= 2.5.1",
+#    "sdcflows @ git+https://github.com/nipreps/sdcflows.git@master",
+    "smriprep >= 0.12.1",
+#    "smriprep @ git+https://github.com/nipreps/smriprep.git@master",
     "tedana ~= 0.0.12",
     "templateflow >= 0.6",
     "toml",
 ]
 dynamic = ["version"]
 
 [project.urls]
@@ -61,26 +64,27 @@
 duecredit = ["duecredit"]
 maint = [
     "fuzzywuzzy",
     "python-Levenshtein",
 ]
 test = [
     "coverage",
-    "codecov",
     "pytest",
     "pytest-cov",
     "pytest-env",
 ]
+telemetry = ["migas"]
 # Aliases
 docs = ["nibabies[doc]"]
 tests = ["nibabies[test]"]
 all = ["nibabies[dev,doc,maint,telemetry,test]"]
 
 [project.scripts]
 nibabies = "nibabies.cli.run:main"
+nibabies-mcribs = "nibabies.cli.mcribs:main"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.sdist]
 exclude = [".git_archival.txt"]  # No longer needed in sdist
```

### Comparing `nibabies-23.0.0/PKG-INFO` & `nibabies-23.1.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibabies
-Version: 23.0.0
+Version: 23.1.0rc0
 Summary: Processing workflows for magnetic resonance images of the brain in infants
 Project-URL: Documentation, https://nibabies.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/nipreps/nibabies
 Project-URL: Bug Tracker, https://github.com/nipreps/nibabies/issues
 Project-URL: Docker Images, https://hub.docker.com/r/nipreps/nibabies
 Author-email: The NiPreps Developers <nipreps@gmail.com>
 License:                                  Apache License
@@ -213,28 +213,28 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.8
-Requires-Dist: migas>=0.3.0
+Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: nibabel>=5.0.0
-Requires-Dist: nipype>=1.8.1
+Requires-Dist: nipype>=1.8.5
 Requires-Dist: nitime
 Requires-Dist: nitransforms>=21.0.0
-Requires-Dist: niworkflows~=1.7.1
+Requires-Dist: niworkflows>=1.8.1
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: packaging
 Requires-Dist: pandas
 Requires-Dist: psutil>=5.4
 Requires-Dist: pybids>=0.15.0
 Requires-Dist: requests
-Requires-Dist: sdcflows~=2.2.2
-Requires-Dist: smriprep~=0.10.0
+Requires-Dist: sdcflows>=2.5.1
+Requires-Dist: smriprep>=0.12.1
 Requires-Dist: tedana~=0.0.12
 Requires-Dist: templateflow>=0.6
 Requires-Dist: toml
 Provides-Extra: all
 Requires-Dist: nibabies[dev,doc,maint,telemetry,test]; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: black~=22.3.0; extra == 'dev'
@@ -249,16 +249,17 @@
 Provides-Extra: docs
 Requires-Dist: nibabies[doc]; extra == 'docs'
 Provides-Extra: duecredit
 Requires-Dist: duecredit; extra == 'duecredit'
 Provides-Extra: maint
 Requires-Dist: fuzzywuzzy; extra == 'maint'
 Requires-Dist: python-levenshtein; extra == 'maint'
+Provides-Extra: telemetry
+Requires-Dist: migas; extra == 'telemetry'
 Provides-Extra: test
-Requires-Dist: codecov; extra == 'test'
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-env; extra == 'test'
 Provides-Extra: tests
 Requires-Dist: nibabies[test]; extra == 'tests'
 Description-Content-Type: text/markdown
```


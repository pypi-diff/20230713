# Comparing `tmp/ascend_deployer-5.0.0b8-py3-none-any.whl.zip` & `tmp/ascend_deployer-5.0.0b9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,398 +1,404 @@
-Zip file size: 461406 bytes, number of entries: 396
--rw-------  2.0 unx      769 b- defN 23-Jun-21 08:01 ascend_deployer/__init__.py
--rw-rw-r--  2.0 unx      348 b- defN 23-Jun-21 08:03 ascend_deployer/ansible.cfg
--rw-------  2.0 unx     7530 b- defN 23-Jun-21 08:03 ascend_deployer/ascend_deployer.py
--rw-------  2.0 unx     2145 b- defN 23-Jun-21 08:03 ascend_deployer/ascend_download.py
--rw-------  2.0 unx     6023 b- defN 23-Jun-21 08:02 ascend_deployer/downloader_ui.py
--rwxr-x---  2.0 unx     4177 b- defN 23-Jun-21 08:02 ascend_deployer/install.sh
--rw-rw-r--  2.0 unx      460 b- defN 23-Jun-21 08:02 ascend_deployer/inventory_file
--rw-------  2.0 unx     5090 b- defN 23-Jun-21 08:02 ascend_deployer/jobs.py
--rwxr-x---  2.0 unx      475 b- defN 23-Jun-21 08:02 ascend_deployer/start_download.sh
--rw-rw-r--  2.0 unx       57 b- defN 23-Jun-21 08:02 ascend_deployer/start_download_ui.bat
--rw-------  2.0 unx     5429 b- defN 23-Jun-21 08:01 ascend_deployer/utils.py
--rw-rw-r--  2.0 unx       54 b- defN 23-Jun-21 08:01 ascend_deployer/version.json
--rw-rw-r--  2.0 unx    13742 b- defN 23-Jun-21 08:03 ascend_deployer/ansible_plugin/ansible_log.py
--rw-rw-r--  2.0 unx     1123 b- defN 23-Jun-21 08:03 ascend_deployer/ansible_plugin/install_info.yaml
--rw-rw-r--  2.0 unx     2225 b- defN 23-Jun-21 08:02 ascend_deployer/downloader/__init__.py
--rw-rw-r--  2.0 unx      137 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config.ini
--rw-rw-r--  2.0 unx    11014 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/deb_downloader.py
--rw-rw-r--  2.0 unx     3923 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dl_mef_dependency_downloader.py
--rw-rw-r--  2.0 unx    18796 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/download_util.py
--rw-rw-r--  2.0 unx    13079 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/downloader.py
--rw-rw-r--  2.0 unx     4552 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/logger_config.py
--rw-rw-r--  2.0 unx     2839 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/obs_downloader.py
--rw-rw-r--  2.0 unx     2730 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/obs_resources.json
--rw-rw-r--  2.0 unx     4562 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/os_dep_downloader.py
--rw-rw-r--  2.0 unx    14550 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/other_downloader.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/other_resources.json
--rw-rw-r--  2.0 unx    13377 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/pip_downloader.py
--rw-rw-r--  2.0 unx     8754 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/python_version.json
--rw-rw-r--  2.0 unx     1775 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/requirements.txt
--rw-rw-r--  2.0 unx    20876 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/rpm_downloader.py
--rw-rw-r--  2.0 unx     8430 b- defN 23-Jun-21 08:02 ascend_deployer/downloader/software_mgr.py
--rw-rw-r--  2.0 unx      462 b- defN 23-Jun-21 08:02 ascend_deployer/downloader/version_match.json
--rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json
--rw-rw-r--  2.0 unx      234 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/CentOS_7.6_aarch64/source.repo
--rw-rw-r--  2.0 unx    10223 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json
--rw-rw-r--  2.0 unx      371 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo
--rw-rw-r--  2.0 unx    43257 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/installed.txt
--rw-rw-r--  2.0 unx     4596 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json
--rw-rw-r--  2.0 unx      131 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/source.repo
--rw-rw-r--  2.0 unx    42707 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/installed.txt
--rw-rw-r--  2.0 unx     3668 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json
--rw-rw-r--  2.0 unx       65 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/source.repo
--rw-rw-r--  2.0 unx    65900 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/installed.txt
--rw-rw-r--  2.0 unx     6028 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json
--rw-rw-r--  2.0 unx      130 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/source.repo
--rw-rw-r--  2.0 unx    42840 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/installed.txt
--rw-rw-r--  2.0 unx     4518 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json
--rw-rw-r--  2.0 unx      130 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/source.repo
--rw-rw-r--  2.0 unx    42208 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/installed.txt
--rw-rw-r--  2.0 unx     3827 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json
--rw-rw-r--  2.0 unx       65 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/source.repo
--rw-rw-r--  2.0 unx    60396 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/installed.txt
--rw-rw-r--  2.0 unx     3388 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/pkg_info.json
--rw-rw-r--  2.0 unx      264 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo
--rw-rw-r--  2.0 unx    60964 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/installed.txt
--rw-rw-r--  2.0 unx     3201 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json
--rw-rw-r--  2.0 unx      253 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo
--rw-rw-r--  2.0 unx    51454 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/installed.txt
--rw-rw-r--  2.0 unx     3369 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/pkg_info.json
--rw-rw-r--  2.0 unx      365 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/source.repo
--rw-rw-r--  2.0 unx    51932 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/installed.txt
--rw-rw-r--  2.0 unx     3651 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json
--rw-rw-r--  2.0 unx      445 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/source.repo
--rw-rw-r--  2.0 unx    51351 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/installed.txt
--rw-rw-r--  2.0 unx     5439 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json
--rw-rw-r--  2.0 unx      458 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/source.repo
--rw-rw-r--  2.0 unx    43010 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/installed.txt
--rw-rw-r--  2.0 unx     3220 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json
--rw-rw-r--  2.0 unx      445 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo
--rw-rw-r--  2.0 unx    57488 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt
--rw-rw-r--  2.0 unx     2460 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json
--rw-rw-r--  2.0 unx      186 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo
--rw-rw-r--  2.0 unx     4204 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json
--rw-rw-r--  2.0 unx      370 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list
--rw-rw-r--  2.0 unx     5718 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json
--rw-rw-r--  2.0 unx      352 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/source.list
--rw-rw-r--  2.0 unx     5172 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json
--rw-rw-r--  2.0 unx      366 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/source.list
--rw-rw-r--  2.0 unx     6256 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json
--rw-rw-r--  2.0 unx      348 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/source.list
--rw-rw-r--  2.0 unx     5891 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json
--rw-rw-r--  2.0 unx      366 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/source.list
--rw-rw-r--  2.0 unx     6644 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json
--rw-rw-r--  2.0 unx      348 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list
--rw-rw-r--  2.0 unx     3637 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json
--rw-rw-r--  2.0 unx     3621 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json
--rw-rw-r--  2.0 unx     3629 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64/resource.json
--rw-rw-r--  2.0 unx     3613 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64/resource.json
--rw-rw-r--  2.0 unx     3709 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json
--rw-rw-r--  2.0 unx     3693 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json
--rw-rw-r--  2.0 unx     3709 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json
--rw-rw-r--  2.0 unx     3693 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json
--rw-rw-r--  2.0 unx     3653 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json
--rw-rw-r--  2.0 unx     3637 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json
--rw-rw-r--  2.0 unx     3653 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json
--rw-rw-r--  2.0 unx     3637 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_x86_64/resource.json
--rw-rw-r--  2.0 unx     3653 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_aarch64/resource.json
--rw-rw-r--  2.0 unx     3637 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json
--rw-rw-r--  2.0 unx     3616 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json
--rw-rw-r--  2.0 unx     3584 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json
--rw-rw-r--  2.0 unx      853 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json
--rw-rw-r--  2.0 unx      847 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json
--rw-rw-r--  2.0 unx     6044 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/software/CANN_6.0.1.json
--rw-rw-r--  2.0 unx     6358 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/software/CANN_6.0.RC1.json
--rw-rw-r--  2.0 unx     5435 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/software/CANN_6.3.RC1.json
--rw-rw-r--  2.0 unx       84 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/software/DL_5.0.RC1.json
--rw-rw-r--  2.0 unx       85 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/software/MEF_5.0.RC1.json
--rw-rw-r--  2.0 unx     5341 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/software/MindSpore_1.10.0.json
--rw-rw-r--  2.0 unx     5304 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/software/MindSpore_1.9.0.json
--rw-rw-r--  2.0 unx     5360 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/software/MindSpore_2.0.0rc1.json
--rw-rw-r--  2.0 unx    48361 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/software/MindStudio_5.0.0.json
--rw-rw-r--  2.0 unx    25492 b- defN 23-Jun-21 08:03 ascend_deployer/downloader/software/MindStudio_5.0.RC3.json
--rw-rw-r--  2.0 unx    48368 b- defN 23-Jun-21 08:02 ascend_deployer/downloader/software/MindStudio_6.0.RC1.json
--rw-rw-r--  2.0 unx     2890 b- defN 23-Jun-21 08:02 ascend_deployer/downloader/software/Torch-npu_1.11.0.json
--rw-rw-r--  2.0 unx     2906 b- defN 23-Jun-21 08:02 ascend_deployer/downloader/software/Torch-npu_1.11.0rc2.json
--rw-rw-r--  2.0 unx     2895 b- defN 23-Jun-21 08:02 ascend_deployer/downloader/software/Torch-npu_1.8.1.json
--rw-rw-r--  2.0 unx     2920 b- defN 23-Jun-21 08:02 ascend_deployer/downloader/software/Torch-npu_1.8.1.post1.json
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-21 08:02 ascend_deployer/downloader/yum_metadata/__init__.py
--rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-21 08:02 ascend_deployer/downloader/yum_metadata/create_yum_metadata_primary_db.sql
--rw-rw-r--  2.0 unx    11330 b- defN 23-Jun-21 08:02 ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py
--rw-rw-r--  2.0 unx     1709 b- defN 23-Jun-21 08:02 ascend_deployer/group_vars/all.yaml
--rw-rw-r--  2.0 unx      807 b- defN 23-Jun-21 08:02 ascend_deployer/patch/selenium_firefox.patch
--rw-rw-r--  2.0 unx     1127 b- defN 23-Jun-21 08:02 ascend_deployer/patch/selenium_firefox_profile.patch
--rw-rw-r--  2.0 unx      236 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/basic.yaml
--rw-rw-r--  2.0 unx      479 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/check.yaml
--rw-rw-r--  2.0 unx       94 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/check_pkgs.yml
--rw-rw-r--  2.0 unx      203 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/clean_nexus.yml
--rw-rw-r--  2.0 unx      611 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/create_nexus.yml
--rw-rw-r--  2.0 unx     1136 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/create_user.yml
--rw-rw-r--  2.0 unx      663 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/distribution.yml
--rw-rw-r--  2.0 unx      672 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/docker.yaml
--rw-rw-r--  2.0 unx     1021 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/gather_app_info.yml
--rw-rw-r--  2.0 unx     3487 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/gather_facts.yaml
--rw-rw-r--  2.0 unx     1019 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/gather_npu_fact.yml
--rw-rw-r--  2.0 unx      121 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/harbor.yaml
--rw-rw-r--  2.0 unx      122 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/hccn.yaml
--rw-rw-r--  2.0 unx      134 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/image_load.yaml
--rw-rw-r--  2.0 unx     2213 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/k8s.yaml
--rw-rw-r--  2.0 unx       85 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/kubeedge.yaml
--rw-rw-r--  2.0 unx     1654 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/mindxdl.yaml
--rw-rw-r--  2.0 unx      491 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/modify_user_group.yml
--rw-rw-r--  2.0 unx      225 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/os_map.yaml
--rw-rw-r--  2.0 unx     2065 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/os_map.yml
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml
--rw-rw-r--  2.0 unx     1687 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_aarch64.yml
--rw-rw-r--  2.0 unx     1687 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_x86_64.yml
--rw-rw-r--  2.0 unx     1076 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml
--rw-rw-r--  2.0 unx     1076 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml
--rw-rw-r--  2.0 unx      422 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/report.yaml
--rw-rw-r--  2.0 unx      139 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/set_facts_cache_permission.yml
--rw-rw-r--  2.0 unx      349 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/sync_time.yml
--rw-rw-r--  2.0 unx     6051 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/task_set_custom_fact.yml
--rw-rw-r--  2.0 unx      155 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/uninstall_mef_kubeedge.yaml
--rw-rw-r--  2.0 unx      246 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/uninstall_mef_releate.yaml
--rw-rw-r--  2.0 unx     5199 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/facts/app_info.fact.j2
--rw-rw-r--  2.0 unx     6392 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/facts/npu_info.fact.j2
--rw-rw-r--  2.0 unx      549 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_atlasedge.yml
--rw-rw-r--  2.0 unx      107 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_device_plugin.yml
--rw-rw-r--  2.0 unx      467 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_docker_images.yml
--rw-rw-r--  2.0 unx      109 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_docker_runtime.yml
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_driver.yml
--rw-rw-r--  2.0 unx     1298 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_firmware.yml
--rw-rw-r--  2.0 unx      896 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_gcc.yml
--rw-rw-r--  2.0 unx      521 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_ha.yml
--rw-rw-r--  2.0 unx       99 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_hccl.yml
--rw-rw-r--  2.0 unx      427 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_ief.yml
--rw-rw-r--  2.0 unx      216 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_kernels.yml
--rw-rw-r--  2.0 unx      927 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_mindspore.yml
--rw-rw-r--  2.0 unx     9154 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_mindstudio.yml
--rw-rw-r--  2.0 unx       96 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_nnae.yml
--rw-rw-r--  2.0 unx      210 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_nnrt.yml
--rw-rw-r--  2.0 unx      100 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_noded.yml
--rw-rw-r--  2.0 unx     1398 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_npu.yml
--rw-rw-r--  2.0 unx      107 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_npu_exporter.yml
--rw-rw-r--  2.0 unx      105 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_python.yml
--rw-rw-r--  2.0 unx     2523 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_pytorch.yml
--rw-rw-r--  2.0 unx      452 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_sys_pkg.yml
--rw-rw-r--  2.0 unx     3280 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_tensorflow.yml
--rw-rw-r--  2.0 unx      104 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_tfplugin.yml
--rw-rw-r--  2.0 unx      102 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_toolbox.yml
--rw-rw-r--  2.0 unx      216 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_toolkit.yml
--rw-rw-r--  2.0 unx      115 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/install_volcano.yml
--rw-rw-r--  2.0 unx     1456 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_atlasedge.yml
--rw-rw-r--  2.0 unx      663 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_cmake.yml
--rw-rw-r--  2.0 unx      653 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_dl.yml
--rw-rw-r--  2.0 unx      818 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_docker_images.yml
--rw-rw-r--  2.0 unx      239 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_driver.yml
--rw-rw-r--  2.0 unx     6360 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_driver_bcinux.yml
--rw-rw-r--  2.0 unx     6443 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_driver_common.yml
--rw-rw-r--  2.0 unx     5660 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_firmware.yml
--rw-rw-r--  2.0 unx     2210 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_gcc.yml
--rw-rw-r--  2.0 unx     3055 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_get_npu_scene.yml
--rw-rw-r--  2.0 unx     1227 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_ha.yml
--rw-rw-r--  2.0 unx      670 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_ief.yml
--rw-rw-r--  2.0 unx     2793 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_ief_a500.yml
--rw-rw-r--  2.0 unx     1681 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_ief_a500pro.yml
--rw-rw-r--  2.0 unx     1395 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_kernel.yml
--rw-rw-r--  2.0 unx     1317 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_kernel_euleros.yml
--rw-rw-r--  2.0 unx     9161 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_kernels.yml
--rw-rw-r--  2.0 unx     2044 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_mindspore.yml
--rw-rw-r--  2.0 unx     3890 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_nnae.yml
--rw-rw-r--  2.0 unx     3890 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_nnrt.yml
--rw-rw-r--  2.0 unx      709 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_protobuf.yml
--rw-rw-r--  2.0 unx     3209 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_python.yml
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_pytorch.yml
--rw-rw-r--  2.0 unx     1894 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_sys_apt.yml
--rw-rw-r--  2.0 unx     2108 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_sys_dnf.yml
--rw-rw-r--  2.0 unx     3230 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_sys_pkg.yml
--rw-rw-r--  2.0 unx     2112 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_sys_yum.yml
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_tensorflow.yml
--rw-rw-r--  2.0 unx     4120 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_tfplugin.yml
--rw-rw-r--  2.0 unx     3426 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_toolbox.yml
--rw-rw-r--  2.0 unx     7662 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/task_toolkit.yml
--rw-rw-r--  2.0 unx      102 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/install_nnae.yml
--rw-rw-r--  2.0 unx      219 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/install_nnrt.yml
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/install_tfplugin.yml
--rw-rw-r--  2.0 unx      225 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/install_toolkit.yml
--rw-rw-r--  2.0 unx      106 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/rollback_nnae.yml
--rw-rw-r--  2.0 unx      106 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/rollback_nnrt.yml
--rw-rw-r--  2.0 unx      114 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/rollback_tfplugin.yml
--rw-rw-r--  2.0 unx      112 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/rollback_toolkit.yml
--rw-rw-r--  2.0 unx     1375 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/task_nnae.yml
--rw-rw-r--  2.0 unx     1375 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/task_nnrt.yml
--rw-rw-r--  2.0 unx      675 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/task_rollback_nnae.yml
--rw-rw-r--  2.0 unx     1653 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/task_rollback_nnrt.yml
--rw-rw-r--  2.0 unx      734 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/task_rollback_tfplugin.yml
--rw-rw-r--  2.0 unx     1743 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/task_rollback_toolkit.yml
--rw-rw-r--  2.0 unx     1438 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/task_tfplugin.yml
--rw-rw-r--  2.0 unx     1311 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/install/patch/task_toolkit.yml
--rw-rw-r--  2.0 unx      369 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/process/process_check.yml
--rw-rw-r--  2.0 unx     3155 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/process/process_install.yml
--rw-rw-r--  2.0 unx      783 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/process/process_patch.yml
--rw-rw-r--  2.0 unx      787 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/process/process_patch_rollback.yml
--rw-rw-r--  2.0 unx     2144 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/process/process_scene.yml
--rw-rw-r--  2.0 unx      969 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/process/process_test.yml
--rw-rw-r--  2.0 unx      310 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.basic/defaults/main.yml
--rw-rw-r--  2.0 unx     1258 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.basic/files/space.sh
--rw-rw-r--  2.0 unx     4154 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.basic/tasks/check.yml
--rw-rw-r--  2.0 unx     1437 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml
--rw-rw-r--  2.0 unx     4660 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml
--rw-rw-r--  2.0 unx     4892 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_status_check.yml
--rw-rw-r--  2.0 unx    10079 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.check/defaults/compatibility_map.yml
--rw-rw-r--  2.0 unx      363 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.check/tasks/compatibility_check.yml
--rw-rw-r--  2.0 unx       76 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/README.md
--rw-rw-r--  2.0 unx     1296 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/defaults/main.yml
--rw-rw-r--  2.0 unx      181 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/meta/main.yml
--rw-rw-r--  2.0 unx     9771 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml
--rw-rw-r--  2.0 unx      675 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/tasks/create_user.yaml
--rw-rw-r--  2.0 unx    12772 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/tasks/deviceplugin.yaml
--rw-rw-r--  2.0 unx     7226 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/tasks/distribute_soft_package.yaml
--rw-rw-r--  2.0 unx      726 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/tasks/dl_common.yaml
--rw-rw-r--  2.0 unx     1517 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/tasks/docker-runtime.yaml
--rw-rw-r--  2.0 unx     5612 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/tasks/hccl.yaml
--rw-rw-r--  2.0 unx     5867 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/tasks/noded.yaml
--rw-rw-r--  2.0 unx     5511 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/tasks/npu-exporter.yaml
--rw-rw-r--  2.0 unx     4347 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/tasks/push_image.yaml
--rw-rw-r--  2.0 unx     7379 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml
--rw-rw-r--  2.0 unx       67 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.docker/README.md
--rw-rw-r--  2.0 unx      171 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.docker/meta/main.yml
--rw-rw-r--  2.0 unx      500 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.docker/tasks/copy.yml
--rw-rw-r--  2.0 unx      418 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml
--rw-rw-r--  2.0 unx      892 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.docker/tasks/post_install.yml
--rw-rw-r--  2.0 unx       55 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.docker/tests/ansible.cfg
--rw-rw-r--  2.0 unx       37 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.docker/tests/inventory
--rw-rw-r--  2.0 unx      116 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.docker/tests/test.yml
--rw-rw-r--  2.0 unx       99 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.docker/vars/main.yml
--rw-rw-r--  2.0 unx     1314 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.harbor/tasks/check.yml
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.harbor/tasks/http.yml
--rw-rw-r--  2.0 unx      346 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.harbor/tasks/https.yml
--rw-rw-r--  2.0 unx     1157 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.harbor/tasks/main.yml
--rw-rw-r--  2.0 unx       42 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.harbor/vars/main.yml
--rw-rw-r--  2.0 unx     1723 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.hccn/tasks/hccn_conf.yaml
--rw-rw-r--  2.0 unx      660 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.image/tasks/image_load.yaml
--rw-rw-r--  2.0 unx      536 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/README.md
--rw-rw-r--  2.0 unx      234 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/defaults/main.yml
--rw-rw-r--  2.0 unx      929 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/files/10-kubeadm.conf
--rw-rw-r--  2.0 unx      283 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/files/kubelet.service
--rw-rw-r--  2.0 unx      179 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/meta/main.yml
--rw-rw-r--  2.0 unx      691 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/containerd.yml
--rw-rw-r--  2.0 unx     1599 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml
--rw-rw-r--  2.0 unx      774 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml
--rw-rw-r--  2.0 unx      693 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/get_k8s_version.yml
--rw-rw-r--  2.0 unx      869 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml
--rw-rw-r--  2.0 unx     1235 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml
--rw-rw-r--  2.0 unx      897 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/os_setting.yml
--rw-rw-r--  2.0 unx     4727 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/push_image.yml
--rw-rw-r--  2.0 unx     1805 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/kubevip/main.yml
--rw-rw-r--  2.0 unx     3557 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master/main.yml
--rw-rw-r--  2.0 unx     1596 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master_backup/main.yml
--rw-rw-r--  2.0 unx      860 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tasks/worker/main.yml
--rw-rw-r--  2.0 unx   202740 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.20.2.yaml
--rw-rw-r--  2.0 unx       55 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tests/ansible.cfg
--rw-rw-r--  2.0 unx       37 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tests/inventory
--rw-rw-r--  2.0 unx      116 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/tests/test.yml
--rw-rw-r--  2.0 unx      485 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.k8s/vars/main.yml
--rw-rw-r--  2.0 unx       78 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/README.md
--rw-rw-r--  2.0 unx      243 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/defaults/main.yml
--rw-rw-r--  2.0 unx     3498 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/files/certgen.sh
--rw-rw-r--  2.0 unx      162 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cloudcore.service
--rw-rw-r--  2.0 unx     1896 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cluster_objectsync_v1alpha1.yaml
--rw-rw-r--  2.0 unx     8715 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_device.yaml
--rw-rw-r--  2.0 unx    10576 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_devicemodel.yaml
--rw-rw-r--  2.0 unx     1877 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/files/objectsync_v1alpha1.yaml
--rw-rw-r--  2.0 unx     2443 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_rule.yaml
--rw-rw-r--  2.0 unx     1355 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_ruleEndpoint.yaml
--rw-rw-r--  2.0 unx      176 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/meta/main.yml
--rw-rw-r--  2.0 unx     5153 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml
--rw-rw-r--  2.0 unx      144 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.rep/defaults/main.yml
--rw-rw-r--  2.0 unx      528 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.rep/tasks/get_npu_info.py
--rw-rw-r--  2.0 unx     2046 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.rep/tasks/hccn_rep.yaml
--rw-rw-r--  2.0 unx     2268 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py
--rw-rw-r--  2.0 unx     1146 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.rep/tasks/local_rep.yaml
--rw-rw-r--  2.0 unx     1011 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.rep/tasks/ls_format.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.rep/tasks/output_json.py
--rw-rw-r--  2.0 unx     1839 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.rep/tasks/packages_rep.yaml
--rw-rw-r--  2.0 unx      389 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_k8s_docker.yaml
--rw-rw-r--  2.0 unx      390 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_mef_kubeedge.yaml
--rw-rw-r--  2.0 unx      960 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_auto.yml
--rw-rw-r--  2.0 unx      613 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_dl.yml
--rw-rw-r--  2.0 unx      259 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_edge.yml
--rw-rw-r--  2.0 unx      357 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_mef.yml
--rw-rw-r--  2.0 unx      514 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_mindspore.yml
--rw-rw-r--  2.0 unx      435 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_offline_dev.yml
--rw-rw-r--  2.0 unx      354 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_offline_run.yml
--rw-rw-r--  2.0 unx      510 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_pytorch_dev.yml
--rw-rw-r--  2.0 unx      504 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_pytorch_run.yml
--rw-rw-r--  2.0 unx      593 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_tensorflow_dev.yml
--rw-rw-r--  2.0 unx      587 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_tensorflow_run.yml
--rw-rw-r--  2.0 unx      273 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/scene/scene_vmhost.yml
--rw-rw-r--  2.0 unx     2180 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/case_driver.yml
--rw-rw-r--  2.0 unx      567 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/case_firmware.yml
--rw-rw-r--  2.0 unx     2614 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/case_mindspore.yml
--rw-rw-r--  2.0 unx     1466 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/case_nnae.yml
--rw-rw-r--  2.0 unx     1466 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/case_nnrt.yml
--rw-rw-r--  2.0 unx     3095 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/case_pytorch.yml
--rw-rw-r--  2.0 unx     6827 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/case_tensorflow.yml
--rw-rw-r--  2.0 unx     1514 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/case_tfplugin.yml
--rw-rw-r--  2.0 unx     1149 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/case_toolbox.yml
--rw-rw-r--  2.0 unx     1509 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/case_toolkit.yml
--rw-rw-r--  2.0 unx      608 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/test_all.yml
--rw-rw-r--  2.0 unx      284 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/test_driver.yml
--rw-rw-r--  2.0 unx      284 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/test_firmware.yml
--rw-rw-r--  2.0 unx       99 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/test_mindspore.yml
--rw-rw-r--  2.0 unx       90 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/test_nnae.yml
--rw-rw-r--  2.0 unx       89 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/test_nnrt.yml
--rw-rw-r--  2.0 unx       96 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/test_pytorch.yml
--rw-rw-r--  2.0 unx      101 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/test_tensorflow.yml
--rw-rw-r--  2.0 unx       97 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/test_tfplugin.yml
--rw-rw-r--  2.0 unx      104 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/test_toolbox.yml
--rw-rw-r--  2.0 unx       95 b- defN 23-Jun-21 08:02 ascend_deployer/playbooks/test/test_toolkit.yml
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/__init__.py
--rw-rw-r--  2.0 unx    20831 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/check_pkgs.sh
--rw-rw-r--  2.0 unx     1116 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/hccn_set.sh
--rw-rw-r--  2.0 unx     1142 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/image_load.sh
--rw-rw-r--  2.0 unx      969 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/install.sh
--rw-rw-r--  2.0 unx     3587 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/install_ansible.sh
--rw-rw-r--  2.0 unx    14207 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/nexus.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/nexus_config.json
--rw-rw-r--  2.0 unx    15393 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/prepare.sh
--rw-rw-r--  2.0 unx      535 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/uninstall_k8s_docker.sh
--rw-rw-r--  2.0 unx      643 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/uninstall_mef_kubeedge.sh
--rw-rw-r--  2.0 unx      679 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/uninstall_mef_related.sh
--rw-rw-r--  2.0 unx     5723 b- defN 23-Jun-21 08:02 ascend_deployer/scripts/utils.sh
--rw-rw-r--  2.0 unx    10900 b- defN 23-Jun-21 08:02 ascend_deployer/tools/DeviceIP-conf.sh
--rw-rw-r--  2.0 unx     1409 b- defN 23-Jun-21 08:02 ascend_deployer/tools/ascend-deployer
--rw-rw-r--  2.0 unx     4049 b- defN 23-Jun-21 08:02 ascend_deployer/tools/check.py
--rw-rw-r--  2.0 unx     7740 b- defN 23-Jun-21 08:02 ascend_deployer/tools/hccn.py
--rw-rw-r--  2.0 unx     9930 b- defN 23-Jun-21 08:02 ascend_deployer/tools/update_crl.sh
--rw-rw-r--  2.0 unx       21 b- defN 23-Jun-21 08:02 ascend_deployer/tools/hccn/main/go.mod
--rw-rw-r--  2.0 unx     6863 b- defN 23-Jun-21 08:02 ascend_deployer/tools/hccn/main/hccn.go
--rw-rw-r--  2.0 unx      142 b- defN 23-Jun-21 08:02 ascend_deployer/tools/report/main/go.mod
--rw-rw-r--  2.0 unx    18729 b- defN 23-Jun-21 08:02 ascend_deployer/tools/report/main/main.go
--rw-rw-r--  2.0 unx       21 b- defN 23-Jun-21 08:02 ascend_deployer/tools/unzip/main/go.mod
--rw-rw-r--  2.0 unx     1587 b- defN 23-Jun-21 08:02 ascend_deployer/tools/unzip/main/unzip.go
--rw-rw-r--  2.0 unx       46 b- defN 23-Jun-21 08:01 ascend_deployer/yamls/basic.yaml
--rw-rw-r--  2.0 unx       46 b- defN 23-Jun-21 08:01 ascend_deployer/yamls/check.yaml
--rw-rw-r--  2.0 unx      132 b- defN 23-Jun-21 08:01 ascend_deployer/yamls/docker.yaml
--rw-rw-r--  2.0 unx       53 b- defN 23-Jun-21 08:01 ascend_deployer/yamls/gather_facts.yaml
--rw-rw-r--  2.0 unx       72 b- defN 23-Jun-21 08:01 ascend_deployer/yamls/harbor.yaml
--rw-rw-r--  2.0 unx       45 b- defN 23-Jun-21 08:01 ascend_deployer/yamls/hccn.yaml
--rw-rw-r--  2.0 unx       51 b- defN 23-Jun-21 08:01 ascend_deployer/yamls/image_load.yaml
--rw-rw-r--  2.0 unx      126 b- defN 23-Jun-21 08:01 ascend_deployer/yamls/k8s.yaml
--rw-rw-r--  2.0 unx      234 b- defN 23-Jun-21 08:01 ascend_deployer/yamls/k8s_reset.yaml
--rw-rw-r--  2.0 unx       74 b- defN 23-Jun-21 08:01 ascend_deployer/yamls/mindxdl.yaml
--rw-rw-r--  2.0 unx       47 b- defN 23-Jun-21 08:01 ascend_deployer/yamls/report.yaml
--rwxr-xr-x  2.0 unx     1409 b- defN 23-Jun-21 08:04 ascend_deployer-5.0.0b8.data/scripts/ascend-deployer
--rw-------  2.0 unx     2739 b- defN 23-Jun-21 08:04 ascend_deployer-5.0.0b8.dist-info/DESCRIPTION.rst
--rw-------  2.0 unx       74 b- defN 23-Jun-21 08:04 ascend_deployer-5.0.0b8.dist-info/entry_points.txt
--rw-------  2.0 unx      777 b- defN 23-Jun-21 08:04 ascend_deployer-5.0.0b8.dist-info/metadata.json
--rw-------  2.0 unx       16 b- defN 23-Jun-21 08:04 ascend_deployer-5.0.0b8.dist-info/top_level.txt
--rw-------  2.0 unx       92 b- defN 23-Jun-21 08:04 ascend_deployer-5.0.0b8.dist-info/WHEEL
--rw-------  2.0 unx     3183 b- defN 23-Jun-21 08:04 ascend_deployer-5.0.0b8.dist-info/METADATA
--rw-------  2.0 unx    44578 b- defN 23-Jun-21 08:04 ascend_deployer-5.0.0b8.dist-info/RECORD
-396 files, 1910146 bytes uncompressed, 387582 bytes compressed:  79.7%
+Zip file size: 469552 bytes, number of entries: 402
+-rw-------  2.0 unx      769 b- defN 23-Jun-30 09:36 ascend_deployer/__init__.py
+-rw-rw-r--  2.0 unx      371 b- defN 23-Jun-30 09:36 ascend_deployer/ansible.cfg
+-rw-------  2.0 unx     7656 b- defN 23-Jun-30 09:36 ascend_deployer/ascend_deployer.py
+-rw-------  2.0 unx     2145 b- defN 23-Jun-30 09:36 ascend_deployer/ascend_download.py
+-rw-------  2.0 unx     6023 b- defN 23-Jun-30 09:36 ascend_deployer/downloader_ui.py
+-rwxr-x---  2.0 unx      898 b- defN 23-Jun-30 09:36 ascend_deployer/install.sh
+-rw-rw-r--  2.0 unx      460 b- defN 23-Jun-30 09:36 ascend_deployer/inventory_file
+-rw-------  2.0 unx     5375 b- defN 23-Jun-30 09:36 ascend_deployer/jobs.py
+-rwxr-x---  2.0 unx      475 b- defN 23-Jun-30 09:36 ascend_deployer/start_download.sh
+-rw-rw-r--  2.0 unx       57 b- defN 23-Jun-30 09:36 ascend_deployer/start_download_ui.bat
+-rw-------  2.0 unx     5429 b- defN 23-Jun-30 09:36 ascend_deployer/utils.py
+-rw-rw-r--  2.0 unx       54 b- defN 23-Jun-30 09:36 ascend_deployer/version.json
+-rw-rw-r--  2.0 unx    14646 b- defN 23-Jun-30 09:36 ascend_deployer/ansible_plugin/ansible_log.py
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Jun-30 09:36 ascend_deployer/ansible_plugin/install_info.yaml
+-rw-rw-r--  2.0 unx     2225 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/__init__.py
+-rw-rw-r--  2.0 unx      137 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config.ini
+-rw-rw-r--  2.0 unx    11022 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/deb_downloader.py
+-rw-rw-r--  2.0 unx     3923 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dl_mef_dependency_downloader.py
+-rw-rw-r--  2.0 unx    18816 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/download_util.py
+-rw-rw-r--  2.0 unx    13079 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/downloader.py
+-rw-rw-r--  2.0 unx     4554 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/logger_config.py
+-rw-rw-r--  2.0 unx     2839 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/obs_downloader.py
+-rw-rw-r--  2.0 unx     2730 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/obs_resources.json
+-rw-rw-r--  2.0 unx     4562 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/os_dep_downloader.py
+-rw-rw-r--  2.0 unx    14550 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/other_downloader.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/other_resources.json
+-rw-rw-r--  2.0 unx    13387 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/pip_downloader.py
+-rw-rw-r--  2.0 unx     8754 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/python_version.json
+-rw-rw-r--  2.0 unx     1775 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/requirements.txt
+-rw-rw-r--  2.0 unx    20157 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/rpm_downloader.py
+-rw-rw-r--  2.0 unx     8446 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software_mgr.py
+-rw-rw-r--  2.0 unx      462 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/version_match.json
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json
+-rw-rw-r--  2.0 unx      234 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/CentOS_7.6_aarch64/source.repo
+-rw-rw-r--  2.0 unx    10223 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json
+-rw-rw-r--  2.0 unx      371 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo
+-rw-rw-r--  2.0 unx    43257 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/installed.txt
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json
+-rw-rw-r--  2.0 unx      131 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/source.repo
+-rw-rw-r--  2.0 unx    42707 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/installed.txt
+-rw-rw-r--  2.0 unx     5062 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/source.repo
+-rw-rw-r--  2.0 unx    65900 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/installed.txt
+-rw-rw-r--  2.0 unx     9438 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json
+-rw-rw-r--  2.0 unx      130 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/source.repo
+-rw-rw-r--  2.0 unx    42840 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/installed.txt
+-rw-rw-r--  2.0 unx     8487 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json
+-rw-rw-r--  2.0 unx      130 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/source.repo
+-rw-rw-r--  2.0 unx    42208 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/installed.txt
+-rw-rw-r--  2.0 unx     8029 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json
+-rw-rw-r--  2.0 unx       65 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/source.repo
+-rw-rw-r--  2.0 unx    60396 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/installed.txt
+-rw-rw-r--  2.0 unx     3388 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/pkg_info.json
+-rw-rw-r--  2.0 unx      264 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo
+-rw-rw-r--  2.0 unx    60964 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/installed.txt
+-rw-rw-r--  2.0 unx     3201 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json
+-rw-rw-r--  2.0 unx      253 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo
+-rw-rw-r--  2.0 unx    51454 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/installed.txt
+-rw-rw-r--  2.0 unx     3369 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/pkg_info.json
+-rw-rw-r--  2.0 unx      365 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/source.repo
+-rw-rw-r--  2.0 unx    51932 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/installed.txt
+-rw-rw-r--  2.0 unx     3651 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json
+-rw-rw-r--  2.0 unx      445 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/source.repo
+-rw-rw-r--  2.0 unx    51351 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/installed.txt
+-rw-rw-r--  2.0 unx     5439 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json
+-rw-rw-r--  2.0 unx      458 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/source.repo
+-rw-rw-r--  2.0 unx    43010 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/installed.txt
+-rw-rw-r--  2.0 unx     3220 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json
+-rw-rw-r--  2.0 unx      445 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo
+-rw-rw-r--  2.0 unx    56970 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt
+-rw-rw-r--  2.0 unx     3134 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json
+-rw-rw-r--  2.0 unx      268 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo
+-rw-rw-r--  2.0 unx     4204 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json
+-rw-rw-r--  2.0 unx      370 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list
+-rw-rw-r--  2.0 unx     5718 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json
+-rw-rw-r--  2.0 unx      352 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/source.list
+-rw-rw-r--  2.0 unx     5172 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json
+-rw-rw-r--  2.0 unx      366 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/source.list
+-rw-rw-r--  2.0 unx     6256 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json
+-rw-rw-r--  2.0 unx      348 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/source.list
+-rw-rw-r--  2.0 unx     5891 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json
+-rw-rw-r--  2.0 unx      366 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/source.list
+-rw-rw-r--  2.0 unx     6644 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json
+-rw-rw-r--  2.0 unx      348 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list
+-rw-rw-r--  2.0 unx     3637 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json
+-rw-rw-r--  2.0 unx     3621 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json
+-rw-rw-r--  2.0 unx     3629 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64/resource.json
+-rw-rw-r--  2.0 unx     3613 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64/resource.json
+-rw-rw-r--  2.0 unx     3709 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json
+-rw-rw-r--  2.0 unx     3693 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json
+-rw-rw-r--  2.0 unx     3709 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json
+-rw-rw-r--  2.0 unx     3693 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json
+-rw-rw-r--  2.0 unx     3653 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json
+-rw-rw-r--  2.0 unx     3637 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json
+-rw-rw-r--  2.0 unx     3653 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json
+-rw-rw-r--  2.0 unx     3637 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_x86_64/resource.json
+-rw-rw-r--  2.0 unx     3653 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_aarch64/resource.json
+-rw-rw-r--  2.0 unx     3637 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json
+-rw-rw-r--  2.0 unx     4358 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json
+-rw-rw-r--  2.0 unx     4324 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json
+-rw-rw-r--  2.0 unx      853 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json
+-rw-rw-r--  2.0 unx      847 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json
+-rw-rw-r--  2.0 unx     6044 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/CANN_6.0.1.json
+-rw-rw-r--  2.0 unx     6358 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/CANN_6.0.RC1.json
+-rw-rw-r--  2.0 unx     5435 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/CANN_6.3.RC1.json
+-rw-rw-r--  2.0 unx       84 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/DL_5.0.RC1.json
+-rw-rw-r--  2.0 unx       85 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/MEF_5.0.RC1.json
+-rw-rw-r--  2.0 unx     5341 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/MindSpore_1.10.0.json
+-rw-rw-r--  2.0 unx     5304 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/MindSpore_1.9.0.json
+-rw-rw-r--  2.0 unx     5360 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/MindSpore_2.0.0rc1.json
+-rw-rw-r--  2.0 unx    48361 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/MindStudio_5.0.0.json
+-rw-rw-r--  2.0 unx    25492 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/MindStudio_5.0.RC3.json
+-rw-rw-r--  2.0 unx    48368 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/MindStudio_6.0.RC1.json
+-rw-rw-r--  2.0 unx     2890 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/Torch-npu_1.11.0.json
+-rw-rw-r--  2.0 unx     2906 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/Torch-npu_1.11.0rc2.json
+-rw-rw-r--  2.0 unx     2895 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/Torch-npu_1.8.1.json
+-rw-rw-r--  2.0 unx     2920 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/software/Torch-npu_1.8.1.post1.json
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/yum_metadata/__init__.py
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/yum_metadata/create_yum_metadata_primary_db.sql
+-rw-rw-r--  2.0 unx    11352 b- defN 23-Jun-30 09:36 ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py
+-rw-rw-r--  2.0 unx     1870 b- defN 23-Jun-30 09:36 ascend_deployer/group_vars/all.yaml
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jun-30 09:36 ascend_deployer/patch/selenium_firefox.patch
+-rw-rw-r--  2.0 unx     1127 b- defN 23-Jun-30 09:36 ascend_deployer/patch/selenium_firefox_profile.patch
+-rw-rw-r--  2.0 unx      236 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/basic.yaml
+-rw-rw-r--  2.0 unx      479 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/check.yaml
+-rw-rw-r--  2.0 unx       94 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/check_pkgs.yml
+-rw-rw-r--  2.0 unx      249 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/clean_nexus.yml
+-rw-rw-r--  2.0 unx      611 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/create_nexus.yml
+-rw-rw-r--  2.0 unx     1136 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/create_user.yml
+-rw-rw-r--  2.0 unx      663 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/distribution.yml
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/docker.yaml
+-rw-rw-r--  2.0 unx     1021 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/gather_app_info.yml
+-rw-rw-r--  2.0 unx     3487 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/gather_facts.yaml
+-rw-rw-r--  2.0 unx     1019 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/gather_npu_fact.yml
+-rw-rw-r--  2.0 unx      121 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/harbor.yaml
+-rw-rw-r--  2.0 unx      193 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/hccn.yaml
+-rw-rw-r--  2.0 unx      134 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/image_load.yaml
+-rw-rw-r--  2.0 unx     2142 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/k8s.yaml
+-rw-rw-r--  2.0 unx       85 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/kubeedge.yaml
+-rw-rw-r--  2.0 unx     2180 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/mindxdl.yaml
+-rw-rw-r--  2.0 unx      491 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/modify_user_group.yml
+-rw-rw-r--  2.0 unx      225 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/os_map.yaml
+-rw-rw-r--  2.0 unx     2065 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/os_map.yml
+-rw-rw-r--  2.0 unx     1056 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml
+-rw-rw-r--  2.0 unx     1056 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml
+-rw-rw-r--  2.0 unx     1653 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_aarch64.yml
+-rw-rw-r--  2.0 unx     1653 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_x86_64.yml
+-rw-rw-r--  2.0 unx     1652 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml
+-rw-rw-r--  2.0 unx     1652 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml
+-rw-rw-r--  2.0 unx      422 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/report.yaml
+-rw-rw-r--  2.0 unx      139 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/set_facts_cache_permission.yml
+-rw-rw-r--  2.0 unx      349 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/sync_time.yml
+-rw-rw-r--  2.0 unx     6051 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/task_set_custom_fact.yml
+-rw-rw-r--  2.0 unx      155 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/uninstall_mef_kubeedge.yaml
+-rw-rw-r--  2.0 unx      246 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/uninstall_mef_releate.yaml
+-rw-rw-r--  2.0 unx     5199 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/facts/app_info.fact.j2
+-rw-rw-r--  2.0 unx     6392 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/facts/npu_info.fact.j2
+-rw-rw-r--  2.0 unx      107 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_ascend-device-plugin.yml
+-rw-rw-r--  2.0 unx      109 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_ascend-docker-runtime.yml
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_ascend-operator.yml
+-rw-rw-r--  2.0 unx      549 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_atlasedge.yml
+-rw-rw-r--  2.0 unx      467 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_docker_images.yml
+-rw-rw-r--  2.0 unx     1264 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_driver.yml
+-rw-rw-r--  2.0 unx     1297 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_firmware.yml
+-rw-rw-r--  2.0 unx      896 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_gcc.yml
+-rw-rw-r--  2.0 unx      522 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_ha.yml
+-rw-rw-r--  2.0 unx       99 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_hccl-controller.yml
+-rw-rw-r--  2.0 unx      427 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_ief.yml
+-rw-rw-r--  2.0 unx      216 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_kernels.yml
+-rw-rw-r--  2.0 unx      927 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_mindspore.yml
+-rw-rw-r--  2.0 unx     9154 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_mindstudio.yml
+-rw-rw-r--  2.0 unx       96 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_nnae.yml
+-rw-rw-r--  2.0 unx      210 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_nnrt.yml
+-rw-rw-r--  2.0 unx      100 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_noded.yml
+-rw-rw-r--  2.0 unx      107 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_npu-exporter.yml
+-rw-rw-r--  2.0 unx     1398 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_npu.yml
+-rw-rw-r--  2.0 unx      105 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_python.yml
+-rw-rw-r--  2.0 unx     2524 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_pytorch.yml
+-rw-rw-r--  2.0 unx      116 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_resilience-controller.yml
+-rw-rw-r--  2.0 unx      452 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_sys_pkg.yml
+-rw-rw-r--  2.0 unx     3280 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_tensorflow.yml
+-rw-rw-r--  2.0 unx      104 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_tfplugin.yml
+-rw-rw-r--  2.0 unx      102 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_toolbox.yml
+-rw-rw-r--  2.0 unx      216 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_toolkit.yml
+-rw-rw-r--  2.0 unx      115 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/install_volcano.yml
+-rw-rw-r--  2.0 unx     1456 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_atlasedge.yml
+-rw-rw-r--  2.0 unx      663 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_cmake.yml
+-rw-rw-r--  2.0 unx      653 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_dl.yml
+-rw-rw-r--  2.0 unx      818 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_docker_images.yml
+-rw-rw-r--  2.0 unx      239 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_driver.yml
+-rw-rw-r--  2.0 unx     6278 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_driver_bcinux.yml
+-rw-rw-r--  2.0 unx     6361 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_driver_common.yml
+-rw-rw-r--  2.0 unx     5578 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_firmware.yml
+-rw-rw-r--  2.0 unx     2210 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_gcc.yml
+-rw-rw-r--  2.0 unx     3055 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_get_npu_scene.yml
+-rw-rw-r--  2.0 unx     1227 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_ha.yml
+-rw-rw-r--  2.0 unx      670 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_ief.yml
+-rw-rw-r--  2.0 unx     2777 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_ief_a500.yml
+-rw-rw-r--  2.0 unx     1665 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_ief_a500pro.yml
+-rw-rw-r--  2.0 unx     1337 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_kernel.yml
+-rw-rw-r--  2.0 unx     1242 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_kernel_euleros.yml
+-rw-rw-r--  2.0 unx     9377 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_kernels.yml
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_mindspore.yml
+-rw-rw-r--  2.0 unx     3767 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_nnae.yml
+-rw-rw-r--  2.0 unx     3768 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_nnrt.yml
+-rw-rw-r--  2.0 unx      709 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_protobuf.yml
+-rw-rw-r--  2.0 unx     3209 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_python.yml
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_pytorch.yml
+-rw-rw-r--  2.0 unx     1812 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_sys_apt.yml
+-rw-rw-r--  2.0 unx     2263 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_sys_dnf.yml
+-rw-rw-r--  2.0 unx     3230 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_sys_pkg.yml
+-rw-rw-r--  2.0 unx     2267 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_sys_yum.yml
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_tensorflow.yml
+-rw-rw-r--  2.0 unx     3997 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_tfplugin.yml
+-rw-rw-r--  2.0 unx     3262 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_toolbox.yml
+-rw-rw-r--  2.0 unx     7416 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/task_toolkit.yml
+-rw-rw-r--  2.0 unx      102 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/install_nnae.yml
+-rw-rw-r--  2.0 unx      219 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/install_nnrt.yml
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/install_tfplugin.yml
+-rw-rw-r--  2.0 unx      225 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/install_toolkit.yml
+-rw-rw-r--  2.0 unx      106 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/rollback_nnae.yml
+-rw-rw-r--  2.0 unx      106 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/rollback_nnrt.yml
+-rw-rw-r--  2.0 unx      114 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/rollback_tfplugin.yml
+-rw-rw-r--  2.0 unx      112 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/rollback_toolkit.yml
+-rw-rw-r--  2.0 unx     1334 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/task_nnae.yml
+-rw-rw-r--  2.0 unx     1334 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/task_nnrt.yml
+-rw-rw-r--  2.0 unx      634 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/task_rollback_nnae.yml
+-rw-rw-r--  2.0 unx     1651 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/task_rollback_nnrt.yml
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/task_rollback_tfplugin.yml
+-rw-rw-r--  2.0 unx     1661 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/task_rollback_toolkit.yml
+-rw-rw-r--  2.0 unx     1397 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/task_tfplugin.yml
+-rw-rw-r--  2.0 unx     1270 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/install/patch/task_toolkit.yml
+-rw-rw-r--  2.0 unx      369 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/process/process_check.yml
+-rw-rw-r--  2.0 unx     3539 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/process/process_install.yml
+-rw-rw-r--  2.0 unx      783 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/process/process_patch.yml
+-rw-rw-r--  2.0 unx      787 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/process/process_patch_rollback.yml
+-rw-rw-r--  2.0 unx     2144 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/process/process_scene.yml
+-rw-rw-r--  2.0 unx     1049 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/process/process_test.yml
+-rw-rw-r--  2.0 unx      310 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.basic/defaults/main.yml
+-rw-rw-r--  2.0 unx     1258 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.basic/files/space.sh
+-rw-rw-r--  2.0 unx     4154 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.basic/tasks/check.yml
+-rw-rw-r--  2.0 unx      702 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.basic/tasks/get_k8s_version.yml
+-rw-rw-r--  2.0 unx     2170 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml
+-rw-rw-r--  2.0 unx     4723 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml
+-rw-rw-r--  2.0 unx     4892 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_status_check.yml
+-rw-rw-r--  2.0 unx    12487 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.check/defaults/compatibility_map.yml
+-rw-rw-r--  2.0 unx      335 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.check/tasks/compatibility_check.yml
+-rw-rw-r--  2.0 unx       76 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/README.md
+-rw-rw-r--  2.0 unx     1296 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/defaults/main.yml
+-rw-rw-r--  2.0 unx      181 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/meta/main.yml
+-rw-rw-r--  2.0 unx     3822 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/ascend-operator.yaml
+-rw-rw-r--  2.0 unx    10933 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml
+-rw-rw-r--  2.0 unx      675 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/create_user.yaml
+-rw-rw-r--  2.0 unx    12772 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/deviceplugin.yaml
+-rw-rw-r--  2.0 unx     7220 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/distribute_soft_package.yaml
+-rw-rw-r--  2.0 unx      484 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/dl_common.yaml
+-rw-rw-r--  2.0 unx     1517 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/docker-runtime.yaml
+-rw-rw-r--  2.0 unx     5612 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/hccl.yaml
+-rw-rw-r--  2.0 unx     5867 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/noded.yaml
+-rw-rw-r--  2.0 unx     5511 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/npu-exporter.yaml
+-rw-rw-r--  2.0 unx     4347 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/push_image.yaml
+-rw-rw-r--  2.0 unx     4105 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/resilience-controller.yaml
+-rw-rw-r--  2.0 unx     8879 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml
+-rw-rw-r--  2.0 unx       67 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.docker/README.md
+-rw-rw-r--  2.0 unx      171 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.docker/meta/main.yml
+-rw-rw-r--  2.0 unx      500 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.docker/tasks/copy.yml
+-rw-rw-r--  2.0 unx      418 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml
+-rw-rw-r--  2.0 unx      446 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.docker/tasks/install_containerd.yml
+-rw-rw-r--  2.0 unx     1135 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.docker/tasks/post_install.yml
+-rw-rw-r--  2.0 unx       55 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.docker/tests/ansible.cfg
+-rw-rw-r--  2.0 unx       37 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.docker/tests/inventory
+-rw-rw-r--  2.0 unx      116 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.docker/tests/test.yml
+-rw-rw-r--  2.0 unx       99 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.docker/vars/main.yml
+-rw-rw-r--  2.0 unx     1314 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.harbor/tasks/check.yml
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.harbor/tasks/http.yml
+-rw-rw-r--  2.0 unx      346 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.harbor/tasks/https.yml
+-rw-rw-r--  2.0 unx     1157 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.harbor/tasks/main.yml
+-rw-rw-r--  2.0 unx       42 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.harbor/vars/main.yml
+-rw-rw-r--  2.0 unx     1723 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.hccn/tasks/hccn_conf.yaml
+-rw-rw-r--  2.0 unx      660 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.image/tasks/image_load.yaml
+-rw-rw-r--  2.0 unx      536 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/README.md
+-rw-rw-r--  2.0 unx      234 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/defaults/main.yml
+-rw-rw-r--  2.0 unx      929 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/files/10-kubeadm.conf
+-rw-rw-r--  2.0 unx      283 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/files/kubelet.service
+-rw-rw-r--  2.0 unx      179 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/meta/main.yml
+-rw-rw-r--  2.0 unx      691 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/containerd.yml
+-rw-rw-r--  2.0 unx     1321 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml
+-rw-rw-r--  2.0 unx      774 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml
+-rw-rw-r--  2.0 unx     1235 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml
+-rw-rw-r--  2.0 unx      897 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/os_setting.yml
+-rw-rw-r--  2.0 unx     4727 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/push_image.yml
+-rw-rw-r--  2.0 unx     1805 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tasks/kubevip/main.yml
+-rw-rw-r--  2.0 unx     3557 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master/main.yml
+-rw-rw-r--  2.0 unx     1596 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master_backup/main.yml
+-rw-rw-r--  2.0 unx      860 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tasks/worker/main.yml
+-rw-rw-r--  2.0 unx   202740 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.20.2.yaml
+-rw-rw-r--  2.0 unx       55 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tests/ansible.cfg
+-rw-rw-r--  2.0 unx       37 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tests/inventory
+-rw-rw-r--  2.0 unx      116 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/tests/test.yml
+-rw-rw-r--  2.0 unx      485 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.k8s/vars/main.yml
+-rw-rw-r--  2.0 unx       78 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.kubeedge/README.md
+-rw-rw-r--  2.0 unx      243 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.kubeedge/defaults/main.yml
+-rw-rw-r--  2.0 unx      162 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cloudcore.service
+-rw-rw-r--  2.0 unx     1896 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cluster_objectsync_v1alpha1.yaml
+-rw-rw-r--  2.0 unx     8715 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_device.yaml
+-rw-rw-r--  2.0 unx    10576 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_devicemodel.yaml
+-rw-rw-r--  2.0 unx     1877 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.kubeedge/files/objectsync_v1alpha1.yaml
+-rw-rw-r--  2.0 unx     2443 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_rule.yaml
+-rw-rw-r--  2.0 unx     1355 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_ruleEndpoint.yaml
+-rw-rw-r--  2.0 unx      176 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.kubeedge/meta/main.yml
+-rw-rw-r--  2.0 unx     4625 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml
+-rw-rw-r--  2.0 unx      144 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.rep/defaults/main.yml
+-rw-rw-r--  2.0 unx      528 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.rep/tasks/get_npu_info.py
+-rw-rw-r--  2.0 unx     2089 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.rep/tasks/hccn_rep.yaml
+-rw-rw-r--  2.0 unx     2856 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py
+-rw-rw-r--  2.0 unx     8254 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py
+-rw-rw-r--  2.0 unx     1218 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.rep/tasks/local_rep.yaml
+-rw-rw-r--  2.0 unx     1011 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.rep/tasks/ls_format.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.rep/tasks/output_json.py
+-rw-rw-r--  2.0 unx     1942 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.rep/tasks/packages_rep.yaml
+-rw-rw-r--  2.0 unx      389 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_k8s_docker.yaml
+-rw-rw-r--  2.0 unx      390 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_mef_kubeedge.yaml
+-rw-rw-r--  2.0 unx      960 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_auto.yml
+-rw-rw-r--  2.0 unx      613 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_dl.yml
+-rw-rw-r--  2.0 unx      259 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_edge.yml
+-rw-rw-r--  2.0 unx      357 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_mef.yml
+-rw-rw-r--  2.0 unx      514 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_mindspore.yml
+-rw-rw-r--  2.0 unx      435 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_offline_dev.yml
+-rw-rw-r--  2.0 unx      354 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_offline_run.yml
+-rw-rw-r--  2.0 unx      510 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_pytorch_dev.yml
+-rw-rw-r--  2.0 unx      504 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_pytorch_run.yml
+-rw-rw-r--  2.0 unx      593 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_tensorflow_dev.yml
+-rw-rw-r--  2.0 unx      587 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_tensorflow_run.yml
+-rw-rw-r--  2.0 unx      273 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/scene/scene_vmhost.yml
+-rw-rw-r--  2.0 unx     2642 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/case_driver.yml
+-rw-rw-r--  2.0 unx     1127 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/case_firmware.yml
+-rw-rw-r--  2.0 unx     3166 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/case_mindspore.yml
+-rw-rw-r--  2.0 unx      753 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/case_nnae.yml
+-rw-rw-r--  2.0 unx      751 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/case_nnrt.yml
+-rw-rw-r--  2.0 unx     3619 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/case_pytorch.yml
+-rw-rw-r--  2.0 unx     7715 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/case_tensorflow.yml
+-rw-rw-r--  2.0 unx     1766 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/case_tfplugin.yml
+-rw-rw-r--  2.0 unx     1473 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/case_toolbox.yml
+-rw-rw-r--  2.0 unx      788 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/case_toolkit.yml
+-rw-rw-r--  2.0 unx      608 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_all.yml
+-rw-rw-r--  2.0 unx      284 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_driver.yml
+-rw-rw-r--  2.0 unx      114 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_exhibit.yml
+-rw-rw-r--  2.0 unx      284 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_firmware.yml
+-rw-rw-r--  2.0 unx       99 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_mindspore.yml
+-rw-rw-r--  2.0 unx       90 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_nnae.yml
+-rw-rw-r--  2.0 unx       89 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_nnrt.yml
+-rw-rw-r--  2.0 unx       96 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_pytorch.yml
+-rw-rw-r--  2.0 unx      101 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_tensorflow.yml
+-rw-rw-r--  2.0 unx       97 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_tfplugin.yml
+-rw-rw-r--  2.0 unx      104 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_toolbox.yml
+-rw-rw-r--  2.0 unx       95 b- defN 23-Jun-30 09:36 ascend_deployer/playbooks/test/test_toolkit.yml
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/__init__.py
+-rw-rw-r--  2.0 unx    20831 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/check_pkgs.sh
+-rw-rw-r--  2.0 unx     1116 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/hccn_set.sh
+-rw-rw-r--  2.0 unx     1142 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/image_load.sh
+-rw-rw-r--  2.0 unx      969 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/install.sh
+-rw-rw-r--  2.0 unx     3587 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/install_ansible.sh
+-rw-rw-r--  2.0 unx    14663 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/nexus.py
+-rw-rw-r--  2.0 unx     1219 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/nexus_config.json
+-rw-rw-r--  2.0 unx    15176 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/prepare.sh
+-rw-rw-r--  2.0 unx      535 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/uninstall_k8s_docker.sh
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/uninstall_mef_kubeedge.sh
+-rw-rw-r--  2.0 unx      679 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/uninstall_mef_related.sh
+-rw-rw-r--  2.0 unx     5723 b- defN 23-Jun-30 09:36 ascend_deployer/scripts/utils.sh
+-rw-rw-r--  2.0 unx    10900 b- defN 23-Jun-30 09:36 ascend_deployer/tools/DeviceIP-conf.sh
+-rw-rw-r--  2.0 unx     1409 b- defN 23-Jun-30 09:36 ascend_deployer/tools/ascend-deployer
+-rw-rw-r--  2.0 unx     4049 b- defN 23-Jun-30 09:36 ascend_deployer/tools/check.py
+-rw-rw-r--  2.0 unx     7684 b- defN 23-Jun-30 09:36 ascend_deployer/tools/hccn.py
+-rw-rw-r--  2.0 unx     9930 b- defN 23-Jun-30 09:36 ascend_deployer/tools/update_crl.sh
+-rw-rw-r--  2.0 unx       21 b- defN 23-Jun-30 09:36 ascend_deployer/tools/hccn/main/go.mod
+-rw-rw-r--  2.0 unx     6863 b- defN 23-Jun-30 09:36 ascend_deployer/tools/hccn/main/hccn.go
+-rw-rw-r--  2.0 unx     4260 b- defN 23-Jun-30 09:36 ascend_deployer/tools/nexus/Dockerfile
+-rw-rw-r--  2.0 unx      142 b- defN 23-Jun-30 09:36 ascend_deployer/tools/report/main/go.mod
+-rw-rw-r--  2.0 unx    18729 b- defN 23-Jun-30 09:36 ascend_deployer/tools/report/main/main.go
+-rw-rw-r--  2.0 unx       21 b- defN 23-Jun-30 09:36 ascend_deployer/tools/unzip/main/go.mod
+-rw-rw-r--  2.0 unx     1587 b- defN 23-Jun-30 09:36 ascend_deployer/tools/unzip/main/unzip.go
+-rw-rw-r--  2.0 unx       46 b- defN 23-Jun-30 09:36 ascend_deployer/yamls/basic.yaml
+-rw-rw-r--  2.0 unx       46 b- defN 23-Jun-30 09:36 ascend_deployer/yamls/check.yaml
+-rw-rw-r--  2.0 unx      132 b- defN 23-Jun-30 09:36 ascend_deployer/yamls/docker.yaml
+-rw-rw-r--  2.0 unx       53 b- defN 23-Jun-30 09:36 ascend_deployer/yamls/gather_facts.yaml
+-rw-rw-r--  2.0 unx       72 b- defN 23-Jun-30 09:36 ascend_deployer/yamls/harbor.yaml
+-rw-rw-r--  2.0 unx       45 b- defN 23-Jun-30 09:36 ascend_deployer/yamls/hccn.yaml
+-rw-rw-r--  2.0 unx       51 b- defN 23-Jun-30 09:36 ascend_deployer/yamls/image_load.yaml
+-rw-rw-r--  2.0 unx      126 b- defN 23-Jun-30 09:36 ascend_deployer/yamls/k8s.yaml
+-rw-rw-r--  2.0 unx      234 b- defN 23-Jun-30 09:36 ascend_deployer/yamls/k8s_reset.yaml
+-rw-rw-r--  2.0 unx       74 b- defN 23-Jun-30 09:36 ascend_deployer/yamls/mindxdl.yaml
+-rw-rw-r--  2.0 unx       47 b- defN 23-Jun-30 09:36 ascend_deployer/yamls/report.yaml
+-rwxr-xr-x  2.0 unx     1409 b- defN 23-Jul-03 09:38 ascend_deployer-5.0.0b9.data/scripts/ascend-deployer
+-rw-------  2.0 unx     2739 b- defN 23-Jul-03 09:38 ascend_deployer-5.0.0b9.dist-info/DESCRIPTION.rst
+-rw-------  2.0 unx       74 b- defN 23-Jul-03 09:38 ascend_deployer-5.0.0b9.dist-info/entry_points.txt
+-rw-------  2.0 unx      777 b- defN 23-Jul-03 09:38 ascend_deployer-5.0.0b9.dist-info/metadata.json
+-rw-------  2.0 unx       16 b- defN 23-Jul-03 09:38 ascend_deployer-5.0.0b9.dist-info/top_level.txt
+-rw-------  2.0 unx       92 b- defN 23-Jul-03 09:38 ascend_deployer-5.0.0b9.dist-info/WHEEL
+-rw-------  2.0 unx     3183 b- defN 23-Jul-03 09:38 ascend_deployer-5.0.0b9.dist-info/METADATA
+-rw-------  2.0 unx    45304 b- defN 23-Jul-03 09:38 ascend_deployer-5.0.0b9.dist-info/RECORD
+402 files, 1944504 bytes uncompressed, 394508 bytes compressed:  79.7%
```

## zipnote {}

```diff
@@ -465,39 +465,42 @@
 
 Filename: ascend_deployer/playbooks/facts/app_info.fact.j2
 Comment: 
 
 Filename: ascend_deployer/playbooks/facts/npu_info.fact.j2
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/install_atlasedge.yml
+Filename: ascend_deployer/playbooks/install/install_ascend-device-plugin.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/install_device_plugin.yml
+Filename: ascend_deployer/playbooks/install/install_ascend-docker-runtime.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/install_docker_images.yml
+Filename: ascend_deployer/playbooks/install/install_ascend-operator.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/install_docker_runtime.yml
+Filename: ascend_deployer/playbooks/install/install_atlasedge.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/install/install_docker_images.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_driver.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_firmware.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_gcc.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_ha.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/install_hccl.yml
+Filename: ascend_deployer/playbooks/install/install_hccl-controller.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_ief.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_kernels.yml
 Comment: 
@@ -513,26 +516,29 @@
 
 Filename: ascend_deployer/playbooks/install/install_nnrt.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_noded.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/install_npu.yml
+Filename: ascend_deployer/playbooks/install/install_npu-exporter.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/install_npu_exporter.yml
+Filename: ascend_deployer/playbooks/install/install_npu.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_python.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_pytorch.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/install/install_resilience-controller.yml
+Comment: 
+
 Filename: ascend_deployer/playbooks/install/install_sys_pkg.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_tensorflow.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_tfplugin.yml
@@ -711,14 +717,17 @@
 
 Filename: ascend_deployer/playbooks/roles/mindx.basic/files/space.sh
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/check.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/get_k8s_version.yml
+Comment: 
+
 Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_status_check.yml
@@ -735,14 +744,17 @@
 
 Filename: ascend_deployer/playbooks/roles/mindx.dl/defaults/main.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.dl/meta/main.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/ascend-operator.yaml
+Comment: 
+
 Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/create_user.yaml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/deviceplugin.yaml
@@ -765,14 +777,17 @@
 
 Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/npu-exporter.yaml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/push_image.yaml
 Comment: 
 
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/resilience-controller.yaml
+Comment: 
+
 Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.docker/README.md
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.docker/meta/main.yml
@@ -780,14 +795,17 @@
 
 Filename: ascend_deployer/playbooks/roles/mindx.docker/tasks/copy.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/roles/mindx.docker/tasks/install_containerd.yml
+Comment: 
+
 Filename: ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.docker/tasks/post_install.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.docker/tests/ansible.cfg
@@ -843,17 +861,14 @@
 
 Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/get_k8s_version.yml
-Comment: 
-
 Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/os_setting.yml
@@ -891,17 +906,14 @@
 
 Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/README.md
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/defaults/main.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/certgen.sh
-Comment: 
-
 Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/cloudcore.service
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/cluster_objectsync_v1alpha1.yaml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_device.yaml
@@ -1026,14 +1038,17 @@
 
 Filename: ascend_deployer/playbooks/test/test_all.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/test/test_driver.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/test/test_exhibit.yml
+Comment: 
+
 Filename: ascend_deployer/playbooks/test/test_firmware.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/test/test_mindspore.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/test/test_nnae.yml
@@ -1113,14 +1128,17 @@
 
 Filename: ascend_deployer/tools/hccn/main/go.mod
 Comment: 
 
 Filename: ascend_deployer/tools/hccn/main/hccn.go
 Comment: 
 
+Filename: ascend_deployer/tools/nexus/Dockerfile
+Comment: 
+
 Filename: ascend_deployer/tools/report/main/go.mod
 Comment: 
 
 Filename: ascend_deployer/tools/report/main/main.go
 Comment: 
 
 Filename: ascend_deployer/tools/unzip/main/go.mod
@@ -1158,32 +1176,32 @@
 
 Filename: ascend_deployer/yamls/mindxdl.yaml
 Comment: 
 
 Filename: ascend_deployer/yamls/report.yaml
 Comment: 
 
-Filename: ascend_deployer-5.0.0b8.data/scripts/ascend-deployer
+Filename: ascend_deployer-5.0.0b9.data/scripts/ascend-deployer
 Comment: 
 
-Filename: ascend_deployer-5.0.0b8.dist-info/DESCRIPTION.rst
+Filename: ascend_deployer-5.0.0b9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: ascend_deployer-5.0.0b8.dist-info/entry_points.txt
+Filename: ascend_deployer-5.0.0b9.dist-info/entry_points.txt
 Comment: 
 
-Filename: ascend_deployer-5.0.0b8.dist-info/metadata.json
+Filename: ascend_deployer-5.0.0b9.dist-info/metadata.json
 Comment: 
 
-Filename: ascend_deployer-5.0.0b8.dist-info/top_level.txt
+Filename: ascend_deployer-5.0.0b9.dist-info/top_level.txt
 Comment: 
 
-Filename: ascend_deployer-5.0.0b8.dist-info/WHEEL
+Filename: ascend_deployer-5.0.0b9.dist-info/WHEEL
 Comment: 
 
-Filename: ascend_deployer-5.0.0b8.dist-info/METADATA
+Filename: ascend_deployer-5.0.0b9.dist-info/METADATA
 Comment: 
 
-Filename: ascend_deployer-5.0.0b8.dist-info/RECORD
+Filename: ascend_deployer-5.0.0b9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ascend_deployer/ansible.cfg

```diff
@@ -1,13 +1,14 @@
 [defaults]
 forks=50
 command_warnings=False
 host_key_checking=False
 callback_plugins   = ./ansible_plugin
 bin_ansible_callbacks=True
+log_path=./install.log
 
 gathering=explicit
 fact_caching=jsonfile
 deprecation_warnings=False
 interpreter_python=auto_legacy_silent
 fact_caching_connection=./facts-cache
```

## ascend_deployer/ascend_deployer.py

```diff
@@ -41,15 +41,18 @@
                 LOG.info("[INFO] Ascend DL deployed success --ascend-deployer")
             return result
         except SystemExit as e:
             if e.code == 0:
                 return 0
             reason = 'exit code: {}'.format(e.code)
             return -1
-        except BaseException as e:  # handle KeyboardInterrupt and other exceptions
+        except KeyboardInterrupt:  # handle KeyboardInterrupt
+            reason = "User interrupted the program by Keyboard"
+            return -1
+        except BaseException as e:  # handle other exceptions
             reason = str(e)
             return -1
         finally:
             msg = "run cmd: {} successfully".format(cmd)
             if reason:
                 msg = "run cmd: {} failed, reason: {}".format(cmd, reason)
             print(msg)
```

## ascend_deployer/install.sh

```diff
@@ -1,51 +1,15 @@
 #!/bin/bash
-unset LD_LIBRARY_PATH
-declare -x PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:"${ASCENDPATH}""
-readonly LOG_SIZE_THRESHOLD=$((20 * 1024 * 1024))
-readonly LOG_COUNT_THRESHOLD=5
 readonly BASE_DIR=$(
     cd "$(dirname $0)" >/dev/null 2>&1
     pwd -P
 )
 
-export ANSIBLE_CONFIG=$BASE_DIR/ansible.cfg
-export ANSIBLE_LOG_PATH=$BASE_DIR/install.log
 export ANSIBLE_CACHE_PLUGIN_CONNECTION=$BASE_DIR/facts_cache
 
-function log_info() {
-    local DATE_N=$(date "+%Y-%m-%d %H:%M:%S")
-    local USER_N=$(whoami)
-    local IP_N=$(who am i | awk '{print $NF}' | sed 's/[()]//g')
-    echo "[INFO] $*"
-    echo "${DATE_N} ${USER_N}@${IP_N} [INFO] $*" >>${BASE_DIR}/install.log
-}
-
-function log_warning() {
-    local DATE_N=$(date "+%Y-%m-%d %H:%M:%S")
-    local USER_N=$(whoami)
-    local IP_N=$(who am i | awk '{print $NF}' | sed 's/[()]//g')
-    echo "[WARNING] $*"
-    echo "${DATE_N} ${USER_N}@${IP_N} [WARNING] $*" >>${BASE_DIR}/install.log
-}
-
-function log_error() {
-    local DATE_N=$(date "+%Y-%m-%d %H:%M:%S")
-    local USER_N=$(whoami)
-    local IP_N=$(who am i | awk '{print $NF}' | sed 's/[()]//g')
-    echo "[ERROR] $*"
-    echo "${DATE_N} ${USER_N}@${IP_N} [ERROR] $*" >>${BASE_DIR}/install.log
-}
-
-function operation_log_info() {
-    local DATE_N=$(date "+%Y-%m-%d %H:%M:%S")
-    local USER_N=$(whoami)
-    local IP_N=$(who am i | awk '{print $NF}' | sed 's/[()]//g')
-    echo "${DATE_N} ${USER_N}@${IP_N} [INFO] $*" >>${BASE_DIR}/install_operation.log
-}
 
 function get_specified_python() {
     if [ ! -z ${ASCEND_PYTHON_VERSION} ]; then
         echo ${ASCEND_PYTHON_VERSION}
     else
         echo $(grep -oP "^ascend_python_version=\K.*" ${BASE_DIR}/downloader/config.ini | sed 's/\r$//')
     fi
@@ -53,70 +17,20 @@
 
 readonly specified_python=$(get_specified_python)
 readonly PYTHON_VERSION=$(echo ${specified_python} | sed 's/P/p/;s/-//')
 readonly PYTHON_PREFIX=${HOME}/.local/${PYTHON_VERSION}
 export PATH=${PYTHON_PREFIX}/bin:$PATH
 export LD_LIBRARY_PATH=${PYTHON_PREFIX}/lib:$LD_LIBRARY_PATH
 
-function rotate_log() {
-    local log_list=$(ls $1* | sort -r)
-    for item in $log_list; do
-        local suffix=${item##*.}
-        local prefix=${item%.*}
-        if [[ ${suffix} != "log" ]]; then
-            if [[ ${suffix} -lt ${LOG_COUNT_THRESHOLD} ]]; then
-                suffix=$(($suffix + 1))
-                mv -f $item $prefix.$suffix
-            fi
-        else
-            mv -f ${item} ${item}.1
-            cat /dev/null >${item}
-        fi
-    done
-}
-
-function check_log() {
-    if [[ ! -e $1 ]]; then
-        touch $1
-    fi
-    local log_size=$(ls -l $1 | awk '{ print $5 }')
-    if [[ ${log_size} -ge ${LOG_SIZE_THRESHOLD} ]]; then
-        rotate_log $1
-    fi
-}
-
-function set_permission() {
-    chmod -R 750 $(find ${BASE_DIR}/ -type d ! -path "${BASE_DIR}/.git*" ! -path "${BASE_DIR}/resources/run_from_*_zip/*") 2>/dev/null
-    chmod -R 640 $(find ${BASE_DIR}/ -type f ! -path "${BASE_DIR}/.git*" ! -path "${BASE_DIR}/resources/run_from_*_zip/*") 2>/dev/null
-    for f in $(find ${BASE_DIR}/ -maxdepth 2 -type f -name "*.sh" -o -name "*.py" ! -path "${BASE_DIR}/.git*" ! -path "${BASE_DIR}/resources/run_from_*_zip/*"); do
-        is_exe=$(file ${f} | grep executable | wc -l)
-        if [[ ${is_exe} -eq 1 ]]; then
-            chmod 550 ${f} 2>/dev/null
-        fi
-    done
-    chmod 750 $BASE_DIR/ $BASE_DIR/playbooks/install
-    chmod 600 ${BASE_DIR}/*.log ${BASE_DIR}/tools/*.log ${BASE_DIR}/inventory_file $BASE_DIR/ansible.cfg ${BASE_DIR}/downloader/config.ini 2>/dev/null
-    chmod 400 ${BASE_DIR}/*.log.? ${BASE_DIR}/tools/*.log.? 2>/dev/null
-}
 
 main() {
-    local os_name=$(grep -oP "^ID=\"?\K\w+" /etc/os-release)
-    check_log ${BASE_DIR}/install.log
-    check_log ${BASE_DIR}/install_operation.log
-    set_permission
-
     python3 -V > /dev/null 2>&1
     if [[ $? != 0 ]]; then
       python ${BASE_DIR}/ascend_deployer.py $*
     else
       python3 ${BASE_DIR}/ascend_deployer.py $*
     fi
 }
 
 main $*
 main_status=$?
-if [[ ${main_status} != 0 ]] && [[ ${main_status} != 6 ]]; then
-    operation_log_info "parameter error,run failed"
-else
-    operation_log_info "$0 $*:Success"
-fi
 exit ${main_status}
```

## ascend_deployer/jobs.py

```diff
@@ -13,14 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 import os
 import sys
 from subprocess import PIPE, Popen, CalledProcessError, STDOUT
+import configparser
 
 import utils
 
 CURSOR_UPWARD = u'\u001b[1A'
 MAX_LEN = 80
 
 
@@ -34,27 +35,26 @@
             cmd = popenargs[0]
         raise CalledProcessError(ret_code, cmd)
     return 0
 
 
 def prepare_install():
     prepare_sh = os.path.join(utils.ROOT_PATH, 'scripts', 'prepare.sh')
-    process = Popen([prepare_sh], shell=False, env=os.environ, stderr=STDOUT, stdout=PIPE)
+    process = Popen(["bash", prepare_sh], shell=False, env=os.environ, stderr=STDOUT, stdout=PIPE)
 
+    sys.stdout.write("\n")  # prevents the first line from being overwritten
     for line in iter(process.stdout.readline, b''):
         line = line.decode('utf-8').strip()
         if len(line) <= MAX_LEN:
             line += (MAX_LEN - len(line)) * " "
         else:
             # if the line too long(> MAX_LEN), only print first (MAX_LEN -3) characters and '...'
             line = line[0:MAX_LEN - 4] + "..."
-        sys.stdout.write("\r" + line + "\n")
         sys.stdout.write(CURSOR_UPWARD)
-        sys.stdout.flush()
-    sys.stdout.write("\n")  # prevents the last line from being overwritten
+        sys.stdout.write("\r" + line + "\n")
 
     process.wait()
     ret_code = process.returncode
     if ret_code:
         raise CalledProcessError(ret_code, ["ascend_deployer/scripts/prepare.sh"])
     return 0
 
@@ -65,15 +65,20 @@
 
     @staticmethod
     def get_inventory_file():
         return os.path.join(utils.ROOT_PATH, 'inventory_file')
 
     @staticmethod
     def handle_python_env(args):
-        ascend_python_version = os.environ.get("ASCEND_PYTHON_VERSION", "Python-3.7.5")
+        ascend_python_version = os.environ.get("ASCEND_PYTHON_VERSION")
+        if not ascend_python_version:
+            config_file = os.path.join(utils.ROOT_PATH, 'downloader', 'config.ini')
+            cfp = configparser.ConfigParser()
+            cfp.read(config_file, encoding='utf-8')
+            ascend_python_version = cfp.get('python', 'ascend_python_version')
         version_list = utils.get_python_version_list()
         if ascend_python_version not in version_list:
             raise Exception("ASCEND_PYTHON_VERSION is not available, "
                             "available python version list is {}".format(version_list))
         version = ascend_python_version.replace('P', 'p').replace('-', '')
         args.extend([
             '-e', 'python_tar={}'.format(ascend_python_version),
```

## ascend_deployer/ansible_plugin/ansible_log.py

```diff
@@ -70,14 +70,18 @@
                 for task in cur_tasks:
                     next_tasks = task.get("import_tasks") or task.get("include_tasks")
                     if next_tasks:
                         ret += get_tasks_amount(os.path.join(dir_name, next_tasks))
     return ret
 
 
+class AnsibleFormatException(Exception):
+    pass
+
+
 class CallbackModule(default):
     CALLBACK_VERSION = 2.0
     CALLBACK_TYPE = 'stdout'
     CALLBACK_NAME = 'ansible_log'
 
     def __init__(self):
 
@@ -98,22 +102,29 @@
 
         with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), 'install_info.yaml'), 'r') as f:
             self._install_info = yaml.safe_load(f)
 
     @staticmethod
     def _parse_msg(_msg):
         if isinstance(_msg, list):
+            CallbackModule._check_msg_list(_msg)
             msg = ';'.join(_msg)
         elif isinstance(_msg, str):
             msg = _msg
         else:
             msg = ''
         msg = msg.split("=>")[0]
         return msg if msg.startswith('[ASCEND]') else ''
 
+    @staticmethod
+    def _check_msg_list(msg_list):
+        for str_item in msg_list:
+            if not isinstance(str_item, str):
+                raise AnsibleFormatException()
+
     def set_options(self, task_keys=None, var_options=None, direct=None):
 
         super(CallbackModule, self).set_options(task_keys=task_keys, var_options=var_options, direct=direct)
 
         for option, constant in COMPAT_OPTIONS:
             try:
                 value = self.get_option(option)
@@ -129,20 +140,22 @@
 
     def v2_runner_on_failed(self, result, ignore_errors=False):
         super(CallbackModule, self).v2_runner_on_unreachable(result)
         show_reason = 'please check log at {HOME}/.log/'
         for record in result._result.get('results', []):
             if not record.get('failed'):
                 continue
-            reason_msg = self._parse_msg(record.get('msg'))
+            reason_msg = self._try_parse_msg(record.get('msg'))
             if reason_msg:
                 show_reason = reason_msg
                 break
         else:
-            reason_msg = self._parse_msg(getattr(result, '_result').get('msg', ''))
+            reason_msg = ''
+            if hasattr(result, '_result'):
+                reason_msg = self._try_parse_msg(getattr(result, '_result').get('msg', ''))
             if reason_msg:
                 show_reason = reason_msg
 
         if not ignore_errors:
             self._fatal_flag = True
             self._extra_msg.append("{:<50}".format("[%s]: FAILED! %s" % (
                 result._host.get_name(), show_reason)))
@@ -159,15 +172,15 @@
 
     def v2_runner_on_start(self, host, task):
         self._display.display(" [started %s on %s]" % (task, host), color=C.COLOR_OK)
 
     def v2_runner_on_ok(self, result):
         super(CallbackModule, self).v2_runner_on_ok(result)
         msg = result._result.get('msg')
-        msg = self._parse_msg(msg)
+        msg = self._try_parse_msg(msg)
         if msg:
             host_label = result._host.get_name()
             extra = "{:<50}".format("%s => %s " % (msg.replace("[ASCEND]", ""), host_label))
             self._extra_msg.append(extra)
 
     def v2_playbook_on_stats(self, stats):
         hosts = sorted(stats.processed.keys())
@@ -234,25 +247,33 @@
         if self._playbook_name is None:
             return
 
         msg = self.search_common_msg(self._playbook_name) or self.search_common_msg(file_name)
         if not msg:
             msg = self.ordinary_msg_scene(file_name)
         title_bar = "{:<50}".format(msg)
-        action = "=" * (int(min(1, self._task_process / self._task_amount) * 49)) + ">"
+        action = "=" * (int(min(1, self._task_process / self._task_amount) * 50))
+        if self._task_process == self._task_amount:
+            action += "="
+        else:
+            action += ">"
         task_bar = "task info:{:<80}".format(self._last_task_name)
         process_bar = "[{:-<51}]".format(action)
         bar_list = [title_bar, task_bar, process_bar]
         bar_list.extend(self._extra_msg)
         if self._task_process != 0:
             for i in range(0, self._lines_num):
                 sys.stdout.write(CURSOR_UPWARD)
         screen_prints = "\r" + "\n".join(bar_list) + "\n"
         sys.stdout.write(screen_prints)
-        self._lines_num = screen_prints.count("\n")
+        screen_size = os.get_terminal_size()[0]
+        backward = 0
+        for bar in bar_list:
+            backward += len(bar) // screen_size
+        self._lines_num = screen_prints.count("\n") + backward
 
     def confirm_playbook_name(self, path):
         if "mindx" in path:
             start_index = path.find('/mindx.') + len('/mindx.')
             end_index = path.find('/', start_index)
             self._playbook_name = path[start_index:end_index]
 
@@ -285,15 +306,23 @@
         if C.ACTION_WARNINGS:
             if 'deprecations' in res and res['deprecations']:
                 for warning in res['deprecations']:
                     self._display.display(**warning)
                 del res['deprecations']
             else:
                 super(CallbackModule, self)._handle_warnings(res)
-                
+
+    def _try_parse_msg(self, item):
+        try:
+            return self._parse_msg(item)
+        except AnsibleFormatException:
+            debug_msg = "{:<50}".format("bad grammar at %s" % self._last_task_name)
+            self._extra_msg.append(debug_msg)
+            return ''
+
 
 class LogDisplay(Display):
     def __init__(self):
         super(LogDisplay, self).__init__()
 
     def display(self, msg, color=None, stderr=False, screen_only=False, log_only=False, newline=True):
         fatal_line = msg.startswith(u'fatal')
```

## ascend_deployer/downloader/deb_downloader.py

```diff
@@ -39,28 +39,28 @@
     source
     """
 
     def __init__(self, line):
         tmp = line.split(' ')
         self.url = tmp[1].strip()
         self.distro = tmp[2].strip()
-        self.repoList = [i.strip() for i in tmp[3:]]
+        self.repo_list = [i.strip() for i in tmp[3:]]
 
     def get_url(self):
         """
         get source url
         """
         return self.url
 
     def repos(self):
         """
         get source repos
         """
         repos = {}
-        for repo in self.repoList:
+        for repo in self.repo_list:
             repo_url = "{0}dists/{1}/{2}".format(self.url, self.distro, repo)
             yield repo, repo_url
 
 
 class Package(object):
     """
     Package
@@ -93,60 +93,27 @@
 class Apt(object):
     """
     downloader for apt
     """
 
     def __init__(self, source_file, arch):
         self.arch = arch
-        self.binary_path = 'binary-amd64' \
-            if 'x86' in self.arch else 'binary-arm64'
+        self.binary_path = 'binary-amd64' if 'x86' in self.arch else 'binary-arm64'
         # 读取源配置
         self.source_list = []
         self.base_dir = get_download_path()
         self.repo_file = os.path.join(self.base_dir, source_file)
         self.resources_dir = os.path.join(self.base_dir, 'resources')
         self.primary_connection = sqlite.Connection(':memory:')
         self.primary_cur = self.primary_connection.cursor()
         with open(self.repo_file) as file:
             for line in file.readlines():
                 source = DebianSource(line)
                 self.source_list.append(source)
 
-    def make_cache(self):
-        """
-        make_cache
-        """
-        try:
-            self.primary_cur.executescript("CREATE TABLE packages \
-                    (name TEXT, version TEXT, source TEXT, repo TEXT, \
-                    url TEXT, sha256 TEXT);")
-        except sqlite.OperationalError as e:
-            pass
-        finally:
-            pass
-
-        for source in self.source_list:
-            for repo, url in source.repos():
-                index_url = '{0}/{1}/Packages.gz'.format(url, self.binary_path)
-                LOG.info('packages_url=[%s]', index_url)
-                packages = self.fetch_package_index(index_url)
-                if packages is False:
-                    print(index_url.ljust(60), 'download failed')
-                    LOG.error('download %s failed', index_url)
-                    return False
-                self.make_cache_from_packages(source.get_url(), repo, packages)
-        self.primary_connection.commit()
-        self.primary_cur.close()
-
-    def clean_cache(self):
-        """
-        clean sqlite Connection
-        """
-        self.primary_connection.close()
-
     @staticmethod
     def fetch_package_index(packages_url):
         """
         fetch_package_index
 
         :param packages_url:
         :return:
@@ -184,14 +151,70 @@
                 pass
             if ver_a_list[i] == ver_b_list[i]:
                 continue
             else:
                 return ver_a_list[i] > ver_b_list[i]
         return len(ver_a) > len(ver_b)
 
+    @staticmethod
+    def need_download_again(target_sha256, dst_file):
+        """
+        need_download_again
+
+        :param name:
+        :param dst_dir:
+        :return:
+        """
+        if target_sha256 is None:
+            return True
+        if not os.path.exists(dst_file):
+            return True
+        file_sha256 = calc_sha256(dst_file)
+        if target_sha256 != file_sha256:
+            LOG.info('target sha256 : %s, existed file sha256 : %s',
+                     target_sha256, file_sha256)
+            print('target sha256 : {}, existed file sha256 : {}'.format(
+                target_sha256, file_sha256))
+            return True
+        else:
+            return False
+
+    def make_cache(self):
+        """
+        make_cache
+        """
+        try:
+            self.primary_cur.executescript("CREATE TABLE packages \
+                    (name TEXT, version TEXT, source TEXT, repo TEXT, \
+                    url TEXT, sha256 TEXT);")
+        except sqlite.OperationalError as e:
+            pass
+        finally:
+            pass
+
+        for source in self.source_list:
+            for repo, url in source.repos():
+                index_url = '{0}/{1}/Packages.gz'.format(url, self.binary_path)
+                LOG.info('packages_url=[%s]', index_url)
+                packages = self.fetch_package_index(index_url)
+                if packages is False:
+                    print(index_url.ljust(60), 'download failed')
+                    LOG.error('download %s failed', index_url)
+                    return False
+                self.make_cache_from_packages(source.get_url(), repo, packages)
+        self.primary_connection.commit()
+        self.primary_cur.close()
+        return True
+
+    def clean_cache(self):
+        """
+        clean sqlite Connection
+        """
+        self.primary_connection.close()
+
     def make_cache_from_packages(self, source_url, repo, packages_content):
         """
         make_cache_from_packages
 
         :param packages_content:
         :return:
         """
@@ -321,30 +344,7 @@
         """
         download
         """
         if 'url' in pkg:
             return self.download_by_url(pkg, dst_dir)
         else:
             return self.download_by_name(pkg, dst_dir)
-
-    @staticmethod
-    def need_download_again(target_sha256, dst_file):
-        """
-        need_download_again
-
-        :param name:
-        :param dst_dir:
-        :return:
-        """
-        if target_sha256 is None:
-            return True
-        if not os.path.exists(dst_file):
-            return True
-        file_sha256 = calc_sha256(dst_file)
-        if target_sha256 != file_sha256:
-            LOG.info('target sha256 : %s, existed file sha256 : %s',
-                     target_sha256, file_sha256)
-            print('target sha256 : {}, existed file sha256 : {}'.format(
-                target_sha256, file_sha256))
-            return True
-        else:
-            return False
```

## ascend_deployer/downloader/download_util.py

```diff
@@ -286,14 +286,15 @@
                 print(timeout)
                 LOG.error(timeout)
             finally:
                 pass
             print('please wait for a moment...')
             LOG.info('please wait for a moment...')
             time.sleep(retry * 2)
+        return None
 
     @classmethod
     def download_to_tmp(cls, url: str, retry_times=5):
         for retry in [x + 1 for x in range(retry_times)]:
             try:
                 cls.proxy_inst.build_proxy_handler()
                 tmp_file, _ = request.urlretrieve(url)
```

## ascend_deployer/downloader/logger_config.py

```diff
@@ -20,15 +20,15 @@
 import os
 import platform
 import stat
 
 
 class RotatingFileHandler(logging.handlers.RotatingFileHandler):
     """
-    rewrite RotatingFileHandler, chmod 600 downloader.log and chmod 400 downloader.log.*
+    rewrite RotatingFileHandler, assign permissions to downloader.log and downloader.log.*
     """
     def doRollover(self):
         largest_backfile = "{}.{}".format(self.baseFilename, self.backupCount)
         if os.path.exists(largest_backfile):
             os.chmod(largest_backfile, mode=0o600)
         os.chmod(self.baseFilename, mode=0o400)
         logging.handlers.RotatingFileHandler.doRollover(self)
```

## ascend_deployer/downloader/pip_downloader.py

```diff
@@ -121,14 +121,64 @@
             LOG.error(err)
             return False
         finally:
             pass
 
         return True
 
+    @staticmethod
+    def source_filter(index, version):
+        """
+        source_filter
+
+        :param index:
+        :param version:
+        :return:
+        """
+        pkg = ''
+        url = ''
+        for name, href in index.items():
+            if 'tar' in name or 'zip' in name:
+                if version in name:
+                    pkg = name
+                    url = href
+            else:
+                continue
+        return pkg, url
+
+    @staticmethod
+    def need_download_again(dst_file, url_with_hash):
+        """
+        need_download_again
+        校验目的文件的hash值与url中的hash值是否相等，来决定是否重新下载
+
+        :param dst_file: 目的文件
+        :param url_with_hash:  带hash值的URL
+        :return:
+        """
+        if url_with_hash is None or len(url_with_hash) == 0:
+            return True
+        if not os.path.exists(dst_file):
+            return True
+
+        key_word = ''
+        file_hash = ''
+        if 'sha256=' in url_with_hash:
+            key_word = 'sha256='
+            file_hash = calc_sha256(dst_file)
+        else:
+            return True
+
+        index_of_hash = str(url_with_hash).index(key_word) + len(key_word)
+        target_hash = url_with_hash[index_of_hash:]
+        if target_hash != file_hash:
+            LOG.info('hash {0} in url: {1} != file: {2}'.format(key_word,
+                                                                target_hash, file_hash))
+        return target_hash != file_hash
+
     def get_simple_index(self, distribution):
         """
         get_simple_index
 
         :param distribution:
         :return:
         """
@@ -177,34 +227,14 @@
                 if self.is_wheel_match(name, version, platform, implement):
                     pkg = name
                     url = href
             else:
                 continue
         return pkg, url
 
-    @staticmethod
-    def source_filter(index, version):
-        """
-        source_filter
-
-        :param index:
-        :param version:
-        :return:
-        """
-        pkg = ''
-        url = ''
-        for name, href in index.items():
-            if 'tar' in name or 'zip' in name:
-                if version in name:
-                    pkg = name
-                    url = href
-            else:
-                continue
-        return pkg, url
-
     def get_url_from_obs(self, name, platform, implement):
         if platform == 'none':
             return "", ""
         distribution, version = name.split('==')
         with open(self.obs_resources_file) as file_content:
             index = json.load(file_content)
             for file_name, href in index.items():
@@ -242,15 +272,15 @@
             if not download_url:
                 LOG.info('can not find {0} for {1} {2}'.format(name, platform, implement))
                 return False
         else:
             download_url = '{0}/{1}/{2}'.format(self.pypi_url, distribution, url)
 
         if file_name in self.downloaded:
-            return
+            return True
         LOG.info("Download {0} from [{1}]".format(file_name, download_url))
         file_path = os.path.join(dest_path, file_name)
         if not self.need_download_again(file_path, download_url):
             print(file_name.ljust(60), "exists")
             LOG.info('{0} no need download again'.format(file_name))
             self.downloaded.append(file_name)
             return True
@@ -268,15 +298,15 @@
         """
         distribution, version = name.split('==')
         index = self.get_simple_index(distribution)
         file_name, url = self.source_filter(index, version)
         if len(url) == 0:
             return False
         if file_name in self.downloaded:
-            return
+            return True
         download_url = '{0}/{1}/{2}'.format(self.pypi_url, distribution, url)
         LOG.info("Download {0} from [{1}]".format(file_name, download_url))
         file_path = os.path.join(dest_path, file_name)
         if not self.need_download_again(file_path, url):
             print(file_name.ljust(60), "exists")
             LOG.info('{0} no need download again'.format(file_name))
             self.downloaded.append(file_name)
@@ -285,44 +315,14 @@
         if not CH.check_download_hash(file_path, url):
             LOG.info('the downloaded file：{} hash is not equal to the hash in the url'.format(file_path))
             raise DownloadCheckError(file_path)
         print(file_name.ljust(60), "download success")
         self.downloaded.append(file_name)
         return True
 
-    @staticmethod
-    def need_download_again(dst_file, url_with_hash):
-        """
-        need_download_again
-        校验目的文件的hash值与url中的hash值是否相等，来决定是否重新下载
-
-        :param dst_file: 目的文件
-        :param url_with_hash:  带hash值的URL
-        :return:
-        """
-        if url_with_hash is None or len(url_with_hash) == 0:
-            return True
-        if not os.path.exists(dst_file):
-            return True
-
-        key_word = ''
-        file_hash = ''
-        if 'sha256=' in url_with_hash:
-            key_word = 'sha256='
-            file_hash = calc_sha256(dst_file)
-        else:
-            return True
-
-        index_of_hash = str(url_with_hash).index(key_word) + len(key_word)
-        target_hash = url_with_hash[index_of_hash:]
-        if target_hash != file_hash:
-            LOG.info('hash {0} in url: {1} != file: {2}'.format(key_word,
-                                                                target_hash, file_hash))
-        return target_hash != file_hash
-
     def download_x86(self, name, implement_flag, dest_path):
         """
         download_x86
 
         :param name:
         :param implement_flag:
         :param dest_path:
```

## ascend_deployer/downloader/rpm_downloader.py

```diff
@@ -43,17 +43,17 @@
 finally:
     pass
 
 try:
     import defusedxml
     defusedxml.defuse_stdlib()
 except ImportError:
-    tips = "defusedxml not found! It is recommended that you install "\
+    TIPS = "defusedxml not found! It is recommended that you install "\
         "defusedxml to avoid vulnerabilities related to XML parsing."
-    LOG.info(tips)
+    LOG.info(TIPS)
 
 
 class Package(object):
     """
     rpm package
     """
     def __init__(self, name):
@@ -103,14 +103,99 @@
                 continue
             self.sources[item] = config.get(item, 'baseurl')
             LOG.info(config.get(item, 'baseurl'))
 
         if os.path.exists(self.installed_file):
             self.load_installed(self.installed_file)
 
+    @staticmethod
+    def uncompress_file(compress_file, dst_file):
+        """
+        解压文件
+        """
+        if os.path.exists(dst_file):
+            return
+
+        fd = os.open(dst_file, os.O_WRONLY | os.O_CREAT, 0o640)
+        if compress_file.endswith('.gz'):
+            with gzip.GzipFile(compress_file) as gzip_file:
+                buf = gzip_file.read()
+                with os.fdopen(fd, 'wb') as uncompress_file:
+                    uncompress_file.write(buf)
+            return
+        if compress_file.endswith('.bz2'):
+            with bz2.BZ2File(compress_file, 'rb') as bz_file:
+                buf = bz_file.read()
+                with os.fdopen(fd, 'wb+') as uncompress_file:
+                    uncompress_file.write(buf)
+            return
+        if compress_file.endswith('.xz'):
+            with lzma.open(compress_file, 'rb') as xz_file:
+                buf = xz_file.read()
+                with os.fdopen(fd, 'wb+') as uncompress_file:
+                    uncompress_file.write(buf)
+            return
+        os.close(fd)
+
+    @staticmethod
+    def parse_repomd(file_name, data_type):
+        """
+        解析repomd.xml文件，得到data_type, 如primary_db url
+        """
+        dom = minidom.parse(file_name)
+        data_elements = dom.getElementsByTagName('data')
+        for i in data_elements:
+            if i.getAttribute('type') != data_type:
+                continue
+            location = i.getElementsByTagName('location')[0]
+            print(location.getAttribute('href'))
+            LOG.info(location.getAttribute('href'))
+            return location.getAttribute('href')
+
+    @staticmethod
+    def download_file(url, dst_file):
+        """
+        download_file
+
+        :param url:
+        :param dst_file:
+        :return:
+        """
+        try:
+            LOG.info('download from [{0}]'.format(url))
+            if DOWNLOAD_INST.download(url, dst_file):
+                return True
+            return False
+        except HTTPError as http_error:
+            print('[{0}]->{1}'.format(url, http_error))
+            LOG.error('[{0}]->{1}'.format(url, http_error))
+            return False
+        finally:
+            pass
+
+    @staticmethod
+    def need_download_again(target_sha256, dst_file):
+        """
+        need_download_again
+
+        :param target_sha256:
+        :param dst_file:
+        :return:
+        """
+        if target_sha256 is None:
+            return True
+        if not os.path.exists(dst_file):
+            return True
+        file_sha256 = calc_sha256(dst_file)
+        if target_sha256 != file_sha256:
+            LOG.info('target sha256 : {}, exists file sha256 : {}'.format(target_sha256, file_sha256))
+            return True
+        else:
+            return False
+
     def load_installed(self, file_name):
         with os.fdopen(os.open(file_name, os.O_RDONLY, 0o640), 'r') as f:
             for item in f.readlines():
                 info = [tmp for tmp in item.split(' ') if len(tmp) > 1]
                 [name_and_arch, version, repo] = info
                 [item_name, item_arch] = name_and_arch.split('.')
                 self.installed[item_name] = {'name': item_name, 'arch': item_arch, 'version': version}
@@ -180,87 +265,23 @@
             # 下载数据库文件
             self.download_file(db_url, compressed_file)
 
             if os.path.exists(db_file):
                 os.remove(db_file)
             # 解压数据库文件
             self.uncompress_file(compressed_file, db_file)
+        return True
 
     def clean_cache(self):
         """
         删除数据库文件
         """
         if os.path.exists(self.db_tmps):
             shutil.rmtree(self.db_tmps)
 
-    @staticmethod
-    def uncompress_file(compress_file, dst_file):
-        """
-        解压文件
-        """
-        if os.path.exists(dst_file):
-            return
-
-        fd = os.open(dst_file, os.O_WRONLY | os.O_CREAT, 0o640)
-        if compress_file.endswith('.gz'):
-            with gzip.GzipFile(compress_file) as gzip_file:
-                buf = gzip_file.read()
-                with os.fdopen(fd, 'wb') as uncompress_file:
-                    uncompress_file.write(buf)
-            return
-        if compress_file.endswith('.bz2'):
-            with bz2.BZ2File(compress_file, 'rb') as bz_file:
-                buf = bz_file.read()
-                with os.fdopen(fd, 'wb+') as uncompress_file:
-                    uncompress_file.write(buf)
-            return
-        if compress_file.endswith('.xz'):
-            with lzma.open(compress_file, 'rb') as xz_file:
-                buf = xz_file.read()
-                with os.fdopen(fd, 'wb+') as uncompress_file:
-                    uncompress_file.write(buf)
-            return
-        os.close(fd)
-
-    @staticmethod
-    def parse_repomd(file_name, data_type):
-        """
-        解析repomd.xml文件，得到data_type, 如primary_db url
-        """
-        dom = minidom.parse(file_name)
-        data_elements = dom.getElementsByTagName('data')
-        for i in data_elements:
-            if i.getAttribute('type') != data_type:
-                continue
-            location = i.getElementsByTagName('location')[0]
-            print(location.getAttribute('href'))
-            LOG.info(location.getAttribute('href'))
-            return location.getAttribute('href')
-
-    @staticmethod
-    def download_file(url, dst_file):
-        """
-        download_file
-
-        :param url:
-        :param dst_file:
-        :return:
-        """
-        try:
-            LOG.info('download from [{0}]'.format(url))
-            if DOWNLOAD_INST.download(url, dst_file):
-                return True
-            return False
-        except HTTPError as http_error:
-            print('[{0}]->{1}'.format(url, http_error))
-            LOG.error('[{0}]->{1}'.format(url, http_error))
-            return False
-        finally:
-            pass
-
     def get_requires(self, conn, pkg_name):
         """
         get the requires of the package pkg_name
 
         :param conn: database connecton
         :param pkg_name: package name
         :returns: requite list
@@ -302,15 +323,15 @@
         :param repo_name: repository name, the repository will serch first
         :returns: provides list
         """
         provide_list = []
         repo_list = [repo_name]
         repo_list += [repo for repo in self.sources.keys() if repo not in repo_list]
         for cur_repo in repo_list:
-            repo_url = self.sources[cur_repo]
+            repo_url = self.sources.get(cur_repo, 'not found key')
             db = os.path.join(self.db_tmps, cur_repo + '_primary.sqlite')
             conn = sqlite3.connect(db)
             cur = conn.cursor()
             sql_param = None
             sql = None
             if provide.flags == 'EQ':
                 sql_param = {'name': provide.name, 'version': provide.version,
@@ -334,15 +355,15 @@
             if len(result) > 0 and len(result[0]) > 0:
                 name = result[0][0]
                 ver = result[0][1]
                 rel = result[0][2]
                 if name not in self.installed.keys():
                     provide_list.append(name)
                 elif provide.flags is not None and len(provide.flags) > 0:
-                    if '{0}-{1}'.format(ver, rel) != self.installed[name]['version']:
+                    if '{0}-{1}'.format(ver, rel) != self.installed.get(name, {}).get('version', ''):
                         provide_list.append(name)
             if len(provide_list) > 0:
                 break
 
         return provide_list
 
     def get_dependencies(self, conn, pkg_name, repo_name):
@@ -350,34 +371,14 @@
         require_list = self.get_requires(conn, pkg_name)
         for require in require_list:
             provide_list = self.get_provides(require, repo_name)
             dependencies = list(set(dependencies + provide_list))
 
         return dependencies
 
-    def search_url(self, repo_url, conn, name, ver, rel):
-        sql_str = None
-        sql_param = None
-        if ver is None or rel is None:
-            sql_str = "SELECT location_href FROM packages \
-                WHERE name = :name AND (arch = :arch or arch = 'noarch')"
-            sql_param = {"name": name, "arch": self.arch}
-        else:
-            sql_str = "SELECT location_href FROM packages \
-                WHERE name = :name AND (arch = :arch or arch = 'noarch') \
-                AND version = :version and release = :release"
-            sql_param = {"name": name, "arch": self.arch, "version": ver, "release": rel}
-        cur = conn.cursor()
-        cur.execute(sql_str, sql_param)
-        result = cur.fetchall()
-        LOG.info(result)
-        if len(result) > 0 and len(result[0]) > 0:
-            return urljoin(repo_url, result[0][0])
-        return None
-
     def search_package(self, conn, name, ver, rel):
         sql_str = None
         sql_param = None
         if ver is None or rel is None:
             sql_str = "SELECT location_href, pkgId, version, release \
                 FROM packages \
                 WHERE name = :name AND (arch = :arch or arch = 'noarch')"
@@ -520,14 +521,16 @@
 
         name = pkg['name']
         ver = pkg['version'] if 'version' in pkg else None
         rel = pkg['release'] if 'release' in pkg else None
         download_dir = dst_dir
         if 'dst_dir' in pkg:
             download_dir = os.path.join(os.path.dirname(dst_dir), pkg['dst_dir'])
+            if pkg['dst_dir'] == 'kernel':
+                download_dir = os.path.join(dst_dir, pkg['dst_dir'])
             if not os.path.exists(download_dir):
                 os.makedirs(download_dir, mode=0o750, exist_ok=True)
 
         if 'url' in pkg:
             file_name = os.path.basename(pkg['url'])
             dst_file = os.path.join(download_dir, file_name)
             checksum = pkg['sha256'] if 'sha256' in pkg else None
@@ -540,28 +543,7 @@
             print(file_name.ljust(60), 'download failed')
             raise RuntimeError
 
         if 'autodependency' in pkg and pkg['autodependency'] == 'true':
             return self.download_with_dep(name, download_dir, ver, rel)
         else:
             return self.download_without_dep(name, download_dir, ver, rel)
-
-
-    @staticmethod
-    def need_download_again(target_sha256, dst_file):
-        """
-        need_download_again
-
-        :param target_sha256:
-        :param dst_file:
-        :return:
-        """
-        if target_sha256 is None:
-            return True
-        if not os.path.exists(dst_file):
-            return True
-        file_sha256 = calc_sha256(dst_file)
-        if target_sha256 != file_sha256:
-            LOG.info('target sha256 : {}, exists file sha256 : {}'.format(target_sha256, file_sha256))
-            return True
-        else:
-            return False
```

## ascend_deployer/downloader/software_mgr.py

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 # ===========================================================================
 """software manager,管理可选下载的软件"""
 import json
 import os
 
 CUR_DIR = os.path.dirname(__file__)
-g_software_list = set()
+G_SOFTWARE_LIST = set()
 sys_software_list, ms_software_list, torch_npu_software_list, other_software_list = ([] for _ in range(4))
 
 
 class Software(object):
     """
     软件类，用于存储软件信息
     """
@@ -65,29 +65,29 @@
 
     def get_sys_pkgs(self, sys_name):
         """
         get sys dependencies
         """
         if sys_name not in self.sys_pkgs:
             return []
-        return self.sys_pkgs[sys_name]
+        return self.sys_pkgs.get(sys_name, '')
 
     def set_sys_pkgs(self, sys_name, pkg_list):
         """
         set sys dependencies
         """
         self.sys_pkgs[sys_name] = pkg_list
 
     def get_mindspore(self, sys_name):
         """
         get mindspore
         """
         if sys_name not in self.mindspore:
             return []
-        return self.mindspore[sys_name]
+        return self.mindspore.get(sys_name, '')
     
     def get_torch_npu(self, sys_name):
         """
         get torch_npu
         """
         return self.torch_npu.get(sys_name, [])
 
@@ -146,48 +146,48 @@
     初始化
     """
     soft_dir = os.path.join(CUR_DIR, 'software')
     for _, _, files in os.walk(soft_dir):
         for file_name in files:
             if file_name.endswith('json'):
                 load_software(os.path.join(CUR_DIR, 'software', file_name))
-    global g_software_list
-    g_software_list = set(sys_software_list + ms_software_list + torch_npu_software_list + other_software_list)
+    global G_SOFTWARE_LIST
+    G_SOFTWARE_LIST = set(sys_software_list + ms_software_list + torch_npu_software_list + other_software_list)
 
 
 def get_software_name_version(software):
     """
     获取软件依包的正式名和版本号
     :param in:  software      软件名,可能带==<version>
     :return:   正式名和版本号。例如 CANN==20.2.RC1->CANN,20.2.RC1; MindStudio==2.0.0->MindStudio,2.0.0
     """
-    if len(g_software_list) == 0:
+    if len(G_SOFTWARE_LIST) == 0:
         software_init()
     version = ''
     if '==' in software:
         name = software.split('==')[0]
         version = software.split('==')[1]
     else:
         name = software
-        for soft in g_software_list:
+        for soft in G_SOFTWARE_LIST:
             if soft.get_default() and soft.get_name() == name:
                 version = soft.get_version()
 
     return name, version
 
 
 def get_software_sys(name, sys_name, version=None):
     """
     获取软件依赖的操作系统依赖
     :param in:  name      软件名
     :param in:  sys_name  操作系统
     :param in:  version   软件版本
     :return:   软件name在操作系统sys_name下的系统依赖列表
     """
-    if len(g_software_list) == 0:
+    if len(G_SOFTWARE_LIST) == 0:
         software_init()
     for soft in sys_software_list:
         if version is None:
             if soft.get_name().lower() == name.lower():
                 return soft.get_sys_pkgs(sys_name)
         else:
             if soft.get_name().lower() == name.lower() and soft.get_version() == version:
@@ -199,15 +199,15 @@
     """
     获取软件依赖的操作系统依赖
     :param in:  name      软件名
     :param in:  sys_name  操作系统
     :param in:  version   软件版本
     :return:   软件name在操作系统sys_name下的mindspore whl
     """
-    if len(g_software_list) == 0:
+    if len(G_SOFTWARE_LIST) == 0:
         software_init()
     for soft in ms_software_list:
         if version is None:
             if soft.get_name().lower() == name.lower():
                 return soft.get_mindspore(sys_name)
         else:
             if soft.get_name().lower() == name.lower() and soft.get_version() == version:
@@ -219,15 +219,15 @@
     """
     获取软件依赖的操作系统依赖
     :param in:  name      软件名
     :param in:  sys_name  操作系统
     :param in:  version   软件版本
     :return:   软件name在操作系统sys_name下的mindspore whl
     """
-    if len(g_software_list) == 0:
+    if len(G_SOFTWARE_LIST) == 0:
         software_init()
     for soft in torch_npu_software_list:
         if version is None:
             if soft.get_name().lower() == name.lower():
                 return soft.get_torch_npu(sys_name)
         else:
             if soft.get_name().lower() == name.lower() and soft.get_version() == version:
@@ -238,15 +238,15 @@
 def get_software_other(name, version=None):
     """
     获取软件的其他依赖项
     :param in:  name      软件名
     :param in:  version   软件版本
     :return:   安装软件name所需要下载的其他内容列表
     """
-    if len(g_software_list) == 0:
+    if len(G_SOFTWARE_LIST) == 0:
         software_init()
     for soft in other_software_list:
         if version is None:
             if soft.get_name().lower() == name.lower():
                 return soft.get_other_pkgs()
         else:
             if soft.get_name().lower() == name.lower() and soft.get_version() == version:
@@ -255,26 +255,26 @@
 
 
 def is_software_support(software):
     """
     check if the software is support
     :param in:  software  like mindstudio
     """
-    if len(g_software_list) == 0:
+    if len(G_SOFTWARE_LIST) == 0:
         software_init()
     name = software
     version = None
     if '==' in software:
         name = software.split('==')[0]
         version = software.split('==')[1]
 
     if version is None:
-        for soft in g_software_list:
+        for soft in G_SOFTWARE_LIST:
             if soft.get_name().lower() == name.lower():
                 return True
     else:
-        for soft in g_software_list:
+        for soft in G_SOFTWARE_LIST:
             if soft.get_name().lower() == name.lower() and version == soft.get_version():
                 return True
 
     return False
```

## ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.7717948717948718%*

 * *Differences: {'13': "{'version': '3.6.14', 'release': '6.h7.eulerosv2r10', delete: ['autodependency']}",*

 * * '14': "{'version': '8.2p1', 'release': '9.h46.eulerosv2r10', delete: ['autodependency']}",*

 * * '23': "{'name': 'sqlite', 'version': '3.32.3', 'release': '2.h7.eulerosv2r10', delete: "*

 * *       "['autodependency']}",*

 * * '24': "{'name': 'sqlite-devel', 'info': 'python sqlite', 'version': '3.32.3', 'release': "*

 * *       "'2.h7.eulerosv2r10', delete: ['autodependency']}",*

 * * '44': "{'name': 'krb5-devel'}",*

 * * 'insert': "[(15, Ordere […]*

```diff
@@ -62,22 +62,34 @@
         "name": "cmake"
     },
     {
         "autodependency": "true",
         "name": "unzip"
     },
     {
-        "autodependency": "true",
         "info": "need upgrade to match the new openssl form repo",
-        "name": "gnutls"
+        "name": "gnutls",
+        "release": "6.h7.eulerosv2r10",
+        "version": "3.6.14"
     },
     {
-        "autodependency": "true",
         "info": "need upgrade to match the new openssl form repo",
-        "name": "openssh"
+        "name": "openssh",
+        "release": "9.h46.eulerosv2r10",
+        "version": "8.2p1"
+    },
+    {
+        "name": "openssh-clients",
+        "release": "9.h46.eulerosv2r10",
+        "version": "8.2p1"
+    },
+    {
+        "name": "openssh-server",
+        "release": "9.h46.eulerosv2r10",
+        "version": "8.2p1"
     },
     {
         "autodependency": "true",
         "name": "pciutils"
     },
     {
         "autodependency": "true",
@@ -100,22 +112,24 @@
     },
     {
         "autodependency": "true",
         "info": "python bz2",
         "name": "bzip2-devel"
     },
     {
-        "autodependency": "true",
         "info": "python sqlite",
-        "name": "sqlite-devel"
+        "name": "sqlite",
+        "release": "2.h7.eulerosv2r10",
+        "version": "3.32.3"
     },
     {
-        "autodependency": "true",
-        "info": "python ssl",
-        "name": "openssl-devel"
+        "info": "python sqlite",
+        "name": "sqlite-devel",
+        "release": "2.h7.eulerosv2r10",
+        "version": "3.32.3"
     },
     {
         "autodependency": "true",
         "info": "python gnureadline",
         "name": "ncurses-devel"
     },
     {
@@ -130,14 +144,19 @@
     },
     {
         "name": "sshpass",
         "sha256": "9656bf3703739b0b29b68e0574781118e2327a8e2ee11319fd214c74b9d3c336",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/aarch64/Packages/s/sshpass-1.06-9.el8.aarch64.rpm"
     },
     {
+        "name": "dkms",
+        "sha256": "4b31e97ff478c39228785acbbd702ca69fa2e498c2ad710b130049463fd21928",
+        "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/dkms-2.6.1-5.oe1.noarch.rpm"
+    },
+    {
         "info": "tensorflow use",
         "name": "hdf5",
         "sha256": "6801cac9eeae57268fd55b9dfbcf7ff9caab5633046bca6c2cdc1963833fed37",
         "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/hdf5-1.8.20-7.oe1.aarch64.rpm"
     },
     {
         "info": "tensorflow use",
@@ -178,17 +197,47 @@
     },
     {
         "autodependency": "true",
         "info": "used for edge ha",
         "name": "gzip"
     },
     {
+        "info": "used for edge ha",
+        "name": "openssl",
+        "release": "8.h35.eulerosv2r10",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "used for edge ha",
+        "name": "openssl-devel",
+        "release": "8.h35.eulerosv2r10",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "used for edge ha",
+        "name": "openssl-libs",
+        "release": "8.h35.eulerosv2r10",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "used for edge ha",
+        "name": "openssl-perl",
+        "release": "8.h35.eulerosv2r10",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "python3-libselinux",
+        "release": "1.h5.eulerosv2r10",
+        "version": "3.1"
+    },
+    {
         "autodependency": "true",
         "info": "used for edge ha",
-        "name": "openssl"
+        "name": "krb5-devel"
     },
     {
         "autodependency": "true",
         "info": "used for edge ha",
         "name": "expect"
     },
     {
@@ -211,9 +260,14 @@
         "info": "used for edge ha",
         "name": "ethtool"
     },
     {
         "autodependency": "true",
         "info": "used for edge ha",
         "name": "unzip"
+    },
+    {
+        "autodependency": "true",
+        "info": "used for hdf5",
+        "name": "gcc-gfortran"
     }
 ]
```

## ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.6984496124031008%*

 * *Differences: {'12': "{'version': '3.6.14', 'release': '6.h7.eulerosv2r10', delete: ['autodependency']}",*

 * * '13': "{'version': '8.2p1', 'release': '9.h46.eulerosv2r10', delete: ['autodependency']}",*

 * * '24': "{'version': '3.32.3', 'release': '2.h7.eulerosv2r10', delete: ['autodependency']}",*

 * * '31': "{'name': 'krb5-devel'}",*

 * * 'insert': "[(14, OrderedDict([('name', 'openssh-clients'), ('info', 'need upgrade to match the "*

 * *           "new openssl form repo'), ('version', '8.2p1'), ('release', '9.h46.eulerosv2r10')])), "*

 * *       […]*

```diff
@@ -56,33 +56,55 @@
         "name": "cmake"
     },
     {
         "autodependency": "true",
         "name": "unzip"
     },
     {
-        "autodependency": "true",
         "info": "need upgrade to match the new openssl form repo",
-        "name": "gnutls"
+        "name": "gnutls",
+        "release": "6.h7.eulerosv2r10",
+        "version": "3.6.14"
+    },
+    {
+        "info": "need upgrade to match the new openssl form repo",
+        "name": "openssh",
+        "release": "9.h46.eulerosv2r10",
+        "version": "8.2p1"
     },
     {
-        "autodependency": "true",
         "info": "need upgrade to match the new openssl form repo",
-        "name": "openssh"
+        "name": "openssh-clients",
+        "release": "9.h46.eulerosv2r10",
+        "version": "8.2p1"
+    },
+    {
+        "info": "need upgrade to match the new openssl form repo",
+        "name": "openssh-server",
+        "release": "9.h46.eulerosv2r10",
+        "version": "8.2p1"
     },
     {
         "autodependency": "true",
         "name": "pciutils"
     },
     {
         "autodependency": "true",
         "name": "net-tools"
     },
     {
         "autodependency": "true",
+        "name": "libgomp"
+    },
+    {
+        "autodependency": "true",
+        "name": "gcc-gfortran"
+    },
+    {
+        "autodependency": "true",
         "info": "python cffi",
         "name": "libffi-devel"
     },
     {
         "autodependency": "true",
         "info": "python zlib",
         "name": "zlib-devel"
@@ -94,22 +116,59 @@
     },
     {
         "autodependency": "true",
         "info": "python bz2",
         "name": "bzip2-devel"
     },
     {
-        "autodependency": "true",
         "info": "python sqlite",
-        "name": "sqlite-devel"
+        "name": "sqlite-devel",
+        "release": "2.h7.eulerosv2r10",
+        "version": "3.32.3"
+    },
+    {
+        "info": "python sqlite",
+        "name": "sqlite",
+        "release": "2.h7.eulerosv2r10",
+        "version": "3.32.3"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl-devel",
+        "release": "8.h35.eulerosv2r10",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl",
+        "release": "8.h35.eulerosv2r10",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl-libs",
+        "release": "8.h35.eulerosv2r10",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl-perl",
+        "release": "8.h35.eulerosv2r10",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "python3-libselinux",
+        "release": "1.h5.eulerosv2r10",
+        "version": "3.1"
     },
     {
         "autodependency": "true",
         "info": "python ssl",
-        "name": "openssl-devel"
+        "name": "krb5-devel"
     },
     {
         "autodependency": "true",
         "info": "python gnureadline",
         "name": "ncurses-devel"
     },
     {
@@ -124,14 +183,19 @@
     },
     {
         "name": "sshpass",
         "sha256": "d30541c4470226e2e6708198692f6e62e9435d5b48d0240f089dce7230fc5a49",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/x86_64/Packages/s/sshpass-1.06-9.el8.x86_64.rpm"
     },
     {
+        "name": "dkms",
+        "sha256": "4b31e97ff478c39228785acbbd702ca69fa2e498c2ad710b130049463fd21928",
+        "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/dkms-2.6.1-5.oe1.noarch.rpm"
+    },
+    {
         "info": "tensorflow use",
         "name": "hdf5",
         "sha256": "6cd28daef6ddb05fa36b3a98a13be498e2390c8751f36a12be08b06fdd8d6d40",
         "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/hdf5-1.8.20-7.oe1.x86_64.rpm"
     },
     {
         "info": "tensorflow use",
```

## ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.5880392156862745%*

 * *Differences: {'13': "{'name': 'kernel-headers', 'release': 'vhulk1907.1.0.h1393.eulerosv2r8'}",*

 * * '33': "{'version': '3.6.7', 'release': '1.h11.eulerosv2r8', delete: ['autodependency']}",*

 * * '34': "{'version': '7.8p1', 'release': '3.h55.eulerosv2r8', delete: ['autodependency']}",*

 * * '44': "{'version': '3.24.0', 'release': '2.h20.eulerosv2r8', delete: ['autodependency']}",*

 * * '45': "{'name': 'sqlite-libs', 'info': 'python sqlite', 'version': '3.24.0', 'release': "*

 * *       "'2.h20.eulerosv2r8', delete: ['autodependency']}",*

 * * '65' […]*

```diff
@@ -1,17 +1,11 @@
 [
     {
         "dst_dir": "kernel",
         "name": "kernel-headers",
-        "release": "vhulk1905.1.0.h273.eulerosv2r8",
-        "version": "4.19.36"
-    },
-    {
-        "dst_dir": "kernel",
-        "name": "kernel-headers",
         "release": "vhulk1905.1.0.h276.eulerosv2r8",
         "version": "4.19.36"
     },
     {
         "dst_dir": "kernel",
         "name": "kernel-headers",
         "release": "vhulk1906.1.0.h288.eulerosv2r8",
@@ -51,16 +45,46 @@
         "dst_dir": "kernel",
         "name": "kernel-headers",
         "release": "vhulk1907.1.0.h906.eulerosv2r8",
         "version": "4.19.36"
     },
     {
         "dst_dir": "kernel",
-        "name": "kernel-devel",
-        "release": "vhulk1905.1.0.h273.eulerosv2r8",
+        "name": "kernel-headers",
+        "release": "vhulk1907.1.0.h962.eulerosv2r8",
+        "version": "4.19.36"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk1907.1.0.h1046.eulerosv2r8",
+        "version": "4.19.36"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk1907.1.0.h1103.eulerosv2r8",
+        "version": "4.19.36"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk1907.1.0.h1130.eulerosv2r8",
+        "version": "4.19.36"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk1907.1.0.h1229.eulerosv2r8",
+        "version": "4.19.36"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk1907.1.0.h1393.eulerosv2r8",
         "version": "4.19.36"
     },
     {
         "dst_dir": "kernel",
         "name": "kernel-devel",
         "release": "vhulk1905.1.0.h276.eulerosv2r8",
         "version": "4.19.36"
@@ -104,14 +128,50 @@
     {
         "dst_dir": "kernel",
         "name": "kernel-devel",
         "release": "vhulk1907.1.0.h906.eulerosv2r8",
         "version": "4.19.36"
     },
     {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk1907.1.0.h962.eulerosv2r8",
+        "version": "4.19.36"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk1907.1.0.h1046.eulerosv2r8",
+        "version": "4.19.36"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk1907.1.0.h1103.eulerosv2r8",
+        "version": "4.19.36"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk1907.1.0.h1130.eulerosv2r8",
+        "version": "4.19.36"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk1907.1.0.h1229.eulerosv2r8",
+        "version": "4.19.36"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk1907.1.0.h1393.eulerosv2r8",
+        "version": "4.19.36"
+    },
+    {
         "autodependency": "true",
         "name": "gcc"
     },
     {
         "autodependency": "true",
         "name": "gcc-c++"
     },
@@ -124,22 +184,34 @@
         "name": "cmake"
     },
     {
         "autodependency": "true",
         "name": "unzip"
     },
     {
-        "autodependency": "true",
         "info": "need upgrade to match the new openssl form repo",
-        "name": "gnutls"
+        "name": "gnutls",
+        "release": "1.h11.eulerosv2r8",
+        "version": "3.6.7"
     },
     {
-        "autodependency": "true",
         "info": "need upgrade to match the new openssl form repo",
-        "name": "openssh"
+        "name": "openssh",
+        "release": "3.h55.eulerosv2r8",
+        "version": "7.8p1"
+    },
+    {
+        "name": "openssh-clients",
+        "release": "3.h55.eulerosv2r8",
+        "version": "7.8p1"
+    },
+    {
+        "name": "openssh-server",
+        "release": "3.h55.eulerosv2r8",
+        "version": "7.8p1"
     },
     {
         "autodependency": "true",
         "name": "pciutils"
     },
     {
         "autodependency": "true",
@@ -162,22 +234,30 @@
     },
     {
         "autodependency": "true",
         "info": "python bz2",
         "name": "bzip2-devel"
     },
     {
-        "autodependency": "true",
         "info": "python sqlite",
-        "name": "sqlite-devel"
+        "name": "sqlite",
+        "release": "2.h20.eulerosv2r8",
+        "version": "3.24.0"
     },
     {
-        "autodependency": "true",
-        "info": "python ssl",
-        "name": "openssl-devel"
+        "info": "python sqlite",
+        "name": "sqlite-devel",
+        "release": "2.h20.eulerosv2r8",
+        "version": "3.24.0"
+    },
+    {
+        "info": "python sqlite",
+        "name": "sqlite-libs",
+        "release": "2.h20.eulerosv2r8",
+        "version": "3.24.0"
     },
     {
         "autodependency": "true",
         "info": "used for h5py compile",
         "name": "blas-devel"
     },
     {
@@ -192,14 +272,19 @@
     },
     {
         "name": "sshpass",
         "sha256": "9656bf3703739b0b29b68e0574781118e2327a8e2ee11319fd214c74b9d3c336",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/aarch64/Packages/s/sshpass-1.06-9.el8.aarch64.rpm"
     },
     {
+        "name": "dkms",
+        "sha256": "c8d63b95ec9d4379bdaeef0067ff6f880a7f6d0f18d96dc3deda48e791a8c780",
+        "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/dkms-2.6.1-5.oe1.noarch.rpm"
+    },
+    {
         "info": "tensorflow use",
         "name": "hdf5",
         "sha256": "6801cac9eeae57268fd55b9dfbcf7ff9caab5633046bca6c2cdc1963833fed37",
         "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/hdf5-1.8.20-7.oe1.aarch64.rpm"
     },
     {
         "info": "tensorflow use",
@@ -241,17 +326,97 @@
     },
     {
         "autodependency": "true",
         "info": "used for edge ha",
         "name": "gzip"
     },
     {
+        "info": "used for edge ha",
+        "name": "openssl",
+        "release": "3.h23.eulerosv2r8",
+        "version": "1.1.1"
+    },
+    {
+        "info": "used for edge ha",
+        "name": "openssl-devel",
+        "release": "3.h23.eulerosv2r8",
+        "version": "1.1.1"
+    },
+    {
+        "info": "used for edge ha",
+        "name": "openssl-libs",
+        "release": "3.h23.eulerosv2r8",
+        "version": "1.1.1"
+    },
+    {
+        "info": "used for edge ha",
+        "name": "openssl-perl",
+        "release": "3.h23.eulerosv2r8",
+        "version": "1.1.1"
+    },
+    {
+        "info": "python ssl",
+        "name": "python3-libselinux",
+        "release": "4.h4.eulerosv2r8",
+        "version": "2.8"
+    },
+    {
         "autodependency": "true",
         "info": "used for edge ha",
-        "name": "openssl"
+        "name": "krb5-devel"
+    },
+    {
+        "name": "libcom_err-devel",
+        "release": "1.h12.eulerosv2r8",
+        "version": "1.44.3"
+    },
+    {
+        "name": "libcom_err",
+        "release": "1.h12.eulerosv2r8",
+        "version": "1.44.3"
+    },
+    {
+        "name": "e2fsprogs",
+        "release": "1.h12.eulerosv2r8",
+        "version": "1.44.3"
+    },
+    {
+        "name": "e2fsprogs-libs",
+        "release": "1.h12.eulerosv2r8",
+        "version": "1.44.3"
+    },
+    {
+        "name": "libss",
+        "release": "1.h12.eulerosv2r8",
+        "version": "1.44.3"
+    },
+    {
+        "autodependency": "true",
+        "info": "python ssl",
+        "name": "libselinux-devel"
+    },
+    {
+        "name": "keyutils-libs",
+        "release": "8.h1.eulerosv2r8",
+        "version": "1.5.10"
+    },
+    {
+        "name": "krb5-devel",
+        "release": "21.h1.eulerosv2r8",
+        "version": "1.16.1"
+    },
+    {
+        "name": "libkadm5",
+        "release": "21.h1.eulerosv2r8",
+        "version": "1.16.1"
+    },
+    {
+        "name": "krb5-libs",
+        "release": "21.h1.eulerosv2r8",
+        "version": "1.16.1"
     },
     {
         "autodependency": "true",
         "info": "used for edge ha",
         "name": "expect"
     },
     {
@@ -279,9 +444,14 @@
         "info": "used for edge ha",
         "name": "unzip"
     },
     {
         "autodependency": "true",
         "info": "used for mindspore",
         "name": "gmp-c++"
+    },
+    {
+        "autodependency": "true",
+        "info": "used for hdf5",
+        "name": "gcc-gfortran"
     }
 ]
```

## ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.5153153153153154%*

 * *Differences: {'29': "{'version': '3.6.9', 'release': '6.h12.eulerosv2r9', delete: ['autodependency']}",*

 * * '30': "{'version': '8.2p1', 'release': '2.h41.eulerosv2r9', delete: ['autodependency']}",*

 * * '46': "{'name': 'krb5-devel', 'info': 'python ssl'}",*

 * * '54': "{'name': 'gcc-gfortran', 'info': 'hdf5 need'}",*

 * * 'delete': '[34]',*

 * * 'insert': "[(4, OrderedDict([('name', 'kernel-headers'), ('version', '4.19.90'), ('release', "*

 * *           "'vhulk2011.1.0.h382.eulerosv2r9'), ('dst_dir', 'kernel')])), (5, OrderedDict([('name', "*

 * *    […]*

```diff
@@ -21,14 +21,62 @@
         "dst_dir": "kernel",
         "name": "kernel-headers",
         "release": "vhulk2009.2.0.h310.eulerosv2r9",
         "version": "4.19.90"
     },
     {
         "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk2011.1.0.h382.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk2103.1.0.h487.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk2103.1.0.h584.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk2103.1.0.h640.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk2103.1.0.h781.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk2103.1.0.h848.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk2103.1.0.h911.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "vhulk2103.1.0.h990.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
         "name": "kernel-devel",
         "release": "vhulk2006.2.0.h171.eulerosv2r9",
         "version": "4.19.90"
     },
     {
         "dst_dir": "kernel",
         "name": "kernel-devel",
@@ -44,14 +92,62 @@
     {
         "dst_dir": "kernel",
         "name": "kernel-devel",
         "release": "vhulk2009.2.0.h310.eulerosv2r9",
         "version": "4.19.90"
     },
     {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk2011.1.0.h382.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk2103.1.0.h487.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk2103.1.0.h584.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk2103.1.0.h640.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk2103.1.0.h781.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk2103.1.0.h848.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk2103.1.0.h911.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "vhulk2103.1.0.h990.eulerosv2r9",
+        "version": "4.19.90"
+    },
+    {
         "autodependency": "true",
         "name": "gcc"
     },
     {
         "autodependency": "true",
         "name": "gcc-c++"
     },
@@ -64,22 +160,36 @@
         "name": "cmake"
     },
     {
         "autodependency": "true",
         "name": "unzip"
     },
     {
-        "autodependency": "true",
         "info": "need upgrade to match the new openssl form repo",
-        "name": "gnutls"
+        "name": "gnutls",
+        "release": "6.h12.eulerosv2r9",
+        "version": "3.6.9"
     },
     {
-        "autodependency": "true",
         "info": "need upgrade to match the new openssl form repo",
-        "name": "openssh"
+        "name": "openssh",
+        "release": "2.h41.eulerosv2r9",
+        "version": "8.2p1"
+    },
+    {
+        "info": "need upgrade to match the new openssl form repo",
+        "name": "openssh-clients",
+        "release": "2.h41.eulerosv2r9",
+        "version": "8.2p1"
+    },
+    {
+        "info": "need upgrade to match the new openssl form repo",
+        "name": "openssh-server",
+        "release": "2.h41.eulerosv2r9",
+        "version": "8.2p1"
     },
     {
         "autodependency": "true",
         "name": "pciutils"
     },
     {
         "autodependency": "true",
@@ -102,34 +212,123 @@
     },
     {
         "autodependency": "true",
         "info": "python bz2",
         "name": "bzip2-devel"
     },
     {
-        "autodependency": "true",
         "info": "python sqlite",
-        "name": "sqlite-devel"
+        "name": "sqlite-devel",
+        "release": "1.h11.eulerosv2r9",
+        "version": "3.31.1"
+    },
+    {
+        "info": "python sqlite",
+        "name": "sqlite",
+        "release": "1.h11.eulerosv2r9",
+        "version": "3.31.1"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl-devel",
+        "release": "7.h32.eulerosv2r9",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl",
+        "release": "7.h32.eulerosv2r9",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl-libs",
+        "release": "7.h32.eulerosv2r9",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl-perl",
+        "release": "7.h32.eulerosv2r9",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "python3-libselinux",
+        "release": "1.h10.eulerosv2r9",
+        "version": "2.9"
     },
     {
         "autodependency": "true",
         "info": "python ssl",
-        "name": "openssl-devel"
+        "name": "krb5-devel"
+    },
+    {
+        "info": "python ssl",
+        "name": "krb5-libs",
+        "release": "1.h13.eulerosv2r9",
+        "version": "1.18"
+    },
+    {
+        "info": "python ssl",
+        "name": "e2fsprogs-devel",
+        "release": "0.h1.eulerosv2r9",
+        "version": "1.45.6"
+    },
+    {
+        "info": "python ssl",
+        "name": "keyutils-libs-devel",
+        "release": "1.h2.eulerosv2r9",
+        "version": "1.6.1"
+    },
+    {
+        "info": "python ssl",
+        "name": "libselinux-devel",
+        "release": "1.h5.eulerosv2r9",
+        "version": "2.9"
+    },
+    {
+        "info": "python ssl",
+        "name": "libsepol-devel",
+        "release": "1.eulerosv2r9",
+        "version": "2.9"
+    },
+    {
+        "info": "python ssl",
+        "name": "libverto-devel",
+        "release": "2.eulerosv2r9",
+        "version": "0.3.1"
+    },
+    {
+        "info": "python ssl",
+        "name": "pcre2-devel",
+        "release": "2.h1.eulerosv2r9",
+        "version": "10.33"
+    },
+    {
+        "autodependency": "true",
+        "info": "hdf5 need",
+        "name": "gcc-gfortran"
     },
     {
         "autodependency": "true",
         "info": "python gnureadline",
         "name": "ncurses-devel"
     },
     {
         "name": "sshpass",
         "sha256": "9656bf3703739b0b29b68e0574781118e2327a8e2ee11319fd214c74b9d3c336",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/aarch64/Packages/s/sshpass-1.06-9.el8.aarch64.rpm"
     },
     {
+        "name": "dkms",
+        "sha256": "c8d63b95ec9d4379bdaeef0067ff6f880a7f6d0f18d96dc3deda48e791a8c780",
+        "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/dkms-2.6.1-5.oe1.noarch.rpm"
+    },
+    {
         "info": "tensorflow use",
         "name": "hdf5",
         "sha256": "6801cac9eeae57268fd55b9dfbcf7ff9caab5633046bca6c2cdc1963833fed37",
         "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/hdf5-1.8.20-7.oe1.aarch64.rpm"
     },
     {
         "info": "tensorflow use",
@@ -172,19 +371,14 @@
         "autodependency": "true",
         "info": "used for edge ha",
         "name": "gzip"
     },
     {
         "autodependency": "true",
         "info": "used for edge ha",
-        "name": "openssl"
-    },
-    {
-        "autodependency": "true",
-        "info": "used for edge ha",
         "name": "expect"
     },
     {
         "autodependency": "true",
         "info": "used for edge ha",
         "name": "iptables"
     },
```

## ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.457843137254902%*

 * *Differences: {'31': "{'version': '3.6.9', 'release': '6.h12.eulerosv2r9', delete: ['autodependency']}",*

 * * '32': "{'version': '8.2p1', 'release': '2.h41.eulerosv2r9', delete: ['autodependency']}",*

 * * '48': "{'name': 'krb5-devel', 'info': 'python ssl'}",*

 * * '56': "{'name': 'gcc-gfortran', 'info': 'hdf5 need'}",*

 * * 'insert': "[(4, OrderedDict([('name', 'kernel-headers'), ('version', '4.18.0'), ('release', "*

 * *           "'147.5.1.2.h340.eulerosv2r9'), ('dst_dir', 'kernel')])), (5, OrderedDict([('name', "*

 * *           "'kernel-headers […]*

```diff
@@ -21,14 +21,68 @@
         "dst_dir": "kernel",
         "name": "kernel-headers",
         "release": "147.5.1.0.h269.eulerosv2r9",
         "version": "4.18.0"
     },
     {
         "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "147.5.1.2.h340.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "147.5.1.6.h475.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "147.5.1.6.h541.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "147.5.1.6.h579.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "147.5.1.6.h638.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "147.5.1.6.h766.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "147.5.1.6.h841.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "147.5.1.6.h902.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-headers",
+        "release": "147.5.1.6.h998.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
         "name": "kernel-devel",
         "release": "147.5.0.5.h116.eulerosv2r9",
         "version": "4.18.0"
     },
     {
         "dst_dir": "kernel",
         "name": "kernel-devel",
@@ -44,14 +98,68 @@
     {
         "dst_dir": "kernel",
         "name": "kernel-devel",
         "release": "147.5.1.0.h269.eulerosv2r9",
         "version": "4.18.0"
     },
     {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "147.5.1.2.h340.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "147.5.1.6.h475.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "147.5.1.6.h541.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "147.5.1.6.h579.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "147.5.1.6.h638.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "147.5.1.6.h766.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "147.5.1.6.h841.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "147.5.1.6.h902.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
+        "dst_dir": "kernel",
+        "name": "kernel-devel",
+        "release": "147.5.1.6.h998.eulerosv2r9",
+        "version": "4.18.0"
+    },
+    {
         "autodependency": "true",
         "name": "gcc"
     },
     {
         "autodependency": "true",
         "name": "gcc-c++"
     },
@@ -64,22 +172,36 @@
         "name": "cmake"
     },
     {
         "autodependency": "true",
         "name": "unzip"
     },
     {
-        "autodependency": "true",
         "info": "need upgrade to match the new openssl form repo",
-        "name": "gnutls"
+        "name": "gnutls",
+        "release": "6.h12.eulerosv2r9",
+        "version": "3.6.9"
+    },
+    {
+        "info": "need upgrade to match the new openssl form repo",
+        "name": "openssh",
+        "release": "2.h41.eulerosv2r9",
+        "version": "8.2p1"
     },
     {
-        "autodependency": "true",
         "info": "need upgrade to match the new openssl form repo",
-        "name": "openssh"
+        "name": "openssh-clients",
+        "release": "2.h41.eulerosv2r9",
+        "version": "8.2p1"
+    },
+    {
+        "info": "need upgrade to match the new openssl form repo",
+        "name": "openssh-server",
+        "release": "2.h41.eulerosv2r9",
+        "version": "8.2p1"
     },
     {
         "autodependency": "true",
         "name": "pciutils"
     },
     {
         "autodependency": "true",
@@ -102,22 +224,106 @@
     },
     {
         "autodependency": "true",
         "info": "python bz2",
         "name": "bzip2-devel"
     },
     {
-        "autodependency": "true",
         "info": "python sqlite",
-        "name": "sqlite-devel"
+        "name": "sqlite-devel",
+        "release": "1.h11.eulerosv2r9",
+        "version": "3.31.1"
+    },
+    {
+        "info": "python sqlite",
+        "name": "sqlite",
+        "release": "1.h11.eulerosv2r9",
+        "version": "3.31.1"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl-devel",
+        "release": "7.h32.eulerosv2r9",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl",
+        "release": "7.h32.eulerosv2r9",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl-libs",
+        "release": "7.h32.eulerosv2r9",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "openssl-perl",
+        "release": "7.h32.eulerosv2r9",
+        "version": "1.1.1f"
+    },
+    {
+        "info": "python ssl",
+        "name": "python3-libselinux",
+        "release": "1.h10.eulerosv2r9",
+        "version": "2.9"
     },
     {
         "autodependency": "true",
         "info": "python ssl",
-        "name": "openssl-devel"
+        "name": "krb5-devel"
+    },
+    {
+        "info": "python ssl",
+        "name": "krb5-libs",
+        "release": "1.h13.eulerosv2r9",
+        "version": "1.18"
+    },
+    {
+        "info": "python ssl",
+        "name": "e2fsprogs-devel",
+        "release": "0.h1.eulerosv2r9",
+        "version": "1.45.6"
+    },
+    {
+        "info": "python ssl",
+        "name": "keyutils-libs-devel",
+        "release": "1.h2.eulerosv2r9",
+        "version": "1.6.1"
+    },
+    {
+        "info": "python ssl",
+        "name": "libselinux-devel",
+        "release": "1.h5.eulerosv2r9",
+        "version": "2.9"
+    },
+    {
+        "info": "python ssl",
+        "name": "libsepol-devel",
+        "release": "1.eulerosv2r9",
+        "version": "2.9"
+    },
+    {
+        "info": "python ssl",
+        "name": "libverto-devel",
+        "release": "2.eulerosv2r9",
+        "version": "0.3.1"
+    },
+    {
+        "info": "python ssl",
+        "name": "pcre2-devel",
+        "release": "2.h1.eulerosv2r9",
+        "version": "10.33"
+    },
+    {
+        "autodependency": "true",
+        "info": "hdf5 need",
+        "name": "gcc-gfortran"
     },
     {
         "autodependency": "true",
         "info": "python gnureadline",
         "name": "ncurses-devel"
     },
     {
@@ -132,14 +338,19 @@
     },
     {
         "name": "sshpass",
         "sha256": "d30541c4470226e2e6708198692f6e62e9435d5b48d0240f089dce7230fc5a49",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/x86_64/Packages/s/sshpass-1.06-9.el8.x86_64.rpm"
     },
     {
+        "name": "dkms",
+        "sha256": "4b31e97ff478c39228785acbbd702ca69fa2e498c2ad710b130049463fd21928",
+        "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/dkms-2.6.1-5.oe1.noarch.rpm"
+    },
+    {
         "info": "tensorflow use",
         "name": "hdf5",
         "sha256": "6cd28daef6ddb05fa36b3a98a13be498e2390c8751f36a12be08b06fdd8d6d40",
         "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/hdf5-1.8.20-7.oe1.x86_64.rpm"
     },
     {
         "info": "tensorflow use",
```

## ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt

```diff
@@ -328,18 +328,14 @@
 nss-util.aarch64                             3.54.0-7.uel20                             @anaconda
 numactl-libs.aarch64                             2.0.13-4.uel20                             @anaconda
 openldap.aarch64                             2.4.50-7.uel20                             @anaconda
 openssh.aarch64                             8.2p1-10.up4.uel20                             @anaconda
 openssh-clients.aarch64                             8.2p1-10.up4.uel20                             @anaconda
 openssh-help.noarch                             8.2p1-10.up4.uel20                             @anaconda
 openssh-server.aarch64                             8.2p1-10.up4.uel20                             @anaconda
-openssl.aarch64                             1:1.1.1f-10.uel20                             @anaconda
-openssl-help.noarch                             1:1.1.1f-10.uel20                             @anaconda
-openssl-libs.aarch64                             1:1.1.1f-10.uel20                             @anaconda
-openssl-pkcs11.aarch64                             0.4.10-1.uel20                             @anaconda
 os-prober.aarch64                             1.77-2.uel20                             @anaconda
 p11-kit.aarch64                             0.23.20-2.uel20                             @anaconda
 p11-kit-trust.aarch64                             0.23.20-2.uel20                             @anaconda
 pam.aarch64                             1.4.0-5.up2.uel20                             @anaconda
 pango.aarch64                             1.44.7-3.uel20                             @anaconda
 parted.aarch64                             3.3-6.uel20                             @anaconda
 passwd.aarch64                             0.80-7.uel20                             @anaconda
@@ -479,15 +475,14 @@
 python3-gobject.aarch64                             3.36.1-2.uel20                             @anaconda
 python3-gobject-base.aarch64                             3.36.1-2.uel20                             @anaconda
 python3-gpgme.aarch64                             1.14.0-1.uel20                             @anaconda
 python3-hawkey.aarch64                             0.48.0-2.uel20                             @anaconda
 python3-help.noarch                             3.7.9-13.uel20                             @anaconda
 python3-libcomps.aarch64                             0.1.10-2.uel20                             @anaconda
 python3-libdnf.aarch64                             0.48.0-2.uel20                             @anaconda
-python3-libselinux.aarch64                             3.1-3.uel20                             @anaconda
 python3-linux-procfs.noarch                             0.6.2-3.uel20                             @anaconda
 python3-perf.aarch64                             4.19.90-2106.3.0.0095.up2.uel20                             @anaconda
 python3-pip.noarch                             20.2.2-1.uel20                             @anaconda
 python3-pyparsing.noarch                             2.4.7-2.uel20                             @anaconda
 python3-pyudev.noarch                             0.22.0-1.uel20                             @anaconda
 python3-pyyaml.aarch64                             5.3.1-3.uel20                             @anaconda
 python3-rpm.aarch64                             4.15.1-28.uel20                             @anaconda
```

## ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.8125%*

 * *Differences: {'insert': "[(16, OrderedDict([('name', 'openssl'), ('autodependency', 'true'), ('info', 'python "*

 * *           "ssl')])), (17, OrderedDict([('name', 'python3-libselinux'), ('autodependency', "*

 * *           "'true'), ('info', 'python ssl')])), (22, OrderedDict([('name', 'fuse-overlayfs'), "*

 * *           "('autodependency', 'true'), ('info', 'docker need')])), (23, OrderedDict([('name', "*

 * *           "'container-selinux'), ('autodependency', 'true'), ('info', 'docker need')])), (24, "*

 * *           "OrderedDict([('nam […]*

```diff
@@ -69,14 +69,24 @@
     {
         "autodependency": "true",
         "info": "python ssl",
         "name": "openssl-devel"
     },
     {
         "autodependency": "true",
+        "info": "python ssl",
+        "name": "openssl"
+    },
+    {
+        "autodependency": "true",
+        "info": "python ssl",
+        "name": "python3-libselinux"
+    },
+    {
+        "autodependency": "true",
         "info": "tensorflow use",
         "name": "hdf5"
     },
     {
         "autodependency": "true",
         "info": "tensorflow use",
         "name": "hdf5-devel"
@@ -88,24 +98,44 @@
     },
     {
         "autodependency": "true",
         "info": "used for edge ha",
         "name": "expect"
     },
     {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "fuse-overlayfs"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "container-selinux"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "libcgroup"
+    },
+    {
         "name": "sshpass",
         "sha256": "9656bf3703739b0b29b68e0574781118e2327a8e2ee11319fd214c74b9d3c336",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/aarch64/Packages/s/sshpass-1.06-9.el8.aarch64.rpm"
     },
     {
         "name": "inotify-tools",
         "sha256": "eb4df7f1af81cde3f559800543a052e98f61fec87500742612c689c0329355c6",
         "url": "https://mirrors.huaweicloud.com/epel/8/Everything/aarch64/Packages/i/inotify-tools-3.14-19.el8.aarch64.rpm"
     },
     {
+        "name": "slirp4netns",
+        "sha256": "c3d964fa9cb020cee2efdce3688ef075734b14bf1dd6fde036117d1914d23c3a",
+        "url": "https://mirrors.huaweicloud.com/centos-altarch/7/extras/aarch64/Packages/slirp4netns-0.4.3-4.el7_8.aarch64.rpm"
+    },
+    {
         "name": "docker-ce-cli",
         "release": "3.el8",
         "version": "20.10.8"
     },
     {
         "name": "containerd.io",
         "release": "3.1.el8",
```

## ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo

```diff
@@ -1,5 +1,8 @@
 [base]
 baseurl = https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS-SP2/OS/aarch64/
 
+[extra]
+baseurl=https://mirrors.huaweicloud.com/centos-altarch/7/extras/aarch64/
+
 [docker-ce]
 baseurl=https://mirrors.huaweicloud.com/docker-ce/linux/centos/8/aarch64/stable/
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'9': "{'sha256': '0a2539d147f8ff23e22d9c394bb7fc28e50381582cf4f683f9ed01dd5b0e5bc6'}"}*

```diff
@@ -52,15 +52,15 @@
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
         "dest": "resources/docker/CentOS_7.6",
         "filename": "aarch64.tar.gz",
-        "sha256": "8a9cda6892efde66981af5bcb0fd2a4b3aef097742342174eaa14e6ef7ff1b5b",
+        "sha256": "0a2539d147f8ff23e22d9c394bb7fc28e50381582cf4f683f9ed01dd5b0e5bc6",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/CentOS_7.6/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': '07820ace82d46c67cdbffbb75093469e98105aeb37bf33b2a42880947ba806fb'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
         "dest": "resources/docker/CentOS_7.6",
         "filename": "x86_64.tar.gz",
-        "sha256": "9b7a3378070561afcfe2bf8b895ab182d0982339d3ee621e14c06ede3b123738",
+        "sha256": "07820ace82d46c67cdbffbb75093469e98105aeb37bf33b2a42880947ba806fb",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/CentOS_7.6/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': 'f33ba8b8bb240449b87f627a4a287cc811783f6401c9ff12f4b909988a6ecb58'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
         "dest": "resources/docker/Kylin_V10",
         "filename": "aarch64.tar.gz",
-        "sha256": "e790311958d1ff67ada8902a5fc6ccb9c645823564a47f131b62ad14b232a678",
+        "sha256": "f33ba8b8bb240449b87f627a4a287cc811783f6401c9ff12f4b909988a6ecb58",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Kylin_V10/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': 'acbc31887d44ebfdfeaa80c36106d595b8979d1568f316f829efc9b5226dd764'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
         "dest": "resources/docker/Kylin_V10",
         "filename": "x86_64.tar.gz",
-        "sha256": "590dec57dd9cc12ab456bd3649e235a358f42401ac0020fb61c155078ec73c05",
+        "sha256": "acbc31887d44ebfdfeaa80c36106d595b8979d1568f316f829efc9b5226dd764",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Kylin_V10/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': 'd700c7217e669b11ef7147d49e3324592ca8d117679e3fa47076cf2fc67af1a2'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
         "dest": "resources/docker/OpenEuler_20.03_LTS",
         "filename": "aarch64.tar.gz",
-        "sha256": "c1ba7b50cffcb0cd8810a8e37e3a3a60355cd25f73ad88a0823d69fd1d54ac7a",
+        "sha256": "d700c7217e669b11ef7147d49e3324592ca8d117679e3fa47076cf2fc67af1a2",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/OpenEuler_20.03_LTS/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': 'dcb8f1d8eb6cc5fa13cc5912f418f4d24ca4e60c841ceaeea5753173fdd6c783'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
         "dest": "resources/docker/OpenEuler_20.03_LTS",
         "filename": "x86_64.tar.gz",
-        "sha256": "759f4efb551fbb0319231a9dbbfec672bbd4ae25e0b9f22138c4674c7768b9b0",
+        "sha256": "dcb8f1d8eb6cc5fa13cc5912f418f4d24ca4e60c841ceaeea5753173fdd6c783",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/OpenEuler_20.03_LTS/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': '27d009ea84a868f116aaa8b529feddc0671986082ace26c2036630a71b2acdc8'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
         "dest": "resources/docker/OpenEuler_22.03_LTS",
         "filename": "aarch64.tar.gz",
-        "sha256": "24084da4c6a673790e76fe7a3e5a544961ad57d986c689f46c7d16e685b104d9",
+        "sha256": "27d009ea84a868f116aaa8b529feddc0671986082ace26c2036630a71b2acdc8",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/OpenEuler_22.03_LTS/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': '50c5047685563ae9c46f69d23107ae36e70ec2fb697f0802d7eb9d771ae7d3d1'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
         "dest": "resources/docker/OpenEuler_22.03_LTS",
         "filename": "x86_64.tar.gz",
-        "sha256": "22606df07f0eaeff816a3a60ea3130f304524fcee1331afdcd78be392dc6dca4",
+        "sha256": "50c5047685563ae9c46f69d23107ae36e70ec2fb697f0802d7eb9d771ae7d3d1",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/OpenEuler_22.03_LTS/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': 'd3761acb25a39ba9ba89928e29a8f2c55b2d3fbd7d3e2149e8c469483a4bf5aa'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
         "dest": "resources/docker/Ubuntu_18.04",
         "filename": "aarch64.tar.gz",
-        "sha256": "25a9f220caf6ab26827ac6e1a6e1d36c829c668f8f0e21980e7bb3d227c736c3",
+        "sha256": "d3761acb25a39ba9ba89928e29a8f2c55b2d3fbd7d3e2149e8c469483a4bf5aa",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_18.04/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': '697649547ac7b68547df2a5bcded59b57160b49f59713c9ed76e2e91e771ea1d'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
         "dest": "resources/docker/Ubuntu_18.04",
         "filename": "x86_64.tar.gz",
-        "sha256": "8a2ee718c683ba3408442301cfb01c517d28259d6d60b00e6b6297b1a0aff5f1",
+        "sha256": "697649547ac7b68547df2a5bcded59b57160b49f59713c9ed76e2e91e771ea1d",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_18.04/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': 'a7249265cbabb821a0b1e13463899f294b8358b7a9067f2b9db199ccc0811f24'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
         "dest": "resources/docker/Ubuntu_20.04",
         "filename": "aarch64.tar.gz",
-        "sha256": "c5aedac3e214973ecc566d8e9279b5f3c3076c80425992b6567b355925e85651",
+        "sha256": "a7249265cbabb821a0b1e13463899f294b8358b7a9067f2b9db199ccc0811f24",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_20.04/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': '7acc79a78e3804cf5a764e2c6320199e74d17d91a2cad5a6c059a6e90aaca937'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
         "dest": "resources/docker/Ubuntu_22.04",
         "filename": "aarch64.tar.gz",
-        "sha256": "90459bf802636653f8c30f996effe6f2e484edd4e522f68cffcc3bdfeb152451",
+        "sha256": "7acc79a78e3804cf5a764e2c6320199e74d17d91a2cad5a6c059a6e90aaca937",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_22.04/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {'10': "{'sha256': 'e3f7e79931aa249fd4e7f98ae38716b40d8033356841d6d87fb8db98b0a135a8'}"}*

```diff
@@ -58,15 +58,15 @@
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
         "dest": "resources/docker/Ubuntu_22.04",
         "filename": "x86_64.tar.gz",
-        "sha256": "cd4b2e563edfa477acf1a5e1b67d0c10e7acd33fc5c485614f5769a7318943ed",
+        "sha256": "e3f7e79931aa249fd4e7f98ae38716b40d8033356841d6d87fb8db98b0a135a8",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_22.04/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
```

## ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {'insert': "[(4, OrderedDict([('filename', "*

 * *           "'Ascend-mindxdl-ascend-operator_5.0.RC1_linux-aarch64.zip'), ('url', "*

 * *           "'https://mindx.obs.cn-south-1.myhuaweicloud.com/OpenSource/MindX/MindX%205.0.RC1/Ascend-mindxdl-ascend-operator_5.0.RC1_linux-aarch64.zip'), "*

 * *           "('sha256', '71b3a9aeb438f8b388d2cdff9ba36973e712c2f963a7e513b705a73e03409c51'), "*

 * *           "('dest', 'resources/mindxdl/dlPackage/aarch64')])), (5, OrderedDict([('filename', "*

 * *           "'Ascend-mindxdl-resilience- […]*

```diff
@@ -21,14 +21,26 @@
         "dest": "resources/mindxdl/dlPackage/aarch64",
         "filename": "Ascend-mindxdl-device-plugin_5.0.RC1_linux-aarch64.zip",
         "sha256": "eab46c4db3d7d6ebc02dd0c3d42973d7837b8eb8acbef22b1ec2cc4c150d9f02",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/mindxdl/dlPackage/aarch64/Ascend-mindxdl-device-plugin_5.0.RC1_linux-aarch64.zip"
     },
     {
         "dest": "resources/mindxdl/dlPackage/aarch64",
+        "filename": "Ascend-mindxdl-ascend-operator_5.0.RC1_linux-aarch64.zip",
+        "sha256": "71b3a9aeb438f8b388d2cdff9ba36973e712c2f963a7e513b705a73e03409c51",
+        "url": "https://mindx.obs.cn-south-1.myhuaweicloud.com/OpenSource/MindX/MindX%205.0.RC1/Ascend-mindxdl-ascend-operator_5.0.RC1_linux-aarch64.zip"
+    },
+    {
+        "dest": "resources/mindxdl/dlPackage/aarch64",
+        "filename": "Ascend-mindxdl-resilience-controller_5.0.RC1_linux-aarch64.zip",
+        "sha256": "ea2d56f57224d38f439f33f7ae598b9b36bd866099874dff8201c4b9d72dd195",
+        "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/MindX%205.0.RC1/Ascend-mindxdl-resilience-controller_5.0.RC1_linux-aarch64.zip"
+    },
+    {
+        "dest": "resources/mindxdl/dlPackage/aarch64",
         "filename": "Ascend-mindxdl-npu-exporter_5.0.RC1_linux-aarch64.zip",
         "sha256": "bf662c67858b480ad355ff59e04658e772bc4f24150d301f6597884c96ec85e0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/mindxdl/dlPackage/aarch64/Ascend-mindxdl-npu-exporter_5.0.RC1_linux-aarch64.zip"
     },
     {
         "dest": "resources/mindxdl/dlPackage/aarch64",
         "filename": "Ascend-mindxdl-hccl-controller_5.0.RC1_linux-aarch64.zip",
```

## ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {'insert': "[(8, OrderedDict([('filename', "*

 * *           "'Ascend-mindxdl-ascend-operator_5.0.RC1_linux-x86_64.zip'), ('url', "*

 * *           "'https://mindx.obs.cn-south-1.myhuaweicloud.com/OpenSource/MindX/MindX%205.0.RC1/Ascend-mindxdl-ascend-operator_5.0.RC1_linux-x86_64.zip'), "*

 * *           "('sha256', 'f9a5e20aaa87262f49c56a983ff00797727d5b90a8f689f841cdbe415f2a7141'), "*

 * *           "('dest', 'resources/mindxdl/dlPackage/x86_64')])), (9, OrderedDict([('filename', "*

 * *           "'Ascend-mindxdl-resilience-con […]*

```diff
@@ -44,14 +44,26 @@
     {
         "dest": "resources/mindxdl/dlPackage/x86_64",
         "filename": "Ascend-mindxdl-device-plugin_5.0.RC1_linux-x86_64.zip",
         "sha256": "9b583db4acff8a9d43432369cf8a6daf13a2c2f450b18c3827dce8f9cc4234d5",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/mindxdl/dlPackage/x86_64/Ascend-mindxdl-device-plugin_5.0.RC1_linux-x86_64.zip"
     },
     {
+        "dest": "resources/mindxdl/dlPackage/x86_64",
+        "filename": "Ascend-mindxdl-ascend-operator_5.0.RC1_linux-x86_64.zip",
+        "sha256": "f9a5e20aaa87262f49c56a983ff00797727d5b90a8f689f841cdbe415f2a7141",
+        "url": "https://mindx.obs.cn-south-1.myhuaweicloud.com/OpenSource/MindX/MindX%205.0.RC1/Ascend-mindxdl-ascend-operator_5.0.RC1_linux-x86_64.zip"
+    },
+    {
+        "dest": "resources/mindxdl/dlPackage/x86_64",
+        "filename": "Ascend-mindxdl-resilience-controller_5.0.RC1_linux-x86_64.zip",
+        "sha256": "16e9178e06100f7e84a7067d820f3b3f1780bdbec0ec418e5334aa543723f700",
+        "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/MindX%205.0.RC1/Ascend-mindxdl-resilience-controller_5.0.RC1_linux-x86_64.zip"
+    },
+    {
         "dest": "resources/npu",
         "filename": "Ascend-hdk-310p-npu_23.0.rc1_linux-x86-64.zip",
         "sha256": "ed33d8741918e6b736fd988ca027bb1e828b78d29f6399ed7e49a1d3b80d8f4b",
         "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/Ascend%20HDK/Ascend%20HDK%2023.0.RC1/Ascend-hdk-310p-npu_23.0.rc1_linux-x86-64.zip"
     },
     {
         "dest": "resources/npu",
```

## ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py

```diff
@@ -22,48 +22,48 @@
 
 LOG = logger_config.LOG
 
 try:
     import defusedxml
     defusedxml.defuse_stdlib()
 except ImportError:
-    tips = "defusedxml not found! It is recommended that you install "\
+    TIPS = "defusedxml not found! It is recommended that you install "\
         "defusedxml to avoid vulnerabilities related to XML parsing."
-    LOG.info(tips)
+    LOG.info(TIPS)
 
 
 class Require(object):
     def __init__(self, name):
         self.name = name
         self.flags = None
         self.epoch = None
         self.version = None
         self.release = None
-        self.pkgKey = None
+        self.pkg_key = None
         self.pre = False
 
 
 class Provide(object):
     def __init__(self, name):
         self.name = name
         self.flags = None
         self.epoch = None
         self.version = None
         self.release = None
-        self.pkgKey = None
+        self.pkg_key = None
 
 
 class YumPackageHandler(xml.sax.handler.ContentHandler):
     """
     parse xml of rpm packages
     """
     def __init__(self):
         super(YumPackageHandler, self).__init__()
-        self.CurrentData = ""
-        self.CurrentAttributes = ""
+        self.current_data = ""
+        self.current_attributes = ""
         self.checksum = None
         self.name = None
         self.arch = None
         self.summary = None
         self.description = None
         self.url = None
 
@@ -88,16 +88,16 @@
         :param key     key
         :param value   value
         :return:
         """
         self.pkg.package[key] = value
 
     def startElement(self, tag, attributes):
-        self.CurrentData = tag
-        self.CurrentAttributes = attributes
+        self.current_data = tag
+        self.current_attributes = attributes
         if tag == 'package':
             self.pkg = YumPackage({})
             self.packages.append(self.pkg)
         elif tag == 'version':
             self.version_attr = attributes
         elif tag == 'time':
             self.time_attr = attributes
@@ -115,43 +115,43 @@
             self.require_flag = True
             self.provide_flag = False
             self.require_list = []
         elif tag == 'rpm:entry':
             self.entry_attr = attributes
 
     def endElement(self, tag):
-        if self.CurrentData == "checksum":
+        if self.current_data == "checksum":
             self.set_pkg('pkgId', self.checksum)
             self.set_pkg('checksum_type', self.checksum_attr.get('type'))
             self.checksum_attr = {}
-        elif self.CurrentData == 'name':
+        elif self.current_data == 'name':
             self.set_pkg('name', self.name)
-        elif self.CurrentData == 'arch':
+        elif self.current_data == 'arch':
             self.set_pkg('arch', self.arch)
-        elif self.CurrentData == 'version':
+        elif self.current_data == 'version':
             self.set_pkg("version", self.version_attr.get('ver'))
             self.set_pkg("epoch", self.version_attr.get('epoch'))
             self.set_pkg("release", self.version_attr.get('rel'))
             self.version_attr = {}
-        elif self.CurrentData == 'summary':
+        elif self.current_data == 'summary':
             self.set_pkg('summary', self.summary)
-        elif self.CurrentData == 'description':
+        elif self.current_data == 'description':
             self.set_pkg('description', self.description)
-        elif self.CurrentData == 'url':
+        elif self.current_data == 'url':
             self.set_pkg('url', self.url)
-        elif self.CurrentData == 'time':
+        elif self.current_data == 'time':
             self.set_pkg('time_file', self.time_attr.get('file'))
             self.set_pkg('time_build', self.time_attr.get('build'))
             self.time_attr = {}
-        elif self.CurrentData == 'size':
+        elif self.current_data == 'size':
             self.set_pkg('size_package', self.size_attr.get('package'))
             self.set_pkg('size_installed', self.size_attr.get('installed'))
             self.set_pkg('size_archive', self.size_attr.get('archive'))
             self.size_attr = {}
-        elif self.CurrentData == 'location':
+        elif self.current_data == 'location':
             self.set_pkg('location_href', self.location_attr.get('href'))
             self.set_pkg('location_base', self.location_attr.get('base'))
             self.location_attr = {}
         elif tag == 'rpm:entry':
             if self.provide_flag:
                 pro = Provide(self.entry_attr.get('name'))
                 pro.flags = self.entry_attr.get('flags')
@@ -173,25 +173,25 @@
             self.set_pkg('provides', self.provide_list)
             self.provide_flag = False
         elif tag == 'rpm:requires':
             self.set_pkg('requires', self.require_list)
             self.require_flag = False
 
     def characters(self, content):
-        if self.CurrentData == 'checksum':
+        if self.current_data == 'checksum':
             self.checksum = content
-        elif self.CurrentData == 'name':
+        elif self.current_data == 'name':
             self.name = content
-        elif self.CurrentData == 'arch':
+        elif self.current_data == 'arch':
             self.arch = content
-        elif self.CurrentData == 'summary':
+        elif self.current_data == 'summary':
             self.summary = content
-        elif self.CurrentData == 'description':
+        elif self.current_data == 'description':
             self.description = content
-        elif self.CurrentData == 'url':
+        elif self.current_data == 'url':
             self.url = content
 
 
 class YumPackage(object):
     def __init__(self, package):
 
         self.package = package
```

## ascend_deployer/group_vars/all.yaml

```diff
@@ -27,17 +27,20 @@
 K8S_COMPONENT: "k8s"
 DOCKER_RUNTIME_COMPONENT: "docker-runtime"
 DEVICE_PLUGIN_COMPONENT: "device-plugin"
 HCCL_COMPONENT: "hccl-controller"
 VOLCANO_COMPONENT: "volcano"
 NODED_COMPONENT: "noded"
 NPU_EXPORTER_COMPONENT: "npu-exporter"
-
+ASCEND_OPERATOR: "ascend-operator"
+RESILIENCE_CONTROLLER: "resilience-controller"
 SCENES: {
-          1: ["{{DOCKER_COMPONENT}}", "{{K8S_COMPONENT}}", "{{DOCKER_RUNTIME_COMPONENT}}", "{{DEVICE_PLUGIN_COMPONENT}}", "{{HCCL_COMPONENT}}", "{{VOLCANO_COMPONENT}}", "{{NODED_COMPONENT}}", "{{NPU_EXPORTER_COMPONENT}}"],
+          1: ["{{DOCKER_COMPONENT}}", "{{K8S_COMPONENT}}", "{{DOCKER_RUNTIME_COMPONENT}}", "{{DEVICE_PLUGIN_COMPONENT}}",
+              "{{HCCL_COMPONENT}}", "{{VOLCANO_COMPONENT}}", "{{NODED_COMPONENT}}", "{{NPU_EXPORTER_COMPONENT}}",
+              "{{ASCEND_OPERATOR}}", "{{RESILIENCE_CONTROLLER}}"],
           2: ["{{DOCKER_RUNTIME_COMPONENT}}", "{{DEVICE_PLUGIN_COMPONENT}}", "{{VOLCANO_COMPONENT}}"],
           3: ["{{DOCKER_RUNTIME_COMPONENT}}", "{{DEVICE_PLUGIN_COMPONENT}}"],
           4: ["{{DOCKER_COMPONENT}}", "{{K8S_COMPONENT}}"]
 }
 
 NO_DOCKER_K8S_SCENES: [2, 3]
 SCENE_NUM: 1
```

## ascend_deployer/playbooks/clean_nexus.yml

```diff
@@ -1,7 +1,10 @@
 - hosts: '{{ hosts_name }}'
   tasks:
     - name: clean nexus
-      shell: docker rm -f nexus && rm -rf /tmp/nexus-data
+      shell: |
+        docker rm -f nexus
+        umount /tmp/nexus-data
+        rm -rf /tmp/nexus-data
       delegate_to: localhost
       run_once: true
       when: ansible_user_uid == 0
```

## ascend_deployer/playbooks/docker.yaml

```diff
@@ -20,14 +20,26 @@
     - roles/mindx.docker/vars/main.yml
   tasks:
     - include_tasks: roles/mindx.docker/tasks/install.yml
       when:
         - not docker_installed
 
 - hosts:
+    - master
+    - worker
+  gather_facts: false
+  become: yes
+  vars_files:
+    - roles/mindx.docker/vars/main.yml
+  tasks:
+    - include_tasks: roles/mindx.docker/tasks/install_containerd.yml
+      when:
+        - not use_old_k8s_version
+
+- hosts:
     - localhost
     - master
     - worker
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.docker/vars/main.yml
```

## ascend_deployer/playbooks/hccn.yaml

```diff
@@ -1,6 +1,10 @@
 - hosts:
     - hccn
   gather_facts: true
   become: yes
   tasks:
-    - include_tasks: roles/mindx.hccn/tasks/hccn_conf.yaml
+    - include_tasks: roles/mindx.hccn/tasks/hccn_conf.yaml
+
+- name: generate report
+  import_playbook: report.yaml
+  tags: always
```

## ascend_deployer/playbooks/k8s.yaml

```diff
@@ -8,15 +8,14 @@
     - worker
   max_fail_percentage: 1
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.k8s/vars/main.yml
   tasks:
-    - include_tasks: roles/mindx.k8s/tasks/install/get_k8s_version.yml
     - include_tasks: roles/mindx.k8s/tasks/install/main.yml
 
 # 安装K8s
 - hosts:
     - master
     - worker
   gather_facts: false
```

## ascend_deployer/playbooks/mindxdl.yaml

```diff
@@ -35,14 +35,34 @@
   become: yes
   tasks:
     - include_tasks: roles/mindx.dl/tasks/hccl.yaml
       when:
         - "HCCL_COMPONENT in (SCENES[SCENE_NUM] + EXTRA_COMPONENT.split(','))"
 
 - hosts:
+    - master
+  gather_facts: false
+  become: yes
+  tasks:
+    - include_tasks: roles/mindx.dl/tasks/ascend-operator.yaml
+      when:
+        - "ASCEND_OPERATOR in (SCENES[SCENE_NUM] + EXTRA_COMPONENT.split(','))"
+        - not use_old_k8s_version
+
+- hosts:
+    - master
+  gather_facts: false
+  become: yes
+  tasks:
+    - include_tasks: roles/mindx.dl/tasks/resilience-controller.yaml
+      when:
+        - "RESILIENCE_CONTROLLER in (SCENES[SCENE_NUM] + EXTRA_COMPONENT.split(','))"
+        - not use_old_k8s_version
+
+- hosts:
     - worker
   gather_facts: false
   become: yes
   tasks:
     - include_tasks: roles/mindx.dl/tasks/deviceplugin.yaml
       when:
         - "DEVICE_PLUGIN_COMPONENT in (SCENES[SCENE_NUM] + EXTRA_COMPONENT.split(','))"
```

## ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml

```diff
@@ -4,15 +4,14 @@
   failed_when: false
   changed_when: have_selinux.rc != 0
 
 - name: create libselinux directory
   file:
     path: ~/libselinux
     state: directory
-    recurse: yes
   when: have_selinux.rc != 0
 
 - name: scp libselinux-python to remote
   shell: scp ../resources/{{os_and_arch}}/libselinux*.rpm {{ansible_ssh_user}}@{{ansible_default_ipv4.address}}:~/libselinux
   delegate_to: localhost
   when:
     - inventory_hostname != "localhost"
```

## ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml

```diff
@@ -4,15 +4,14 @@
   failed_when: false
   changed_when: have_selinux.rc != 0
 
 - name: create libselinux directory
   file:
     path: ~/libselinux
     state: directory
-    recurse: yes
   when: have_selinux.rc != 0
 
 - name: scp libselinux-python to remote
   shell: scp ../resources/{{os_and_arch}}/libselinux*.rpm {{ansible_ssh_user}}@{{ansible_default_ipv4.address}}:~/libselinux
   delegate_to: localhost
   when:
     - inventory_hostname != "localhost"
```

## ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_aarch64.yml

```diff
@@ -4,15 +4,14 @@
   failed_when: false
   changed_when: have_selinux.rc != 0
 
 - name: create libselinux directory
   file:
     path: ~/libselinux
     state: directory
-    recurse: yes
   when: have_selinux.rc != 0
 
 - name: scp libselinux-python to remote
   shell: scp ../resources/{{os_and_arch}}/*libselinux*.rpm {{ansible_ssh_user}}@{{ansible_default_ipv4.address}}:~/libselinux
   delegate_to: localhost
   when:
     - inventory_hostname != "localhost"
@@ -37,15 +36,14 @@
   failed_when: false
   changed_when: have_tar.rc != 0
 
 - name: create tar directory
   file:
     path: ~/tar
     state: directory
-    recurse: yes
   when: have_tar.rc != 0
 
 - name: scp tar to remote
   shell: scp ../resources/{{os_and_arch}}/tar*.rpm {{ansible_ssh_user}}@{{ansible_default_ipv4.address}}:~/tar
   delegate_to: localhost
   when:
     - inventory_hostname != "localhost"
```

## ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_x86_64.yml

```diff
@@ -4,15 +4,14 @@
   failed_when: false
   changed_when: have_selinux.rc != 0
 
 - name: create libselinux directory
   file:
     path: ~/libselinux
     state: directory
-    recurse: yes
   when: have_selinux.rc != 0
 
 - name: scp libselinux-python to remote
   shell: scp ../resources/{{os_and_arch}}/*libselinux*.rpm {{ansible_ssh_user}}@{{ansible_default_ipv4.address}}:~/libselinux
   delegate_to: localhost
   when:
     - inventory_hostname != "localhost"
@@ -37,15 +36,14 @@
   failed_when: false
   changed_when: have_tar.rc != 0
 
 - name: create tar directory
   file:
     path: ~/tar
     state: directory
-    recurse: yes
   when: have_tar.rc != 0
 
 - name: scp tar to remote
   shell: scp ../resources/{{os_and_arch}}/tar*.rpm {{ansible_ssh_user}}@{{ansible_default_ipv4.address}}:~/tar
   delegate_to: localhost
   when:
     - inventory_hostname != "localhost"
```

## ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml

```diff
@@ -4,15 +4,14 @@
   failed_when: false
   changed_when: have_selinux.rc != 0
 
 - name: create libselinux directory
   file:
     path: ~/libselinux
     state: directory
-    recurse: yes
   when: have_selinux.rc != 0
 
 - name: scp libselinux-python to remote
   shell: scp ../resources/{{os_and_arch}}/*libselinux*.rpm {{ansible_ssh_user}}@{{ansible_default_ipv4.address}}:~/libselinux
   delegate_to: localhost
   when:
     - inventory_hostname != "localhost"
@@ -26,7 +25,30 @@
     - have_selinux.rc != 0
 
 # Usually the libselinux in the repository is newer than system
 # so here add --replacepkgs
 - name: install libselinux-python
   shell: rpm -ivh --force --replacepkgs --nodeps ~/libselinux/*libselinux*.rpm
   when: have_selinux.rc != 0 and ansible_user_uid == 0
+
+- name: check if have tar
+  shell: "tar --version"
+  register: have_tar
+  failed_when: false
+  changed_when: have_tar.rc != 0
+
+- name: create tar directory
+  file:
+    path: ~/tar
+    state: directory
+  when: have_tar.rc != 0
+
+- name: scp tar to remote
+  shell: scp ../resources/{{os_and_arch}}/tar*.rpm {{ansible_ssh_user}}@{{ansible_default_ipv4.address}}:~/tar
+  delegate_to: localhost
+  when:
+    - inventory_hostname != "localhost"
+    - have_tar.rc != 0
+
+- name: install tar
+  shell: yum install -y tar ~/tar/tar*.rpm --disablerepo="*"
+  when: have_tar.rc != 0 and ansible_user_uid == 0
```

## ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml

```diff
@@ -4,15 +4,14 @@
   failed_when: false
   changed_when: have_selinux.rc != 0
 
 - name: create libselinux directory
   file:
     path: ~/libselinux
     state: directory
-    recurse: yes
   when: have_selinux.rc != 0
 
 - name: scp libselinux-python to remote
   shell: scp ../resources/{{os_and_arch}}/*libselinux*.rpm {{ansible_ssh_user}}@{{ansible_default_ipv4.address}}:~/libselinux
   delegate_to: localhost
   when:
     - inventory_hostname != "localhost"
@@ -26,7 +25,30 @@
     - have_selinux.rc != 0
 
 # Usually the libselinux in the repository is newer than system
 # so here add --replacepkgs
 - name: install libselinux-python
   shell: rpm -ivh --force --replacepkgs --nodeps ~/libselinux/*libselinux*.rpm
   when: have_selinux.rc != 0 and ansible_user_uid == 0
+
+- name: check if have tar
+  shell: "tar --version"
+  register: have_tar
+  failed_when: false
+  changed_when: have_tar.rc != 0
+
+- name: create tar directory
+  file:
+    path: ~/tar
+    state: directory
+  when: have_tar.rc != 0
+
+- name: scp tar to remote
+  shell: scp ../resources/{{os_and_arch}}/tar*.rpm {{ansible_ssh_user}}@{{ansible_default_ipv4.address}}:~/tar
+  delegate_to: localhost
+  when:
+    - inventory_hostname != "localhost"
+    - have_tar.rc != 0
+
+- name: install tar
+  shell: yum install -y tar ~/tar/tar*.rpm --disablerepo="*"
+  when: have_tar.rc != 0 and ansible_user_uid == 0
```

## ascend_deployer/playbooks/install/install_atlasedge.yml

 * *Ordering differences only*

```diff
@@ -1,20 +1,20 @@
 - hosts: '{{ hosts_name }}'
   tasks:
     - name: create user
       import_tasks: ../create_user.yml
       when: ansible_user_uid == 0
 
+    - name: message
+      debug:
+        msg:
+        - "[ASCEND]not support installing atlasedge by non-root user, please switch to root user"
+      when: ansible_user_uid != 0
+
     - name: install atlasedge
       import_tasks: task_atlasedge.yml
       when: ansible_user_uid == 0
 
     - name: fail if not root
       fail:
         status: 3
       when: "'atlasedge' in ansible_run_tags and ansible_user_uid != 0"
-
-    - name: message
-      debug:
-        msg:
-        - "[ASCEND]not support installing atlasedge by non-root user, please switch to root user"
-      when: ansible_user_uid != 0
```

## ascend_deployer/playbooks/install/install_driver.yml

 * *Ordering differences only*

```diff
@@ -30,17 +30,17 @@
         - NPUIssue is defined
         - force_upgrade_npu == 'false'
 
     - name: import driver task
       import_tasks: task_driver.yml
       when: ansible_user_uid == 0
 
-    - name: fail if not root
-      fail:
-        status: 3
-      when: "'driver' in ansible_run_tags and ansible_user_uid != 0"
-
     - name: message
       debug:
         msg:
         - "[ASCEND]not support installing driver by non-root user, please switch to root user"
       when: ansible_user_uid != 0
+
+    - name: fail if not root
+      fail:
+        status: 3
+      when: "'driver' in ansible_run_tags and ansible_user_uid != 0"
```

## ascend_deployer/playbooks/install/install_firmware.yml

 * *Ordering differences only*

```diff
@@ -31,17 +31,17 @@
         - NPUIssue is defined
         - force_upgrade_npu == 'false'
 
     - name: import firmware task
       import_tasks: task_firmware.yml
       when: ansible_user_uid == 0
 
-    - name: fail if not root
-      fail:
-        status: 3
-      when: "'firmware' in ansible_run_tags and ansible_user_uid != 0"
-
     - name: message
       debug:
         msg:
         - "[ASCEND]not support installing firmware by non-root user, please switch to root user"
       when: ansible_user_uid != 0
+
+    - name: fail if not root
+      fail:
+        status: 3
+      when: "'firmware' in ansible_run_tags and ansible_user_uid != 0"
```

## ascend_deployer/playbooks/install/install_ha.yml

```diff
@@ -4,17 +4,18 @@
       import_tasks: ../create_user.yml
       when: ansible_user_uid == 0
 
     - name: install ha
       import_tasks: task_ha.yml
       when: ansible_user_uid == 0
 
-    - name: fail if not root
-      fail:
-        status: 3
-      when: "'ha' in ansible_run_tags and ansible_user_uid != 0"
-
     - name: message
       debug:
         msg:
         - "[ASCEND]not support installing ha by non-root user, please switch to root user"
       when: ansible_user_uid != 0
+
+    - name: fail if not root
+      fail:
+        status: 3
+      when: "'ha' in ansible_run_tags and ansible_user_uid != 0"
+
```

## ascend_deployer/playbooks/install/install_ief.yml

 * *Ordering differences only*

```diff
@@ -1,16 +1,16 @@
 - hosts: '{{ hosts_name }}'
   tasks:
     - name: install ief
       import_tasks: task_ief.yml
       when: ansible_user_uid == 0
 
-    - name: fail if not root
-      fail:
-        status: 3
-      when: "'ief' in ansible_run_tags and ansible_user_uid != 0"
-
     - name: message
       debug:
         msg:
         - "[ASCEND]not support installing ief by non-root user, please switch to root user"
       when: ansible_user_uid != 0
+
+    - name: fail if not root
+      fail:
+        status: 3
+      when: "'ief' in ansible_run_tags and ansible_user_uid != 0"
```

## ascend_deployer/playbooks/install/install_pytorch.yml

```diff
@@ -59,15 +59,15 @@
         file_type: file
         use_regex: yes
         patterns: ".*apex.*{{ ansible_architecture }}.whl"
       register: apex_whl
       when: import_torch.rc != 0
 
     - name: install pytorch if not import
-      import_tasks: task_pytorch.yml
+      include_tasks: task_pytorch.yml
       when:
         - import_torch.rc != 0
         - pytorch_whl.matched > 0
         - apex_whl.matched > 0
 
     - name: message
       debug:
```

## ascend_deployer/playbooks/install/task_driver_bcinux.yml

```diff
@@ -182,21 +182,19 @@
   debug:
     msg:
       - "[ASCEND]can not find driver package, driver install skipped"
   when: driver_run is undefined and driver_pro_run is undefined
 
 - name: message
   debug:
-    msg:
-      - "{{ driver_result | default('NOT DEFINED') }}"
+    var: driver_result
   when: driver_result.changed
 
 - name: message
   debug:
-    msg:
-      - "{{ driver_up_result | default('NOT DEFINED') }}"
+    msg: driver_up_result
   when: driver_up_result.changed
 
 - name: service host_sys_init start
   shell: service host_sys_init start
   failed_when: false
   when: (driver_result.changed) or (driver_up_result.changed)
```

## ascend_deployer/playbooks/install/task_driver_common.yml

```diff
@@ -182,21 +182,19 @@
   debug:
     msg:
       - "[ASCEND]can not find driver package, driver install skipped"
   when: driver_run is undefined and driver_pro_run is undefined
 
 - name: message
   debug:
-    msg:
-      - "{{ driver_result | default('NOT DEFINED') }}"
+    var: driver_result
   when: driver_result.changed
 
 - name: message
   debug:
-    msg:
-      - "{{ driver_up_result | default('NOT DEFINED') }}"
+    var: driver_up_result
   when: driver_up_result.changed
 
 - name: service host_sys_init start
   shell: service host_sys_init start
   failed_when: false
   when: (driver_result.changed) or (driver_up_result.changed)
```

## ascend_deployer/playbooks/install/task_firmware.yml

```diff
@@ -170,16 +170,14 @@
   debug:
     msg:
       - "[ASCEND]can not find firmware package, firmware install skipped"
   when: firmware_run is undefined and firmware_pro_run is undefined
 
 - name: message
   debug:
-    msg:
-      - "{{ firmware_result | default('NOT DEFINED') }}"
+    var: firmware_result
   when: firmware_result.changed
 
 - name: message
   debug:
-    msg:
-      - "{{ firmware_up_result | default('NOT DEFINED') }}"
+    var: firmware_up_result
   when: firmware_up_result.changed
```

## ascend_deployer/playbooks/install/task_ha.yml

 * *Ordering differences only*

```diff
@@ -14,25 +14,25 @@
 
 - name: install ha
   shell: "bash {{ ha.files[0].path }}/install.sh -f -p /usr/local/"
   register: ha_result
   when: ha.matched is defined and ha.matched > 0
   failed_when: "ha_result.rc !=0 and 'has been installed' not in ha_result.stdout"
 
-- name: fail if not success
-  fail:
-    status: 3
-  when: "ha_result.rc !=0 or 'has been installed' not in ha_result.stdout and 'ha' in ansible_run_tags"
-
 - name: ha scene message
   debug:
     msg:
       - "[ASCEND]scene is not infer or server is not A500 Pro, ha install skipped"
   when: ha.matched is undefined
 
+- name: fail if not success
+  fail:
+    status: 3
+  when: "ha_result.rc !=0 or 'has been installed' not in ha_result.stdout and 'ha' in ansible_run_tags"
+
 - name: ha message
   debug:
     msg:
       - "[ASCEND]can not find ha package, ha install skipped"
   when: ha.matched is defined and ha.matched == 0
 
 - name: ha install message
```

## ascend_deployer/playbooks/install/task_ief_a500.yml

```diff
@@ -91,10 +91,9 @@
   shell: ./register --mode=cert
   args:
     chdir: /opt/edge-register
   register: ief_result
 
 - name: ief register message
   debug:
-    msg:
-      - "{{ ief_result }}"
+    var: ief_result
   when: ief_result.changed
```

## ascend_deployer/playbooks/install/task_ief_a500pro.yml

```diff
@@ -62,10 +62,9 @@
   shell: ./register --mode=cert
   args:
     chdir: /opt/edge-register
   register: ief_result
 
 - name: ief register message
   debug:
-    msg:
-      - "{{ ief_result }}"
+    var: ief_result
   when: ief_result.changed
```

## ascend_deployer/playbooks/install/task_kernel.yml

```diff
@@ -1,48 +1,41 @@
 - name: check kernel headers
   shell: rpm -q kernel-headers | grep {{ ansible_kernel }} | wc -l
   register: kh_cnt
   changed_when: false
 
-- name: find kernel headers rpm
-  find:
-    path: "{{ resources_dir }}"
-    recurse: yes
-    file_type: file
-    use_regex: yes
-    patterns: "kernel-headers-{{ ansible_kernel }}.rpm"
-  register: kh_rpm
-  when: kh_cnt.stdout == "0"
-
-- name: install kernel headers rpm
-  shell: rpm -ivh --force --nodeps --replacepkgs {{ kh_rpm.files[0].path }}
-  when: kh_cnt.stdout == "0" and kh_rpm.matched > 0
-  failed_when: false
+- name: install kernel headers yum
+  shell: |
+    yum clean all &>/dev/null
+    yum makecache --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo &>/dev/null
+    yum install --skip-broken -y kernel-headers-{{ ansible_kernel }} --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo
   register: kernel_headers_result
+  environment:
+    LD_LIBRARY_PATH: ""
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when: kh_cnt.stdout == "0"
 
 - name: check kernel devel
   shell: rpm -q kernel-devel | grep {{ ansible_kernel }} | wc -l
   register: kd_cnt
   changed_when: false
 
-- name: find kernel devel rpm
-  find:
-    path: "{{ resources_dir }}"
-    recurse: yes
-    file_type: file
-    use_regex: yes
-    patterns: "kernel-devel-{{ ansible_kernel }}.rpm"
-  register: kd_rpm
-  when: kd_cnt.stdout == "0"
-
-- name: install kernel devel rpm
-  shell: rpm -ivh --force --nodeps --replacepkgs {{ kd_rpm.files[0].path }}
-  when: kd_cnt.stdout == "0" and kd_rpm.matched > 0
-  failed_when: false
+- name: install kernel devel yum
+  shell: |
+    yum makecache --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo &>/dev/null
+    yum install --skip-broken -y kernel-devel-{{ ansible_kernel }} --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo
   register: kernel_devel_result
+  environment:
+    LD_LIBRARY_PATH: ""
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when: kd_cnt.stdout == "0"
 
 - name: message
   debug:
-    msg:
-      - "{{ kernel_headers_result | default('NOT DEFINED') }}"
-      - "{{ kernel_devel_result | default('NOT DEFINED') }}"
+    var: kernel_headers_result,kernel_devel_result
   when: kernel_headers_result.changed or kernel_devel_result.changed
```

## ascend_deployer/playbooks/install/task_kernel_euleros.yml

```diff
@@ -1,38 +1,41 @@
 - name: check kernel headers
   shell: rpm -qa kernel-headers | wc -l
   register: kh_cnt
   changed_when: false
 
-- name: find kernel headers rpm
-  shell: "find {{ resources_dir }}/kernel/ -name 'kernel-headers*' | sort -r | grep -m1 {{ euleros_kernel_flag }} | wc -l"
-  register: kh_rpm
-  when: kh_cnt.stdout == "0"
-
-- name: install kernel headers rpm
-  shell: rpm -ivh --force --nodeps --replacepkgs {{ resources_dir }}/kernel/kernel-headers*
-  when: kh_cnt.stdout == "0" and kh_rpm.stdout != "0"
-  failed_when: false
+- name: install kernel headers yum
+  shell: |
+    yum clean all &>/dev/null
+    yum makecache --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo &>/dev/null
+    yum install --skip-broken -y kernel-headers --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo
   register: kernel_headers_result
+  environment:
+    LD_LIBRARY_PATH: ""
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when: kh_cnt.stdout == "0"
 
 - name: check kernel devel
   shell: rpm -qa kernel-devel | wc -l
   register: kd_cnt
   changed_when: false
 
-- name: find kernel devel rpm
-  shell: "find {{ resources_dir }}/kernel/ -name 'kernel-devel*' | sort -r | grep -m1 {{ euleros_kernel_flag }} | wc -l"
-  register: kd_rpm
-  when: kd_cnt.stdout == "0"
-
-- name: install kernel devel rpm
-  shell: rpm -ivh --force --nodeps --replacepkgs {{ resources_dir }}/kernel/kernel-devel*
-  when: kd_cnt.stdout == "0" and kd_rpm.stdout != "0"
-  failed_when: false
+- name: install kernel devel yum
+  shell: |
+    yum makecache --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo &>/dev/null
+    yum install --skip-broken -y kernel-devel --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo
   register: kernel_devel_result
+  environment:
+    LD_LIBRARY_PATH: ""
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when: kd_cnt.stdout == "0"
 
 - name: message
   debug:
-    msg:
-      - "{{ kernel_headers_result | default('NOT DEFINED') }}"
-      - "{{ kernel_devel_result | default('NOT DEFINED') }}"
+    var: kernel_headers_result, kernel_devel_result
   when: kernel_headers_result.changed or kernel_devel_result.changed
```

## ascend_deployer/playbooks/install/task_kernels.yml

```diff
@@ -123,25 +123,25 @@
 
 - name: message
   debug:
     msg:
       - "[ASCEND]The nnae and toolkit packages are not installed, kernels install skipped"
   when: kernels_version != 'NA' and toolkit_status.matched == 0 and nnae_status.matched == 0
 
-- name: check whether to fail for scene
-  fail:
-    msg: "end the task"
-  when: "'kernels' in ansible_run_tags and kernels_version != 'NA' and toolkit_status.matched == 0 and nnae_status.matched == 0"
-
 - name: message for no packages
   debug:
     msg:
       - "[ASCEND]can not find kernels packages, kernels install skipped"
   when: kernels_310P_run.matched == 0 and kernels_910_run.matched == 0 and kernels_910b_run.matched == 0 or ansible_local.npu_info.scene == 'infer'
 
+- name: check whether to fail for scene
+  fail:
+    msg: "end the task"
+  when: "'kernels' in ansible_run_tags and kernels_version != 'NA' and toolkit_status.matched == 0 and nnae_status.matched == 0"
+
 - name: check if should terminal
   fail:
     msg:
       - "end the task_kernels"
   when:
     - "'kernels' in ansible_run_tags"
     - kernels_310P_run.matched == 0 and (ansible_local.npu_info.scene == 'a300i' or ansible_local.npu_info.scene == 'a300iduo') or kernels_910_run.matched == 0 and ansible_local.npu_info.scene == 'train' or kernels_910b_run.matched == 0 and ansible_local.npu_info.scene == 'a910b' or ansible_local.npu_info.scene == 'infer'
@@ -155,106 +155,100 @@
   shell: "bash {{ kernels_310P.files[0].path }} {{ log_path }} {{ kernels_type }}"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: kernels_310P_result
   when:
     - kernels_310P.matched > 0
-    - toolkit_status.matched > 0 or nnae_status.matched > 0
+    - (toolkit_status.matched is defined and toolkit_status.matched > 0) or (nnae_status.matched is defined and nnae_status.matched > 0)
     - ansible_local.npu_info.scene == 'a300i' or ansible_local.npu_info.scene == 'a300iduo'
   failed_when: kernels_310P_result.rc != 0
 
 - name: message for 310P
   debug:
-    msg:
-      - "{{ kernels_310P_result | default('NOT DEFINED') }}"
+    var: kernels_310P_result
   when: kernels_310P_result.changed
 
 - name: install kernels for 310P
   shell: "bash {{ kernels_310P_run.files[0].path }} --install --type={{ kernels_type }}"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: kernels_310P_run_result
   when:
     - kernels_310P_run.matched > 0 and kernels_310P.matched == 0
-    - toolkit_status.matched > 0 or nnae_status.matched > 0
+    - (toolkit_status.matched is defined and toolkit_status.matched > 0) or (nnae_status.matched is defined and nnae_status.matched > 0)
     - ansible_local.npu_info.scene == 'a300i' or ansible_local.npu_info.scene == 'a300iduo'
   failed_when: kernels_310P_run_result.rc != 0
 
 - name: message for 310P
   debug:
-    msg:
-      - "{{ kernels_310P_run_result | default('NOT DEFINED') }}"
+    var: kernels_310P_run_result
   when: kernels_310P_run_result.changed
 
 - name: install kernels using scripts for 910
   shell: "bash {{ kernels_910.files[0].path }} {{ log_path }} {{ kernels_type }}"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: kernels_910_result
   when:
     - kernels_910.matched > 0
-    - toolkit_status.matched > 0 or nnae_status.matched > 0
+    - (toolkit_status.matched is defined and toolkit_status.matched > 0) or (nnae_status.matched is defined and nnae_status.matched > 0)
     - ansible_local.npu_info.scene == 'train'
   failed_when: kernels_910_result.rc != 0
 
 - name: message for 910
   debug:
-    msg:
-      - "{{ kernels_910_result | default('NOT DEFINED') }}"
+    var: kernels_910_result
   when: kernels_910_result.changed and ansible_local.npu_info.scene == 'train'
 
 - name: install kernels for 910
   shell: "bash {{ kernels_910_run.files[0].path }} --install --type={{ kernels_type }}"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: kernels_910_run_result
   when:
     - kernels_910_run.matched > 0 and kernels_910.matched == 0
-    - toolkit_status.matched > 0 or nnae_status.matched > 0
+    - (toolkit_status.matched is defined and toolkit_status.matched > 0) or (nnae_status.matched is defined and nnae_status.matched > 0)
     - ansible_local.npu_info.scene == 'train'
   failed_when: kernels_910_run_result.rc != 0
 
 - name: message for 910
   debug:
-    msg:
-      - "{{ kernels_910_run_result | default('NOT DEFINED') }}"
+    var: kernels_910_run_result
   when: kernels_910_run_result.changed and ansible_local.npu_info.scene == 'train'
 
 - name: install kernels using scripts for 910b
   shell: "bash {{ kernels_910b.files[0].path }} {{ log_path }} {{ kernels_type }}"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: kernels_910b_result
   when:
     - kernels_910b.matched > 0
-    - toolkit_status.matched > 0 or nnae_status.matched > 0
+    - (toolkit_status.matched is defined and toolkit_status.matched > 0) or (nnae_status.matched is defined and nnae_status.matched > 0)
     - ansible_local.npu_info.scene == 'a910b'
   failed_when: kernels_910b_result.rc != 0
 
 - name: message for 910b
   debug:
-    msg:
-      - "{{ kernels_910b_result | default('NOT DEFINED') }}"
+    var: kernels_910b_result
   when: kernels_910b_result.changed and ansible_local.npu_info.scene == 'a910b'
 
 - name: install kernels for 910b
   shell: "bash {{ kernels_910b_run.files[0].path }} --install --type={{ kernels_type }}"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: kernels_910b_run_result
   when:
     - kernels_910b_run.matched > 0 and kernels_910.matched == 0
-    - toolkit_status.matched > 0 or nnae_status.matched > 0
+    - (toolkit_status.matched is defined and toolkit_status.matched > 0) or (nnae_status.matched is defined and nnae_status.matched > 0)
     - ansible_local.npu_info.scene == 'a910b'
   failed_when: kernels_910b_run_result.rc != 0
 
 - name: message for 910b
   debug:
-    msg:
-      - "{{ kernels_910b_run_result | default('NOT DEFINED') }}"
+    var: kernels_910b_run_result
   when: kernels_910b_run_result.changed and ansible_local.npu_info.scene == 'a910b'
```

## ascend_deployer/playbooks/install/task_mindspore.yml

```diff
@@ -32,20 +32,24 @@
   shell: python3 -m pip install {{ mindspore_whl_cpu.files[0].path }} --no-index --find-links {{ resources_dir }}/pylibs {{ pip_install_option }}
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ local_path }}/gcc7.3.0/lib64"
   when:
     - mindspore_whl_cpu.matched is defined and mindspore_whl_cpu.matched > 0
 
-- name: fail if this install
-  fail:
-    status: 3
-  when: "'mindspore' in ansible_run_tags and mindspore_whl_ascend.skipped and mindspore_whl_cpu.skipped"
-
 - name: message
   debug:
     msg:
       - "[ASCEND]os: {{ os_and_arch }}, scene: {{ ansible_local.npu_info.scene }}, mindspore install skipped"
       - "maybe you should check mindspore whl package in dir: ascend-deployer/resources/{{ os_and_arch }}/Ascend(or CPU)/"
   when:
-    - mindspore_whl_ascend.skipped is true
-    - mindspore_whl_cpu.skipped is true
+    - mindspore_whl_ascend.skipped is defined
+    - mindspore_whl_cpu.skipped is defined
+
+- name: fail if this install
+  fail:
+    status: 3
+  when:
+    - mindspore_whl_ascend.skipped is defined
+    - mindspore_whl_cpu.skipped is defined
+    - "'mindspore' in ansible_run_tags"
+
```

## ascend_deployer/playbooks/install/task_nnae.yml

```diff
@@ -40,16 +40,15 @@
   when:
     - nnae.matched > 0
     - ansible_local.npu_info.scene != 'a910b' or nnae_version.stdout != '6.3.RC1' and ansible_local.npu_info.scene == 'a910b'
   failed_when: "nnae_result.rc != 0 and 'already installed' not in nnae_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ nnae_result | default('NOT DEFINED') }}"
+    var: nnae_result
   when: nnae_result.changed
 
 - name: check ascend cann install info
   stat:
     path: "{{ cann_info_path }}/ascend_cann_install.info"
   register: install_info
 
@@ -76,16 +75,15 @@
   when:
     - nnae.matched == 0 and nnae_run.matched > 0 and nnae_status.stdout == '0'
     - ansible_local.npu_info.scene != 'a910b' or nnae_version.stdout != '6.3.RC1' and ansible_local.npu_info.scene == 'a910b'
   failed_when: "nnae_result.rc != 0 and 'already installed' not in nnae_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ nnae_result | default('NOT DEFINED') }}"
+    var: nnae_result
   when: nnae.matched == 0 and nnae_result.changed and nnae_status.stdout == '0'
 
 - name: upgrade nnae
   shell: "bash {{ nnae_run.files[0].path }} --nox11 --upgrade"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
@@ -93,16 +91,15 @@
   when:
     - nnae.matched == 0 and nnae_run.matched > 0 and nnae_status.stdout != '0'
     - ansible_local.npu_info.scene != 'a910b' or nnae_version.stdout != '6.3.RC1' and ansible_local.npu_info.scene == 'a910b'
   failed_when: "nnae_result.rc != 0 and 'already installed' not in nnae_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ nnae_result | default('NOT DEFINED') }}"
+    var: nnae_result
   when: nnae.matched == 0 and nnae_result.changed and nnae_status.stdout != '0'
 
 - name: fail if this install
   fail:
     status: 3
   when:
     - "'nnae' in ansible_run_tags"
```

## ascend_deployer/playbooks/install/task_nnrt.yml

```diff
@@ -40,16 +40,15 @@
   when:
     - nnrt.matched > 0
     - ansible_local.npu_info.scene != 'a910b' or nnrt_version.stdout != '6.3.RC1' and ansible_local.npu_info.scene == 'a910b'
   failed_when: "nnrt_result.rc != 0 and 'already installed' not in nnrt_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ nnrt_result | default('NOT DEFINED') }}"
+    var: nnrt_result
   when: nnrt_result.changed
 
 - name: check ascend cann install info
   stat:
     path: "{{ cann_info_path }}/ascend_cann_install.info"
   register: install_info
 
@@ -76,16 +75,15 @@
   when:
     - nnrt.matched == 0 and nnrt_run.matched > 0 and nnrt_status.stdout == '0'
     - ansible_local.npu_info.scene != 'a910b' or nnrt_version.stdout != '6.3.RC1' and ansible_local.npu_info.scene == 'a910b'
   failed_when: "nnrt_result.rc != 0 and 'already installed' not in nnrt_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ nnrt_result | default('NOT DEFINED') }}"
+    var: nnrt_result
   when: nnrt.matched == 0 and nnrt_result.changed and nnrt_status.stdout == '0'
 
 - name: upgrade nnrt
   shell: "bash {{ nnrt_run.files[0].path }} --nox11 --upgrade"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
@@ -93,23 +91,23 @@
   when:
    - nnrt.matched == 0 and nnrt_run.matched > 0 and nnrt_status.stdout != '0'
    - ansible_local.npu_info.scene != 'a910b' or nnrt_version.stdout != '6.3.RC1' and ansible_local.npu_info.scene == 'a910b'
   failed_when: "nnrt_result.rc != 0 and 'already installed' not in nnrt_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ nnrt_result | default('NOT DEFINED') }}"
+    var: nnrt_result
   when: nnrt.matched == 0 and nnrt_result.changed and nnrt_status.stdout != '0'
 
+- name: message
+  debug:
+    msg:
+      - "[ASCEND]can not find nnrt package, nnrt install skipped"
+  when: nnrt_run.matched == 0 or (nnrt_run.matched > 0 and nnrt_version.stdout == '6.3.RC1' and ansible_local.npu_info.scene == 'a910b')
+
 - name: fail if this install
   fail:
     status: 3
   when:
     - "'nnrt' in ansible_run_tags"
     - nnrt_run.matched == 0 or (nnrt_run.matched > 0 and nnrt_version.stdout == '6.3.RC1' and ansible_local.npu_info.scene == 'a910b')
 
-- name: message
-  debug:
-    msg:
-      - "[ASCEND]can not find nnrt package, nnrt install skipped"
-  when: nnrt_run.matched == 0 or (nnrt_run.matched > 0 and nnrt_version.stdout == '6.3.RC1' and ansible_local.npu_info.scene == 'a910b')
```

## ascend_deployer/playbooks/install/task_sys_apt.yml

```diff
@@ -21,16 +21,15 @@
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
   when:
     - ansible_pkg_mgr != 'apt'
 
 - name: message
   debug:
-    msg:
-      - "{{ sys_result | default('NOT DEFINED') }}"
+    var: sys_result
   when: ansible_pkg_mgr != 'apt' and sys_result.changed
 
 - name: check if Docker is installed
   shell: command -v docker | wc -l
   register: docker_status
   when:
     - ansible_pkg_mgr != 'apt'
@@ -60,10 +59,9 @@
     dpkg --force-all -i {{ resources_dir }}/{{ os_and_arch }}/docker/*.deb
   when:
     - ansible_pkg_mgr == 'apt'
   register: sys_result
 
 - name: message
   debug:
-    msg:
-      - "{{ sys_result | default('NOT DEFINED') }}"
+    var: sys_result
   when: sys_result.changed or sys_result_linx.changed
```

## ascend_deployer/playbooks/install/task_sys_dnf.yml

```diff
@@ -1,7 +1,23 @@
+- name: check index status
+  shell: |
+    timeout=0
+    while true;do
+        if [ $(docker logs nexus | grep 'Finished .* {{os_and_arch}}' | wc -l) -eq 1 ];then
+            break
+        else
+            sleep 1
+            ((++timeout))
+            if [ $timeout -eq 120 ];then
+                echo "install sys_pkgs failed" && exit 1
+            fi
+        fi
+    done
+  delegate_to: localhost
+
 - name: install kernel headers devel
   include_tasks: task_kernel.yml
   when: "'EulerOS' in os_and_arch"
 
 - name: install kernel headers devel force for euler
   include_tasks: task_kernel_euleros.yml
   when: "'EulerOS' in os_and_arch"
@@ -14,52 +30,52 @@
   register: sys_result
   environment:
     LD_LIBRARY_PATH: ""
     http_proxy: ""
     https_proxy: ""
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
-  when: "'OpenEuler' in os_and_arch or 'Kylin_V10Tercel' in os_and_arch"
+  when: "'CentOS_7.6' not in os_and_arch"
 
 - name: message
   debug: var=sys_result
   when:
-    - "'OpenEuler' in os_and_arch or 'Kylin_V10Tercel' in os_and_arch"
+    - "'CentOS_7.6' not in os_and_arch"
     - sys_result.changed
 
 - name: check if Docker is installed
   shell: command -v docker | wc -l
   register: docker_status
-  when: "'OpenEuler' in os_and_arch or 'Kylin_V10Tercel' in os_and_arch"
+  when: "'CentOS_7.6' not in os_and_arch"
 
 - name: install Docker when Docker is not installed
   shell: |
     yum install -y --skip-broken {{docker_pkgs}} --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo
   register: docker_result
   environment:
     LD_LIBRARY_PATH: ""
     http_proxy: ""
     https_proxy: ""
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
   when:
-    - "'OpenEuler' in os_and_arch or 'Kylin_V10Tercel' in os_and_arch"
+    - "'CentOS_7.6' not in os_and_arch"
     - docker_status.stdout == "0"
 
 - name: message
   debug: var=docker_result
   when:
-    - "'OpenEuler' in os_and_arch or 'Kylin_V10Tercel' in os_and_arch"
+    - "'CentOS_7.6' not in os_and_arch"
     - docker_result.changed
 
 - name: dnf install system packages
   shell: |
     rpm -ivh --force --nodeps --replacepkgs {{ resources_dir }}/{{ os_and_arch }}/*.rpm
     rpm -ivh --force --nodeps --replacepkgs {{ resources_dir }}/{{ os_and_arch }}/docker/*.rpm
   register: sys_result
-  when: "'OpenEuler' not in os_and_arch and 'Kylin_V10Tercel' not in os_and_arch"
+  when: "'CentOS_7.6' in os_and_arch"
 
 - name: message
   debug: var=sys_result
   when:
-    - "'OpenEuler' not in os_and_arch and 'Kylin_V10Tercel' not in os_and_arch"
+    - "'CentOS_7.6' in os_and_arch"
     - sys_result.changed
```

## ascend_deployer/playbooks/install/task_sys_yum.yml

```diff
@@ -1,7 +1,23 @@
+- name: check index status
+  shell: |
+    timeout=0
+    while true;do
+        if [ $(docker logs nexus | grep 'Finished .* {{os_and_arch}}' | wc -l) -eq 1 ];then
+            break
+        else
+            sleep 1
+            ((++timeout))
+            if [ $timeout -eq 120 ];then
+                echo "install sys_pkgs failed" && exit 1
+            fi
+        fi
+    done
+  delegate_to: localhost
+
 - name: install kernel headers devel
   include_tasks: task_kernel.yml
   when: "'EulerOS' in os_and_arch"
 
 - name: install kernel headers devel force for euler
   include_tasks: task_kernel_euleros.yml
   when: "'EulerOS' in os_and_arch"
@@ -14,52 +30,52 @@
   register: sys_result
   environment:
     LD_LIBRARY_PATH: ""
     http_proxy: ""
     https_proxy: ""
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
-  when: "'OpenEuler' in os_and_arch or 'Kylin_V10Tercel' in os_and_arch"
+  when: "'CentOS_7.6' not in os_and_arch"
 
 - name: message
   debug: var=sys_result
   when:
-    - "'OpenEuler' in os_and_arch or 'Kylin_V10Tercel' in os_and_arch"
+    - "'CentOS_7.6' not in os_and_arch"
     - sys_result.changed
 
 - name: check if Docker is installed
   shell: command -v docker | wc -l
   register: docker_status
-  when: "'OpenEuler' in os_and_arch or 'Kylin_V10Tercel' in os_and_arch"
+  when: "'CentOS_7.6' not in os_and_arch"
 
 - name: install Docker when Docker is not installed
   shell: |
     yum install -y --skip-broken {{docker_pkgs}} --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo
   register: docker_result
   environment:
     LD_LIBRARY_PATH: ""
     http_proxy: ""
     https_proxy: ""
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
   when:
-    - "'OpenEuler' in os_and_arch or 'Kylin_V10Tercel' in os_and_arch"
+    - "'CentOS_7.6' not in os_and_arch"
     - docker_status.stdout == "0"
 
 - name: message
   debug: var=docker_result
   when:
-    - "'OpenEuler' in os_and_arch or 'Kylin_V10Tercel' in os_and_arch"
+    - "'CentOS_7.6' not in os_and_arch"
     - docker_result.changed
 
 - name: yum install system packages
   shell: |
     rpm -ivh --force --nodeps --replacepkgs {{ resources_dir }}/{{ os_and_arch }}/*.rpm
     rpm -ivh --force --nodeps --replacepkgs {{ resources_dir }}/{{ os_and_arch }}/docker/*.rpm
   register: sys_result
-  when: "'OpenEuler' not in os_and_arch and 'Kylin_V10Tercel' not in os_and_arch"
+  when: "'CentOS_7.6' in os_and_arch"
 
 - name: message
   debug: var=sys_result
   when:
-    - "'OpenEuler' not in os_and_arch and 'Kylin_V10Tercel' not in os_and_arch"
+    - "'CentOS_7.6' in os_and_arch"
     - sys_result.changed
```

## ascend_deployer/playbooks/install/task_tfplugin.yml

```diff
@@ -40,16 +40,15 @@
   when:
     - tfplugin.matched > 0
     - ansible_local.npu_info.scene != 'a910b' or ansible_local.npu_info.scene == 'a910b' and tfplugin_version.stdout != '6.3.RC1'
   failed_when: "tfplugin_result.rc !=0 and 'already installed' not in tfplugin_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ tfplugin_result | default('NOT DEFINED') }}"
+    var: tfplugin_result
   when: tfplugin_result.changed
 
 - name: check ascend cann install info
   stat:
     path: "{{ cann_info_path }}/ascend_cann_install.info"
   register: install_info
 
@@ -76,16 +75,15 @@
   when:
     - tfplugin.matched == 0 and tfplugin_run.matched > 0 and tfplugin_status.stdout == '0'
     - ansible_local.npu_info.scene != 'a910b' or ansible_local.npu_info.scene == 'a910b' and tfplugin_version.stdout != '6.3.RC1'
   failed_when: "tfplugin_result.rc !=0 and 'already installed' not in tfplugin_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ tfplugin_result | default('NOT DEFINED') }}"
+    var: tfplugin_result
   when: tfplugin.matched == 0 and tfplugin_result.changed and tfplugin_status.stdout == '0'
 
 - name: upgrade tfplugin
   shell: "bash {{ tfplugin_run.files[0].path }} --nox11 --upgrade"
   environment:
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
@@ -93,16 +91,15 @@
   when:
     - tfplugin.matched == 0 and tfplugin_run.matched > 0 and tfplugin_status.stdout != '0'
     - ansible_local.npu_info.scene != 'a910b' or ansible_local.npu_info.scene == 'a910b' and tfplugin_version.stdout != '6.3.RC1'
   failed_when: "tfplugin_result.rc !=0 and 'already installed' not in tfplugin_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ tfplugin_result | default('NOT DEFINED') }}"
+    var: tfplugin_result
   when: tfplugin.matched == 0 and tfplugin_result.changed and tfplugin_status.stdout != '0'
 
 - name: fail if not success
   fail:
     status: 3
   when:
     - "'tfplugin' in ansible_run_tags"
```

## ascend_deployer/playbooks/install/task_toolbox.yml

```diff
@@ -30,28 +30,26 @@
   shell: "export TOOLBOX_SOC=A200ISoC && bash {{ toolbox.files[0].path }} {{ log_path }}"
   register: toolbox_result
   when: toolbox.matched > 0 and ansible_local.npu_info.model == "Atlas 200I SoC A1"
   failed_when: "toolbox_result.rc != 0 and 'already installed' not in toolbox_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ toolbox_result | default('NOT DEFINED') }}"
+    var: toolbox_result
   when: toolbox_result.changed and ansible_local.npu_info.model == "Atlas 200I SoC A1"
 
 - name: install toolbox
   shell: "bash {{ toolbox.files[0].path }} {{ log_path }}"
   register: toolbox_result
   when: toolbox.matched > 0 and ansible_local.npu_info.model != "Atlas 200I SoC A1"
   failed_when: "toolbox_result.rc != 0 and 'already installed' not in toolbox_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ toolbox_result | default('NOT DEFINED') }}"
+    var: toolbox_result
   when: toolbox_result.changed and ansible_local.npu_info.model != "Atlas 200I SoC A1"
 
 - name: check ascend cann install info
   stat:
     path: "{{ cann_info_path }}/ascend_cann_install.info"
   register: install_info
 
@@ -77,33 +75,31 @@
   shell: "bash {{ toolbox_run.files[0].path }} --nox11 {{ cann_install_params }} {{ins_path_cmd}}"
   register: toolbox_result
   when: toolbox.matched == 0 and toolbox_run.matched > 0 and (not toolbox_info.stat.exists)
   failed_when: "toolbox_result.rc != 0 and 'already installed' not in toolbox_result.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ toolbox_result | default('NOT DEFINED') }}"
+    var: toolbox_result
   when: toolbox.matched == 0 and toolbox_result.changed
 
 - name: upgrade toolbox
   shell: "bash {{ toolbox_run.files[0].path }} --nox11 --upgrade --quiet {{ins_path_cmd}}"
   register: toolbox_result
   when: toolbox.matched == 0 and toolbox_run.matched > 0 and toolbox_info.stat.exists
   failed_when: "toolbox_result.rc != 0 and 'already installed' not in toolbox_result.stdout"
 
-- name: fail if not success
-  fail:
-    status: 3
-  when: "toolbox_run.matched == 0 and 'toolbox' in ansible_run_tags"
-
 - name: message
   debug:
     msg:
       - "[ASCEND]can not find toolbox package, toolbox install skipped"
   when: toolbox_run.matched == 0
 
+- name: fail if not success
+  fail:
+    status: 3
+  when: "toolbox_run.matched == 0 and 'toolbox' in ansible_run_tags"
+
 - name: message
   debug:
-    msg:
-      - "{{ toolbox_result | default('NOT DEFINED') }}"
+    var: toolbox_result
   when: toolbox.matched == 0 and toolbox_result.changed
```

## ascend_deployer/playbooks/install/task_toolkit.yml

```diff
@@ -77,17 +77,15 @@
     - os_and_arch == 'Ubuntu_18.04_x86_64' or os_and_arch == 'Ubuntu_20.04_x86_64'
     - toolkit_aarch64.matched is defined and toolkit_aarch64.matched > 0
     - ansible_local.npu_info.scene != 'a910b' or toolkit_aarch64_version.stdout != '6.3.RC1' and ansible_local.npu_info.scene == 'a910b'
   failed_when: "toolkit_result_ubuntu.rc != 0 and 'already installed' not in toolkit_result_ubuntu.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ toolkit_result | default('NOT DEFINED') }}"
-      - "{{ toolkit_result_ubuntu | default('NOT DEFINED') }}"
+    var: toolkit_result,toolkit_result_ubuntu
   when: toolkit_result.changed or toolkit_result_ubuntu.changed
 
 - name: check ascend cann install info
   stat:
     path: "{{ cann_info_path }}/ascend_cann_install.info"
   register: install_info
 
@@ -126,17 +124,15 @@
     - toolkit_aarch64_run.matched is defined and toolkit_aarch64_run.matched > 0 and toolkit_status.stdout == '0'
     - toolkit_aarch64.matched == 0 and (os_and_arch == 'Ubuntu_18.04_x86_64' or os_and_arch == 'Ubuntu_20.04_x86_64')
     - ansible_local.npu_info.scene != 'a910b' or toolkit_aarch64_version.stdout != '6.3.RC1' and ansible_local.npu_info.scene == 'a910b'
   failed_when: "toolkit_result_ubuntu.rc != 0 and 'already installed' not in toolkit_result_ubuntu.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ toolkit_result | default('NOT DEFINED') }}"
-      - "{{ toolkit_result_ubuntu | default('NOT DEFINED') }}"
+    var: toolkit_result,toolkit_result_ubuntu
   when: toolkit.matched == 0 and (toolkit_result.changed or toolkit_result_ubuntu.changed) and toolkit_status.stdout == '0'
 
 - name: upgrade toolkit
   shell: "bash {{ toolkit_run.files[0].path }} --nox11 --upgrade"
   environment:
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
@@ -156,17 +152,15 @@
     - toolkit_aarch64_run.matched is defined and toolkit_aarch64_run.matched > 0 and toolkit_status.stdout != '0'
     - toolkit_aarch64.matched == 0 and (os_and_arch == 'Ubuntu_18.04_x86_64' or os_and_arch == 'Ubuntu_20.04_x86_64')
     - ansible_local.npu_info.scene != 'a910b' or toolkit_aarch64_version.stdout != '6.3.RC1' and ansible_local.npu_info.scene == 'a910b'
   failed_when: "toolkit_result_ubuntu.rc != 0 and 'already installed' not in toolkit_result_ubuntu.stdout"
 
 - name: message
   debug:
-    msg:
-      - "{{ toolkit_result | default('NOT DEFINED') }}"
-      - "{{ toolkit_result_ubuntu | default('NOT DEFINED') }}"
+    var: toolkit_result,toolkit_result_ubuntu
   when: toolkit.matched == 0 and (toolkit_result.changed or toolkit_result_ubuntu.changed) and toolkit_status.stdout != '0'
 
 - name: fail if not success
   fail:
     status: 3
   when:
     - "'toolkit' in ansible_run_tags"
```

## ascend_deployer/playbooks/install/patch/task_nnae.yml

```diff
@@ -27,23 +27,22 @@
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: nnae_result
   when: nnae.matched > 0
   failed_when: "nnae_result.rc != 0 and 'already installed' not in nnae_result.stdout"
 
-- name: fail if this rollback
-  fail:
-    status: 3
-  when: "'nnae' in ansible_run_tags and nnae.matched == 0"
-
 - name: message
   debug:
     msg:
       - "[ASCEND]can not find nnae patch package, nnae patch install skipped"
   when: nnae.matched == 0
 
+- name: fail if this rollback
+  fail:
+    status: 3
+  when: "'nnae' in ansible_run_tags and nnae.matched == 0"
+
 - name: message
   debug:
-    msg:
-      - "{{ nnae_result | default('NOT DEFINED') }}"
+    var: nnae_result
   when: nnae_result.changed
```

## ascend_deployer/playbooks/install/patch/task_nnrt.yml

```diff
@@ -27,23 +27,22 @@
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: nnrt_result
   when: nnrt.matched > 0
   failed_when: "nnrt_result.rc != 0 and 'already installed' not in nnrt_result.stdout"
 
-- name: fail if this rollback
-  fail:
-    status: 3
-  when: "'nnrt' in ansible_run_tags and nnrt.matched == 0"
-
 - name: message
   debug:
     msg:
       - "[ASCEND]can not find nnrt patch package, nnrt patch install skipped"
   when: nnrt.matched == 0
 
+- name: fail if this rollback
+  fail:
+    status: 3
+  when: "'nnrt' in ansible_run_tags and nnrt.matched == 0"
+
 - name: message
   debug:
-    msg:
-      - "{{ nnrt_result | default('NOT DEFINED') }}"
+    var: nnrt_result
   when: nnrt_result.changed
```

## ascend_deployer/playbooks/install/patch/task_rollback_nnae.yml

```diff
@@ -8,23 +8,22 @@
   register: nnae
 
 - name: rollback nnae
   shell: "bash {{ nnae.files[0].path }} --rollback"
   register: nnae_result
   when: nnae.matched > 0
 
-- name: fail if this rollback
-  fail:
-    status: 3
-  when: "'nnae' in ansible_run_tags and nnae.matched == 0"
-
 - name: message
   debug:
     msg:
       - "[ASCEND]can not find nnae package, nnae rollback skipped"
   when: nnae.matched == 0
 
+- name: fail if this rollback
+  fail:
+    status: 3
+  when: "'nnae' in ansible_run_tags and nnae.matched == 0"
+
 - name: message
   debug:
-    msg:
-      - "{{ nnae_result | default('NOT DEFINED') }}"
+    var: nnae_result
   when: nnae_result.changed
```

## ascend_deployer/playbooks/install/patch/task_rollback_nnrt.yml

```diff
@@ -38,23 +38,23 @@
     - ansible_architecture == 'x86_64'
 
 - name: rollback nnrt for x86_64
   shell: "bash {{ nnrt_x64.files[0].path }} --rollback"
   register: nnrt_x64_result
   when: "ansible_architecture == 'x86_64' and nnrt_x64.matched > 0"
 
-- name: fail if this rollback
-  fail:
-    status: 3
-  when: "'nnrt' in ansible_run_tags and ansible_architecture == 'x86_64' and nnrt_x64.matched == 0"
-
 - name: message
   debug:
     msg:
       - "[ASCEND]can not find nnrt rollback script,nnrt rollback skipped"
-  when: "ansible_architecture == 'x86_64' and nnrt_x64.matched == 0"  
+  when: "ansible_architecture == 'x86_64' and nnrt_x64.matched == 0"
+
+- name: fail if this rollback
+  fail:
+    status: 3
+  when: "'nnrt' in ansible_run_tags and ansible_architecture == 'x86_64' and nnrt_x64.matched == 0"
 
 - name: message
   debug:
     msg:
       - "[ASCEND]{{ nnrt_x64_result | default('NOT DEFINED') }}"
   when: nnrt_x64_result.changed
```

## ascend_deployer/playbooks/install/patch/task_rollback_tfplugin.yml

```diff
@@ -8,23 +8,22 @@
   register: tfplugin
 
 - name: rollback tfplugin
   shell: "bash {{ tfplugin.files[0].path }} --rollback"
   register: tfplugin_result
   when: tfplugin.matched > 0
 
-- name: fail if this rollback
-  fail:
-    status: 3
-  when: "'tfplugin' in ansible_run_tags and tfplugin.matched == 0"
-
 - name: message
   debug:
     msg:
       - "[ASCEND]can not find tfplugin patch package,tfplugin rollback skipped"
   when: tfplugin.matched == 0
 
+- name: fail if this rollback
+  fail:
+    status: 3
+  when: "'tfplugin' in ansible_run_tags and tfplugin.matched == 0"
+
 - name: message
   debug:
-    msg:
-      - "{{ tfplugin_result | default('NOT DEFINED') }}"
+    var: tfplugin_result
   when: tfplugin_result.changed
```

## ascend_deployer/playbooks/install/patch/task_rollback_toolkit.yml

```diff
@@ -10,29 +10,28 @@
     - ansible_architecture == 'aarch64'
 
 - name: rollback toolkit for aarch64
   shell: "bash {{ toolkit_aarch64.files[0].path }} --rollback"
   register: toolkit_aarch64_result
   when: "ansible_architecture == 'aarch64' and toolkit_aarch64.matched > 0"
 
-- name: fail if this rollback
-  fail:
-    status: 3
-  when: "'toolkit' in ansible_run_tags and ansible_architecture == 'aarch64' and toolkit_aarch64.matched == 0"
-
 - name: message
   debug:
     msg:
       - "[ASCEND]can not find toolkit rollback script for aarch64,toolkit rollback skipped"
   when: "ansible_architecture == 'aarch64' and toolkit_aarch64.matched == 0"
 
+- name: fail if this rollback
+  fail:
+    status: 3
+  when: "'toolkit' in ansible_run_tags and ansible_architecture == 'aarch64' and toolkit_aarch64.matched == 0"
+
 - name: message
   debug:
-    msg:
-      - "{{ toolkit_aarch64_result | default('NOT DEFINED') }}"
+    var: toolkit_aarch64_result
   when: toolkit_aarch64_result.changed
 
 - name: find toolkit x86_64 rollback script
   find:
     paths: "{{ cann_dirs }}"
     recurse: no
     file_type: file
@@ -51,10 +50,9 @@
   debug:
     msg:
       - "[ASCEND]can not find toolkit rollback script for x86_64,toolkit rollback skipped"
   when: "ansible_architecture == 'x86_64' and toolkit_x64.matched == 0"
 
 - name: message
   debug:
-    msg:
-      - "{{ toolkit_x64_result | default('NOT DEFINED') }}"
+    var: toolkit_x64_result
   when: toolkit_x64_result.changed
```

## ascend_deployer/playbooks/install/patch/task_tfplugin.yml

```diff
@@ -27,23 +27,22 @@
   environment:
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
   register: tfplugin_result
   when: tfplugin.matched > 0
   failed_when: "tfplugin_result.rc !=0 and 'already installed' not in tfplugin_result.stdout"
 
-- name: fail if this rollback
-  fail:
-    status: 3
-  when: "'tfplugin' in ansible_run_tags and tfplugin.matched == 0"
-
 - name: message
   debug:
     msg:
       - "[ASCEND]can not find tfplugin patch package, tfplugin patch install skipped"
   when: tfplugin.matched == 0
 
+- name: fail if this rollback
+  fail:
+    status: 3
+  when: "'tfplugin' in ansible_run_tags and tfplugin.matched == 0"
+
 - name: message
   debug:
-    msg:
-      - "{{ tfplugin_result | default('NOT DEFINED') }}"
+    var: tfplugin_result
   when: tfplugin_result.changed
```

## ascend_deployer/playbooks/install/patch/task_toolkit.yml

```diff
@@ -36,10 +36,9 @@
     msg:
       - "[ASCEND]can not find toolkit patch package, toolkit patch install skipped"
   when:
     - toolkit.matched == 0
 
 - name: message
   debug:
-    msg:
-      - "{{ toolkit_result | default('NOT DEFINED') }}"
+    var: toolkit_result
   when: toolkit_result.changed
```

## ascend_deployer/playbooks/process/process_install.yml

```diff
@@ -107,43 +107,53 @@
   import_playbook: ../install/install_mindspore.yml
   tags: mindspore
 
 - name: prepare for dl
   import_playbook: ../install/task_dl.yml
   tags:
     - volcano
-    - hccl
-    - device_plugin
+    - hccl-controller
+    - ascend-device-plugin
     - noded
-    - npu_exporter
-    - docker_runtime
+    - npu-exporter
+    - ascend-docker-runtime
+    - ascend-operator
+    - resilience-controller
 
 - name: install volcano
   import_playbook: ../install/install_volcano.yml
   tags: volcano
 
-- name: install hccl
-  import_playbook: ../install/install_hccl.yml
-  tags: hccl
+- name: install hccl-controller
+  import_playbook: ../install/install_hccl-controller.yml
+  tags: hccl-controller
 
 - name: install device plugin
-  import_playbook: ../install/install_device_plugin.yml
-  tags: device_plugin
+  import_playbook: ../install/install_ascend-device-plugin.yml
+  tags: ascend-device-plugin
 
 - name: install noded
   import_playbook: ../install/install_noded.yml
   tags: noded
 
+- name: install ascend-operator
+  import_playbook: ../install/install_ascend-operator.yml
+  tags: ascend-operator
+
+- name: install resilience-controller
+  import_playbook: ../install/install_resilience-controller.yml
+  tags: resilience-controller
+
 - name: install npu-exporter
-  import_playbook: ../install/install_npu_exporter.yml
-  tags: npu_exporter
+  import_playbook: ../install/install_npu-exporter.yml
+  tags: npu-exporter
 
 - name: install docker-runtime
-  import_playbook: ../install/install_docker_runtime.yml
-  tags: docker_runtime
+  import_playbook: ../install/install_ascend-docker-runtime.yml
+  tags: ascend-docker-runtime
 
 - name: clean nexus
   import_playbook: ../clean_nexus.yml
   tags: sys_pkg
 
 - name: generate report
   import_playbook: ../report.yaml
```

## ascend_deployer/playbooks/process/process_test.yml

```diff
@@ -41,7 +41,11 @@
 - name: test toolbox
   import_playbook: ../test/test_toolbox.yml
   tags: toolbox
 
 - name: test toolkit
   import_playbook: ../test/test_toolkit.yml
   tags: toolkit
+
+- name: show result
+  import_playbook: ../test/test_exhibit.yml
+  tags: always
```

## ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml

```diff
@@ -43,8 +43,38 @@
   shell: rpm -iUv {{ base_dir }}/{{ ansible_architecture }}/*.rpm --nodeps --force
   environment:
     DEBIAN_FRONTEND: noninteractive
     DEBIAN_PRIORITY: critical
   when:
     - use_rpm_command
     - inventory_hostname != "localhost"
-  ignore_errors: true
+  ignore_errors: true
+
+
+# 创建K8s目录
+- name: create k8s image directory
+  file:
+    path: "{{resource_dir}}/k8s"
+    state: directory
+    mode: 0750
+  when:
+    - no_copy_flag != "true"
+
+# 复制version.json到远端
+- name: unarchive k8s version.json on remote
+  copy:
+    src: "{{resource_dir}}/k8s/version.json"
+    dest: "{{resource_dir}}/k8s"
+    remote_src: no
+  when:
+    - not (host_count == "1" and first_host == "localhost")
+    - no_copy_flag != "true"
+
+# 复制resources version.json到远端
+- name: unarchive resources version.json on remote
+  copy:
+    src: "{{resource_dir}}/version.json"
+    dest: "{{resource_dir}}"
+    remote_src: no
+  when:
+    - not (host_count == "1" and first_host == "localhost")
+    - no_copy_flag != "true"
```

## ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml

```diff
@@ -109,10 +109,12 @@
     - POD_NETWORK_CIDR != "" and POD_NETWORK_CIDR.startswith("192.168")
 
 - name: include k8s_status_check
   include_tasks: ./k8s_status_check.yml
   when:
     - in_k8s_group
 
+- name: get k8s version
+  include_tasks: ./get_k8s_version.yml
```

## ascend_deployer/playbooks/roles/mindx.check/defaults/compatibility_map.yml

```diff
@@ -48,18 +48,34 @@
 
 model_tags_not_support:
   "Atlas 200I SoC A1":
     - mindstudio
 
   "Atlas 500 Pro (Model 3000)":
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mindstudio
     
   "Atlas 500 Pro(Model 3000)":
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mindstudio
 
   "Atlas 800 (Model 9000)":
     - mindstudio
 
   "Atlas 800 (Model 9010)":
     - mindstudio
@@ -82,14 +98,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mindspore
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
     - tensorflow_dev
     - tensorflow_run
@@ -111,14 +135,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mindspore
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
     - tensorflow_dev
     - tensorflow_run
@@ -341,14 +373,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mindspore
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
     - tensorflow_dev
     - tensorflow_run
@@ -370,14 +410,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mindspore
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
     - tensorflow_dev
     - tensorflow_run
@@ -400,14 +448,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mef
     - mindspore
     - mindstudio
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
@@ -432,14 +488,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mef
     - mindspore
     - mindstudio
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
@@ -465,14 +529,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mindspore
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
     - tensorflow_dev
     - tensorflow_run
@@ -495,14 +567,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mindspore
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
     - tensorflow_dev
     - tensorflow_run
@@ -524,14 +604,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mef
     - mindspore
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
     - tensorflow_dev
@@ -554,14 +642,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mef
     - mindspore
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
     - tensorflow_dev
@@ -585,14 +681,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mindspore
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
     - tensorflow_dev
     - tensorflow_run
@@ -615,14 +719,22 @@
     - sys_pkg
     - tensorflow
     - tfplugin
     - toolbox
     - toolkit
     - auto
     - dl
+    - volcano
+    - hccl-controller
+    - ascend-device-plugin
+    - noded
+    - npu-exporter
+    - ascend-docker-runtime
+    - resilience-controller
+    - ascend-operator
     - mindspore
     - offline_dev
     - offline_run
     - pytorch_dev
     - pytorch_run
     - tensorflow_dev
     - tensorflow_run
```

## ascend_deployer/playbooks/roles/mindx.check/tasks/compatibility_check.yml

```diff
@@ -1,9 +1,9 @@
 - name: check compatibility for specified host
-  shell: "{{ hostvars['localhost'].discovered_interpreter_python }} {{ script_path}} {{ fact_path_dir }} {{ inventory_hostname }} {{ check_tags }}"
+  shell: "{{ ansible_playbook_python }} {{ script_path}} {{ fact_path_dir }} {{ inventory_hostname }} {{ check_tags }}"
   delegate_to: localhost
   failed_when: false
   register: check_result
 
 - name: check result
   fail:
     msg:  "{{ check_result.stdout }}"
```

## ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml

```diff
@@ -17,37 +17,48 @@
 - name: list mindxdl component dir
   shell: "ls {{mindxdl_deploy_package_dir}}/{{ansible_architecture}} | grep -vE 'zip|run' "
   register: component_list
   when:
     - inventory_hostname in groups['other_build_image'] or inventory_hostname in groups['master'][0]
 
 # 制作 noded npu-exporter deviceplugin hccl-controller镜像
-- name: build mindxdl image
+- name: build mindxdl image of noded npu-exporter deviceplugin hccl-controller resilience-controller
   shell:
     cmd:
       img_txt="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}} && (find . -name "*.yaml" -type f | grep -v "without" | grep -v "1usoc" | head -n 1))";
       if [ "$img_txt" = "" ]; then echo can not find "*.yaml" in {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}} && exit 1; fi;
       img="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}} && cat $img_txt |grep 'image:')";
       img_tag="$(echo "${img#*image:}" | sed 's/[ \t\r]*//g')";
       cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}} && docker build -t "$img_tag" .;
       cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}} && docker save -o "$(echo "$img_tag" | awk -F":" '{print $1}')_{{ansible_architecture}}.tar" "$img_tag";
   loop: "{{component_list.stdout_lines}}"
   when:
     - inventory_hostname in groups['other_build_image'] or inventory_hostname in groups['master'][0]
     - not item.endswith("tar")
     - item.count('volcano') == 0
+    - item.count('ascend-operator') == 0
 
-
-- name: check file is exist
-  stat:
-    path: "{{resource_dir}}/mindxdl/version.json"
-  register: file_status
+# 制作 ascend-operator 镜像
+- name: build mindxdl image of ascend-operator
+  shell:
+    cmd:
+      img_txt="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}} && (find . -name "*.yaml" -type f | grep -v "without" | grep -v "1usoc" | head -n 1))";
+      if [ "$img_txt" = "" ]; then echo can not find "*.yaml" in {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}} && exit 1; fi;
+      img="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}} && cat $img_txt |grep 'ascend-operator:v5.0.RC')";
+      img_tag="$(echo "${img#*image:}" | sed 's/[ \t\r]*//g')";
+      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}} && docker build -t "$img_tag" .;
+      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}} && docker save -o "$(echo "$img_tag" | awk -F":" '{print $1}')_{{ansible_architecture}}.tar" "$img_tag";
+  loop: "{{component_list.stdout_lines}}"
+  when:
+    - inventory_hostname in groups['other_build_image'] or inventory_hostname in groups['master'][0]
+    - not item.endswith("tar")
+    - item.count('ascend-operator') != 0
 
 # 制作volcano镜像
-- name: build volcano image
+- name: build volcano image for k8s 1.19.16
   shell:
     cmd:
       sche_img="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}} && cat $(find . -name "*.yaml" -type f | grep -v "without" | head -n 1) |grep 'image:' | grep "scheduler")";
       sche_img_tag="$(echo "${sche_img#*image:}" | sed 's/[ \s\t]*//')";
       cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}} && docker build -t "$sche_img_tag" -f Dockerfile-scheduler .;
       cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}} && docker save -o "{{VOLCANO_SCHEDULER_PREFIX}}_{{ansible_architecture}}.tar" "$sche_img_tag";
 
@@ -58,121 +69,116 @@
   loop: "{{component_list.stdout_lines}}"
   when:
     - inventory_hostname in groups['other_build_image'] or inventory_hostname in groups['master'][0]
     - not item.endswith("tar")
     - item.count('volcano') != 0
     - not file_status.stat.exists
 
-
 # 制作volcano镜像
-- name: build volcano image
+- name: build volcano image for k8s 1.19.16(RC2)
   shell:
     cmd:
-      sche_img="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && cat $(find . -name "*.yaml" -type f | grep -v "without" | head -n 1) |grep 'image:' | grep "scheduler")";
+      sche_img="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && cat $(find . -name "*.yaml" -type f | grep -v "without" | head -n 1) |grep 'image:' | grep "scheduler")";
       sche_img_tag="$(echo "${sche_img#*image:}" | sed 's/[ \s\t]*//')";
-      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && docker build -t "$sche_img_tag" -f Dockerfile-scheduler .;
-      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && docker save -o "{{VOLCANO_SCHEDULER_PREFIX}}_{{ansible_architecture}}.tar" "$sche_img_tag";
+      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && docker build -t "$sche_img_tag" -f Dockerfile-scheduler .;
+      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && docker save -o "{{VOLCANO_SCHEDULER_PREFIX}}_{{ansible_architecture}}.tar" "$sche_img_tag";
 
-      ctr_img="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && cat $(find . -name "*.yaml" -type f | grep -v "without" | head -n 1) |grep 'image:' | grep "controller")";
+      ctr_img="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && cat $(find . -name "*.yaml" -type f | grep -v "without" | head -n 1) |grep 'image:' | grep "controller")";
       ctr_img_tag="$(echo "${ctr_img#*image:}" | sed 's/[ \s\t]*//')";
-      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && docker build -t "$ctr_img_tag" -f Dockerfile-controller .;
-      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && docker save -o "{{VOLCANO_CONTROLLER_PREFIX}}_{{ansible_architecture}}.tar" "$ctr_img_tag";
+      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && docker build -t "$ctr_img_tag" -f Dockerfile-controller .;
+      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && docker save -o "{{VOLCANO_CONTROLLER_PREFIX}}_{{ansible_architecture}}.tar" "$ctr_img_tag";
   loop: "{{component_list.stdout_lines}}"
   when:
     - inventory_hostname in groups['other_build_image'] or inventory_hostname in groups['master'][0]
     - not item.endswith("tar")
     - item.count('volcano') != 0
-    - not use_old_k8s_version
+    - use_old_k8s_version
     - file_status.stat.exists
 
-
 # 制作volcano镜像
-- name: build volcano image
+- name: build volcano image for k8s 1.25.3(RC2)
   shell:
     cmd:
-      sche_img="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && cat $(find . -name "*.yaml" -type f | grep -v "without" | head -n 1) |grep 'image:' | grep "scheduler")";
+      sche_img="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && cat $(find . -name "*.yaml" -type f | grep -v "without" | head -n 1) |grep 'image:' | grep "scheduler")";
       sche_img_tag="$(echo "${sche_img#*image:}" | sed 's/[ \s\t]*//')";
-      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && docker build -t "$sche_img_tag" -f Dockerfile-scheduler .;
-      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && docker save -o "{{VOLCANO_SCHEDULER_PREFIX}}_{{ansible_architecture}}.tar" "$sche_img_tag";
+      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && docker build -t "$sche_img_tag" -f Dockerfile-scheduler .;
+      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && docker save -o "{{VOLCANO_SCHEDULER_PREFIX}}_{{ansible_architecture}}.tar" "$sche_img_tag";
 
-      ctr_img="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && cat $(find . -name "*.yaml" -type f | grep -v "without" | head -n 1) |grep 'image:' | grep "controller")";
+      ctr_img="$(cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && cat $(find . -name "*.yaml" -type f | grep -v "without" | head -n 1) |grep 'image:' | grep "controller")";
       ctr_img_tag="$(echo "${ctr_img#*image:}" | sed 's/[ \s\t]*//')";
-      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && docker build -t "$ctr_img_tag" -f Dockerfile-controller .;
-      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0 && docker save -o "{{VOLCANO_CONTROLLER_PREFIX}}_{{ansible_architecture}}.tar" "$ctr_img_tag";
+      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && docker build -t "$ctr_img_tag" -f Dockerfile-controller .;
+      cd {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0 && docker save -o "{{VOLCANO_CONTROLLER_PREFIX}}_{{ansible_architecture}}.tar" "$ctr_img_tag";
   loop: "{{component_list.stdout_lines}}"
   when:
     - inventory_hostname in groups['other_build_image'] or inventory_hostname in groups['master'][0]
     - not item.endswith("tar")
     - item.count('volcano') != 0
-    - use_old_k8s_version
+    - not use_old_k8s_version
     - file_status.stat.exists
 
-
 # 拷贝所有的yaml到固定目录下
-- name: copy mindxdl images
+- name: copy mindxdl yaml
   shell: "cp {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/*.yaml {{mindxdl_yaml_dir}}"
   loop: "{{component_list.stdout_lines}}"
   when:
     - inventory_hostname in groups['master'][0]
     - not item.endswith("tar")
     - item.count('volcano') == 0
 
-- name: copy volcano images
+- name: copy volcano yaml
   shell: "cp {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/*.yaml {{mindxdl_yaml_dir}}"
   loop: "{{component_list.stdout_lines}}"
   when:
     - inventory_hostname in groups['master'][0]
     - not item.endswith("tar")
     - item.count('volcano') != 0
     - use_old_k8s_version
+    - not file_status.stat.exists
 
-# 拷贝所有的yaml到固定目录下
-- name: copy volcano 1.4.0 images
+- name: copy volcano 1.4.0 for k8s 1.19.16(RC2)
   shell: "cp {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0/*.yaml {{mindxdl_yaml_dir}}"
   loop: "{{component_list.stdout_lines}}"
   when:
     - inventory_hostname in groups['master'][0]
     - not item.endswith("tar")
     - item.count('volcano') != 0
     - use_old_k8s_version
     - file_status.stat.exists
 
-
 # 拷贝所有的yaml到固定目录下
-- name: copy volcano 1.7.0 images
+- name: copy volcano yaml
   shell: "cp {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0/*.yaml {{mindxdl_yaml_dir}}"
   loop: "{{component_list.stdout_lines}}"
   when:
     - inventory_hostname in groups['master'][0]
     - not item.endswith("tar")
     - item.count('volcano') != 0
     - not use_old_k8s_version
     - file_status.stat.exists
 
 # 拷贝volcano的yaml到固定目录下
 - name: copy volcano mindxdl images
-  shell: "cp {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0/*.tar {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}"
+  shell: "cp {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0/*.tar {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}"
   loop: "{{component_list.stdout_lines}}"
   when:
     - inventory_hostname in groups['master'][0]
     - item.count('volcano') != 0
-    - not use_old_k8s_version
+    - use_old_k8s_version
     - file_status.stat.exists
 
 # 拷贝volcano的yaml到固定目录下
 - name: copy volcano mindxdl images
-  shell: "cp {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.4.0/*.tar {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}"
+  shell: "cp {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item}}/volcano-v1.7.0/*.tar {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}"
   loop: "{{component_list.stdout_lines}}"
   when:
     - inventory_hostname in groups['master'][0]
     - item.count('volcano') != 0
-    - use_old_k8s_version
+    - not use_old_k8s_version
     - file_status.stat.exists
 
-
 - name: list mindxdl component dir
   shell: "ls {{mindxdl_deploy_package_dir}}/{{ansible_architecture}} | grep tar"
   register: images_list
   when:
     - inventory_hostname in groups['other_build_image'] or inventory_hostname in groups['master'][0]
 
 - name: fetch master dl images
```

## ascend_deployer/playbooks/roles/mindx.dl/tasks/distribute_soft_package.yaml

```diff
@@ -106,43 +106,37 @@
     - inventory_hostname in groups['other_build_image'] or inventory_hostname in groups['master'][0]
 
 - name: stat version version
   stat:
     path: "{{ resource_dir }}/version.json"
   register: version_stat
 
-
 - name: get version
   shell: cat "{{ resource_dir }}/version.json"
   register: resource_version
   when: version_stat.stat.exists
 
-
 - name: set the json data to a variable as fact
   set_fact:
     jsondata: "{{resource_version.stdout | from_json}}"
   when: version_stat.stat.exists
 
-
-
 - name: execute with version is not exist
   shell:
     cmd: |
       npu_exporter_yaml="$(ls {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item | replace('.zip', '')}} | grep yaml | grep -v 1usoc)";
       npu_exporter_yaml_PATH={{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item | replace('.zip', '')}}/$npu_exporter_yaml;
       sed -i "s/updateTime=5\s*$/updateTime=5 -enableHTTP=true /" $npu_exporter_yaml_PATH;
   loop: "{{dl_package.stdout_lines}}"
   when:
     - not version_stat.stat.exists
     - inventory_hostname in groups['other_build_image'] or inventory_hostname in groups['master'][0]
     - item.endswith("zip")
     - NPU_EXPORTER_COMPONENT in item
 
-
-
 - name: execute_sed_with300
   shell: 
     cmd: |
       npu_exporter_yaml="$(ls {{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item | replace('.zip', '')}} | grep yaml | grep -v 1usoc)";
       npu_exporter_yaml_PATH={{mindxdl_deploy_package_dir}}/{{ansible_architecture}}/{{item | replace('.zip', '')}}/$npu_exporter_yaml;
       sed -i "s/updateTime=5\s*$/updateTime=5 -enableHTTP=true /" $npu_exporter_yaml_PATH;
   loop: "{{dl_package.stdout_lines}}"
```

## ascend_deployer/playbooks/roles/mindx.dl/tasks/dl_common.yaml

```diff
@@ -9,20 +9,11 @@
     https_proxy: ""
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
   changed_when: false
   when:
     - inventory_hostname in groups['master'][0]
 
-
-# 获取节点K8s版本
-- name: get k8s version
-  shell:
-    cmd:
-      echo $(kubelet --version 2>/dev/null || echo '') | awk '{print $2}' | sed  "s/v//" | awk -F"." '{print $2}';
-  register: k8s_mid_version
-  changed_when: false
-
-- name: set fact for use_old_k8s
-  set_fact:
-    use_old_k8s_version: "{{ k8s_mid_version.stdout | int}} <= 21"
-    cacheable: yes
+- name: check mindxdl version file exist
+  stat:
+    path: "{{resource_dir}}/mindxdl/version.json"
+  register: file_status
```

## ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml

```diff
@@ -144,14 +144,65 @@
     https_proxy: ""
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
   when:
     - ansible_architecture == "aarch64"
     - inventory_hostname in groups['worker']
 
+- name: get 910B card num
+  shell: "npu-smi info -m | grep -i 910B\\d* | wc -l"
+  register: num_of_910B_card
+
+- name: label module-910b-16
+  shell: kubectl label --overwrite node {{ NODE_NAME }} accelerator-type=module-910b-16
+  delegate_to: "{{ groups['master'][0] }}"
+  delegate_facts: true
+  environment:
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when:
+     - "{{ num_of_910B_card.stdout }} > 8"
+     - inventory_hostname in groups['worker']
+     - not use_old_k8s_version
+     - file_status.stat.exists
+
+- name: label module-910b-8
+  shell: kubectl label --overwrite node {{ NODE_NAME }} accelerator-type=module-910b-8
+  delegate_to: "{{ groups['master'][0] }}"
+  delegate_facts: true
+  environment:
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when:
+     - "{{ num_of_910B_card.stdout }} <= 8"
+     - "{{ num_of_910B_card.stdout }} > 2"
+     - inventory_hostname in groups['worker']
+     - not use_old_k8s_version
+     - file_status.stat.exists
+
+- name: label module-910B-2
+  shell: kubectl label --overwrite node {{ NODE_NAME }} accelerator-type=card-910b-2
+  delegate_to: "{{ groups['master'][0] }}"
+  delegate_facts: true
+  environment:
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when:
+     - "{{ num_of_910B_card.stdout }} <= 2"
+     - "{{ num_of_910B_card.stdout }} > 0"
+     - inventory_hostname in groups['worker']
+     - not use_old_k8s_version
+     - file_status.stat.exists
+
 - name: create log directories
   file:
     path: /var/log/mindx-dl
     state: directory
     owner: root
     group: root
     mode: 0755
```

## ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml

```diff
@@ -23,12 +23,21 @@
   changed_when: false
 
 - name: message
   debug:
     msg: "*************************start install docker***************************"
   when: not docker_installed
 
+- name: message
+  debug:
+    msg: "containerd need reinstall, the script will install containerd."
+  when: not use_old_k8s_version
+
+- name: message
+  debug:
+    msg: "************************start install containerd**********************"
+  when: not use_old_k8s_version
+
 - name: include copy task
   include_tasks: copy.yml
-  when: not docker_installed
```

## ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml

```diff
@@ -22,24 +22,14 @@
     src: "{{ k8s_image_dir }}/{{ ansible_architecture }}_125.tar.gz"
     dest: "{{ k8s_image_dir }}"
     remote_src: no
   when:
     - no_copy_flag != "true"
     - not use_old_k8s_version
 
-# 复制version.json到远端
-- name: unarchive k8s version.json on remote
-  copy:
-    src: "{{resource_dir}}/k8s/version.json"
-    dest: "{{resource_dir}}/k8s"
-    remote_src: no
-  when:
-    - not (host_count == "1" and first_host == "localhost")
-    - no_copy_flag != "true"
-
 - name: list k8s images
   shell: "ls {{ k8s_image_dir }}/{{ ansible_architecture }}"
   register: k8s_image
 
 # 1.25.3 加载k8s镜像
 - name: load k8s images by ctr load
   shell: "ctr -n k8s.io images import {{ k8s_image_dir }}/{{ ansible_architecture }}/{{ item }} --all-platforms"
```

## ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml

```diff
@@ -103,44 +103,22 @@
     - devices_v1alpha1_devicemodel.yaml
     - cluster_objectsync_v1alpha1.yaml
     - objectsync_v1alpha1.yaml
     - router_v1_rule.yaml
     - router_v1_ruleEndpoint.yaml
 
 - name: generate cert and default config
-  shell: |
-    bash {{role_path}}/files/certgen.sh genCertAndKey server /etc/kubeedge/certs {{ MASTER_IP }}
-    /usr/local/bin/cloudcore --defaultconfig > /etc/kubeedge/config/cloudcore.yaml
+  shell: /usr/local/bin/cloudcore --defaultconfig > /etc/kubeedge/config/cloudcore.yaml
 
 - name: set kubeconfig
   lineinfile:
     path: /etc/kubeedge/config/cloudcore.yaml
     regexp: 'kubeConfig: ""'
     line: '  kubeConfig: "/etc/kubernetes/admin.conf"'
 
-- name: copy rootCA.crt to edge-manager
-  copy:
-    src: /etc/kubeedge/ca/rootCA.crt
-    dest: "{{ item }}"
-    owner: "{{DL_USR}}"
-    group: "{{DL_GRP}}"
-    remote_src: yes
-    mode: 0600
-  loop:
-    - /etc/mindx-dl/edge-manager
-
-- name: copy rootCA.crt to image-manager
-  copy:
-    src: /etc/kubeedge/ca/rootCA.crt
-    dest: /etc/mindx-dl/image-manager
-    owner: root
-    group: root
-    remote_src: yes
-    mode: 0600
-
 - name: apply kubeedge yamls
   shell: "kubectl apply -f /etc/kubeedge/yamls/{{ item }}"
   with_items:
     - devices_v1alpha1_device.yaml
     - devices_v1alpha1_devicemodel.yaml
     - cluster_objectsync_v1alpha1.yaml
     - objectsync_v1alpha1.yaml
```

## ascend_deployer/playbooks/roles/mindx.rep/tasks/hccn_rep.yaml

```diff
@@ -1,20 +1,25 @@
 - name: check driver exists
   shell: npu-smi info ||true
   register: raw_driver_info
 
+- name: get npu num id
+  shell: npu-smi info -l| grep 'NPU ID'| awk '{print $4}'
+  register: npu_ids
+  when: raw_driver_info.stdout != ''
+
 - name: get the driver info
   copy:
     src: ./get_npu_info.py
     dest: "{{ ansible_env.HOME }}/"
     mode: 0700
     force: yes
 
 - name: execute the info script1
-  command: python3 {{ansible_env.HOME}}/get_npu_info.py {{raw_driver_info.stdout_lines|default([])}}
+  command: "{{ discovered_interpreter_python | default('python') }} {{ansible_env.HOME}}/get_npu_info.py {{raw_driver_info.stdout_lines|default([])}}"
   register: driver_info
 
 - name: gather driver facts
   set_fact:
     driver_dict: "{{driver_dict|default({})|combine({item:{'npu':hostvars[item]['driver_info']['stdout']|default('')}})}}"
   delegate_to: localhost
   run_once: true
@@ -27,49 +32,41 @@
     content: "{{ driver_dict }}"
     dest:  "{{ tmp_file_path }}/driver_dict.json"
     mode: 0700
     force: yes
   delegate_to: localhost
   run_once: true
 
-- name: check tool exist
-  stat:
-    path: "{{ resource_dir }}/tool/hccn"
+- name: check hccn tool exist
+  shell: command -v hccn_tool||true
   register: hccn_tool
 
-- name: copy hccn-aarch64 to remote hosts
-  copy:
-    src: "{{ resource_dir }}/tool/hccn/hccn-aarch64"
-    dest: "{{ ansible_env.HOME }}/"
-    mode: 0700
-    force: yes
-  when: hccn_tool.stat.exists
-
-- name: copy hccn-x86_64 to remote hosts
-  copy:
-    src: "{{ resource_dir }}/tool/hccn/hccn-x86_64"
-    dest: "{{ ansible_env.HOME }}/"
-    mode: 0700
-    force: yes
-  when: hccn_tool.stat.exists
+- name: get raw hccn info
+  shell: "hccn_tool -i {{item}} -ip -g&&hccn_tool -i {{item}} -net_health -g"
+  register: temp_hccn
+  ignore_errors: true
+  loop: "{{npu_ids.stdout_lines}}"
+  when: hccn_tool.stdout != ''
 
-- name: hccn_tool configures IP address
-  shell: "{{ ansible_env.HOME }}/hccn-{{ ansible_architecture }} view"
-  register: hccn_result
-  when: hccn_tool.stat.exists
+- name: add hccn output
+  set_fact:
+    hccn_result: "{{ hccn_result + [item.stdout] }}"
+  loop: "{{ temp_hccn.results }}"
+  when: item.stdout is defined and item.stdout != '' and hccn_tool.stdout != ''
 
 - set_fact:
-    hccn_dict: "{{hccn_dict|default({})|combine({item:{'hccn':hostvars[item]['hccn_result']['stdout']|default('')}})}}"
+    hccn_dict: "{{hccn_dict|default({})|combine({item:{'hccn':hostvars[item]['hccn_result']}})}}"
   delegate_to: localhost
   run_once: true
   with_items: "{{ groups['master'] +  groups['worker'] }}"
   ignore_errors: true
   when: hostvars[item].hccn_result is defined
 
 - name: output hccn file
   copy:
     content: "{{ hccn_dict }}"
     dest:  "{{ tmp_file_path }}/hccn_dict.json"
     mode: 0700
     force: yes
   delegate_to: localhost
   run_once: true
+  when: hccn_dict is defined
```

## ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py

```diff
@@ -1,7 +1,23 @@
+#!/usr/bin/env python3
+# coding: utf-8
+# Copyright 2023 Huawei Technologies Co., Ltd
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ===========================================================================
 import json
 import csv
 import os.path
 import sys
 
 
 def solve_value_list(value_list):
@@ -15,41 +31,47 @@
                 if key == 'version':
                     str_item += (":" + value)
             value_list[index] = str_item
     ret += "\n".join(value_list)
     return ret
 
 
+def get_hccn(hccn_list):
+    if not hccn_list:
+        return 'NA'
+    for hccn in hccn_list:
+        if isinstance(hccn, str) and 'success' not in hccn.lower():
+            return 'fail'
+    return 'ok'
+
+
 def main(path):
     with open(path) as f:
         data = json.load(f)
         dir_name = os.path.dirname(path)
         ips = list(data.keys())
 
-        fieldsname = ["IP", "npu", "packages", "HCCN info", "node name", "node type", "status", "ok pods",
-                      "missing pods", "failed pods", "npu resource name in K8s", "images", "dl result"]
+        fieldsname = ["IP", "node name", "node type", "node status", "npu", "packages", "HCCN health check", "ok pods",
+                      "MindX-DL status"]
         flags = os.O_WRONLY | os.O_CREAT
         with os.fdopen(os.open(dir_name + '/report.csv', flags, 0o644), 'w', newline='') as wf:
             writer = csv.DictWriter(wf, fieldnames=fieldsname)
             writer.writeheader()
             for ip in ips:
                 row = [ip]
-                npu = data.get(ip, {}).get('npu', '')
+                npu = data.get(ip, {}).get('npu', 'NA')
                 packages = solve_value_list(data.get(ip, {}).get('packages', []))
-                hccn_info = data.get(ip, {}).get('hccn', '')
-                node_name = data.get(ip, {}).get('node name', '')
-                node_type = data.get(ip, {}).get('node type', '')
-                status = data.get(ip, {}).get('status', '')
+                hccn_list = data.get(ip, {}).get('hccn', [])
+                hccn_info = get_hccn(hccn_list)
+                node_name = data.get(ip, {}).get('node name', 'NA')
+                node_type = data.get(ip, {}).get('node type', 'NA')
+                status = data.get(ip, {}).get('status', 'NA')
                 ready_pods = "\n".join(data.get(ip, {}).get('ready pods', []))
-                missing_pods = "\n".join(data.get(ip, {}).get('missing pods', []))
-                failed_pods = "\n".join(data.get(ip, {}).get('failed pods', []))
-                npu_cap = "\n".join(data.get(ip, {}).get('npu in K8s', []))
-                images = "\n".join(data.get(ip, {}).get('images', []))
-                result = data.get(ip, {}).get('dl result', '')
+                result = data.get(ip, {}).get('dl result', 'NA')
                 row.extend(
-                    [npu, packages, hccn_info, node_name, node_type, status, ready_pods, missing_pods, failed_pods,
-                     npu_cap, images, result])
+                    [node_name, node_type, status, npu, packages or 'NA', hccn_info, ready_pods or 'NA',
+                     result or 'NA'])
                 writer.writerow(dict(zip(fieldsname, row)))
 
 
 if __name__ == '__main__':
     main(sys.argv[1])
```

## ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py

```diff
@@ -1,7 +1,23 @@
+#!/usr/bin/env python3
+# coding: utf-8
+# Copyright 2023 Huawei Technologies Co., Ltd
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ===========================================================================firmware_ver
 import os.path
 import subprocess
 import json
 import sys
 from collections import OrderedDict
 
 require_by_all = ["calico-node", "kube-proxy", ]
@@ -15,79 +31,46 @@
 all_master_together_by_scene = {'1': ["calico-kube-controllers", "coredns", "hccl-controller", "ascend-operator",
                                       " resilience-controller", "volcano-scheduler", "volcano-controllers"],
                                 '2': ["calico-kube-controllers", "coredns",
                                       "volcano-scheduler", "volcano-controllers", ],
                                 '3': ["calico-kube-controllers", "coredns"],
                                 '4': ["calico-kube-controllers", "coredns"]
                                 }
-                                
+
 worker_by_scene = {
     '1': ["ascend-device-plugin", "noded", "npu-exporter", ],
     '2': ["ascend-device-plugin", ],
     '3': ["ascend-device-plugin", ]
 }
 
 
-def get_type(master, worker):
-    if master and worker:
-        ret = "master,worker"
-    elif master:
-        ret = "master"
-    else:
-        ret = "worker"
-    return ret
-
-
-def get_status(conditions):
-    return conditions[len(conditions) - 1].get("type", "")
-
-
-def get_npu(capacity):
-    devices = []
-    for key, value in capacity.items():
-        if "huawei" in key:
-            devices.append("%s:%s" % (key, value))
-    return devices
-
-
-def get_images(images):
-    ret = []
-    for dic in images:
-        ret.extend(dic.get("names", []))
-    return ret
-
-
 def get_nodes_info():
     result = subprocess.check_output(['kubectl', 'get', 'nodes', '-o', 'json'], encoding="utf-8")
     nodes_info = json.loads(result)
-    nodes_dict = {}
-    for node in nodes_info.get("items", {}):
-        ip_address = node.get("status", {}).get("addresses", [])[0].get("address", "")
+    k8s_node = {}
+    for node_json in nodes_info.get("items", {}):
+        node = K8sNode(**node_json)
+        ip_address = node.get_ip()
         property_dict = OrderedDict()
-        property_dict['node name'] = node.get("status", {}).get("addresses", [])[1].get("address", "")
-        property_dict['node type'] = get_type(node.get("metadata", {}).get("labels", {}).get("masterselector", ""),
-                                              node.get("metadata", {}).get("labels", {}).get("workerselector", ""))
-        property_dict['status'] = get_status(node.get("status", {}).get("conditions", []))
-        property_dict['npu in K8s'] = get_npu(node.get("status", {}).get("capacity", {}))
-        property_dict['images'] = get_images(node.get("status", {}).get("images", []))
-        property_dict['ready pods'] = []
-        property_dict['missing pods'] = []
-        property_dict['failed pods'] = []
-        nodes_dict[ip_address] = property_dict
-    return nodes_dict
+        property_dict['node name'] = node.get_name()
+        property_dict['node type'] = node.get_type()
+        property_dict['status'] = node.get_status()
+        k8s_node[ip_address] = property_dict
+    return k8s_node
 
 
 def get_pods_info(nodes_dict):
     result = subprocess.check_output(['kubectl', 'get', 'pods', '-A', '-o', 'json'], encoding="utf-8")
     pods_info = json.loads(result)
-    for pod in pods_info.get("items", {}):
-        ip = pod.get("status", {}).get("hostIP", "")
+    for pod_json in pods_info.get("items", {}):
+        pod = K8sPod(**pod_json)
+        ip = pod.get_ip()
         property_dict = nodes_dict.get(ip, {})
-        name = pod.get("metadata", {}).get("name", "")
-        if pod.get("status", {}).get("phase", "") == "Running":
+        name = pod.get_name()
+        if pod.get_status():
             property_dict.setdefault('ready pods', [])
             property_dict.get('ready pods', []).append(name)
         else:
             property_dict.setdefault('failed pods', [])
             property_dict.get('failed pods', []).append(name)
 
     return nodes_dict
@@ -142,25 +125,102 @@
 
 
 def append_result(node_dict, result):
     for ip, info in node_dict.items():
         info.setdefault("dl result", result)
 
 
+class K8sPod:
+    def __init__(self, status=None, metadata=None, **kwargs):
+        self.status = PodStatus(**status)
+        self.metadata = metadata
+
+    def get_ip(self):
+        return self.status.host_ip or ''
+
+    def get_name(self):
+        if isinstance(self.metadata, dict) and 'name' in self.metadata:
+            return self.metadata.get('name', '')
+        return ''
+
+    def get_status(self):
+        if self.status.container_statuses:
+            return self.status.container_statuses[0].get('ready', False)
+        return False
+
+
+class PodStatus:
+    def __init__(self, **kwargs):
+        self.host_ip = kwargs.get('hostIP')
+        self.container_statuses = kwargs.get('containerStatuses')
+
+
+class K8sNode:
+    def __init__(self, status=None, metadata=None, **kwargs):
+        self.status = NodeStatus(**status)
+        self.metadata = MetaData(**metadata)
+
+    def get_ip(self):
+        if self.status.addresses:
+            return self.status.addresses[0].get('address', 'NA')
+        return ''
+
+    def get_name(self):
+        if self.status.addresses:
+            return self.status.addresses[1].get('address', 'NA')
+        return ''
+
+    def get_type(self):
+        if self.metadata.labels.get("masterselector") and self.metadata.labels.get("workerselector"):
+            return "master,worker"
+        elif self.metadata.labels.get("masterselector"):
+            return "master"
+        elif self.metadata.labels.get("workerselector"):
+            return "worker"
+        else:
+            return ''
+
+    def get_status(self):
+        if isinstance(self.status.conditions, list) and len(self.status.conditions) >= 2:
+            return self.status.conditions[-1].get("type", "")
+        return ''
+
+    def get_npu(self):
+        devices = []
+        for key, value in self.status.capacity.items():
+            if "huawei" in key:
+                devices.append("%s:%s" % (key, value))
+        return devices
+
+
+class MetaData:
+    def __init__(self, labels=None, **kwargs):
+        self.labels = labels
+
+
+class NodeStatus:
+    def __init__(self, addresses=None, capacity=None, conditions=None, **kwargs):
+        if not isinstance(addresses, list) or len(addresses) < 2:
+            raise Exception('json format error, wrong address: %s' % str(addresses))
+        self.addresses = addresses
+        self.capacity = capacity
+        self.conditions = conditions
+
+
 def main(path_name, scene):
     node_dict = get_nodes_info()
     node_dict = get_pods_info(node_dict)
     node_dict = check_missing_pods(node_dict, scene)
     if is_dl_success(node_dict):
         append_result(node_dict, "success")
     else:
         append_result(node_dict, "failed")
     if os.path.isdir(path_name):
         flags = os.O_WRONLY | os.O_CREAT
-        with os.fdopen(os.open(path_name + '/node_dict.json', flags, 0o700), 'w', newline='') as f:
+        with os.fdopen(os.open(os.path.join(path_name, 'node_dict.json'), flags, 0o700), 'w', newline='') as f:
             json.dump(node_dict, f)
 
 
 if __name__ == '__main__':
     path = sys.argv[1]
     scene_num = sys.argv[2]
     main(path, scene_num)
```

## ascend_deployer/playbooks/roles/mindx.rep/tasks/local_rep.yaml

```diff
@@ -1,25 +1,25 @@
 - name: check if k8s cluster exist
   shell: kubectl get nodes||true
   register: cluster_set
 
 - name: collect k8s info
-  command: python3 {{playbook_dir}}/roles/mindx.rep/tasks/k8s_rep.py {{tmp_file_path}} {{SCENE_NUM|default('1')}}
+  command: "{{ ansible_playbook_python }} {{playbook_dir}}/roles/mindx.rep/tasks/k8s_rep.py {{tmp_file_path}} {{SCENE_NUM|default('1')}}"
   when: cluster_set.stdout != ''
 
 - name: remove the former report
   ansible.builtin.file:
     path: "{{report_output_path}}"
     state: absent
 
 - name: create the dir if not exist
   command: mkdir -p {{report_output_path}}
   
 - name: merge all json
-  command: python3 {{playbook_dir}}/roles/mindx.rep/tasks/output_json.py {{tmp_file_path}} {{report_output_path}}
+  command: "{{ ansible_playbook_python }} {{playbook_dir}}/roles/mindx.rep/tasks/output_json.py {{tmp_file_path}} {{report_output_path}}"
   
 - name: remove the tmp file
   ansible.builtin.file:
     path: "{{ tmp_file_path }}"
     state: absent
 
 - name: convert json to csv - read
@@ -29,9 +29,9 @@
 
 - name: convert json to csv - write
   set_fact:
     report_json_data: "{{ report_json.stdout|from_json }}"
   when: output_format == 'csv'
 
 - name: output to csv
-  command: python3  {{playbook_dir}}/roles/mindx.rep/tasks/json_to_csv.py {{report_output_path}}/report.json
+  command: "{{ ansible_playbook_python }}  {{playbook_dir}}/roles/mindx.rep/tasks/json_to_csv.py {{report_output_path}}/report.json"
   when: output_format == 'csv'
```

## ascend_deployer/playbooks/roles/mindx.rep/tasks/packages_rep.yaml

```diff
@@ -13,15 +13,15 @@
 
 - name: print missed host
   fail:
     msg: "missing hosts: {{(groups['master'] + groups['worker'])|difference(ansible_play_batch)}}"
   when: (groups['master'] + groups['worker'])|difference(ansible_play_batch)|length >0
 
 - name: python3 the scripts
-  command: python3 {{ tmp_file_path }}/app_info.fact.j2
+  command: "{{ discovered_interpreter_python | default('python') }} {{ tmp_file_path }}/app_info.fact.j2"
   register: packages_result
 
 - name: remove the app info file
   ansible.builtin.file:
     path: "{{ tmp_file_path }}/app_info.fact.j2"
     state: absent
 
@@ -46,20 +46,22 @@
     dest:  "{{ tmp_file_path }}/packages_dict.json"
     mode: 0700
     force: yes
   delegate_to: localhost
   run_once: true
 
 - name: get the formatted result
-  shell: python3 {{playbook_dir}}/roles/mindx.rep/tasks/ls_format.py {{ tmp_file_path }}/packages_dict.json
+  shell: "{{ ansible_playbook_python }} {{playbook_dir}}/roles/mindx.rep/tasks/ls_format.py {{ tmp_file_path }}/packages_dict.json"
   register: package_list
   delegate_to: localhost
   run_once: true
 
 - name: show the result
   debug:
     msg: "[ASCEND]{{package_list.stdout|default('')}}"
   run_once: true
   when: only_package
 
 - include_tasks: ./hccn_rep.yaml
-  when: not only_package
+  vars:
+    - hccn_result: []
+  when: not only_package
```

## ascend_deployer/playbooks/test/case_driver.yml

```diff
@@ -1,7 +1,10 @@
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'driver':'ERROR'})}}"
+
 - name: test if driver installed
   find:
     path: /usr/local/Ascend/driver
     recurse: yes
     file_type: file
     use_regex: yes
     patterns: "version.info"
@@ -9,26 +12,34 @@
 
 - name: message
   debug:
     msg:
       - "driver not installed"
   when: driver.matched == 0
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'driver':'not installed'})}}"
+  when: driver.matched == 0
+
 - name: execute npu-smi info
   shell: npu-smi info
   environment:
     PATH: /usr/local/{{ python_version }}/bin:/usr/local/Ascend/toolbox/latest/Ascend-DMI/bin:{{ ansible_env.PATH }}
     LD_LIBRARY_PATH: /usr/local/{{ python_version }}/lib:/usr/local/Ascend/toolbox/latest/Ascend-DMI/lib64:/usr/local/dcmi:/usr/local/Ascend/nnae/latest/fwkacllib/lib64:/usr/local/Ascend/nnrt/latest/acllib/lib64
   when: driver.matched > 0
   register: smi_info
 
 - name: print npu-smi info
   debug: var=smi_info
   when: driver.matched > 0
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'driver':'OK'})}}"
+  when: smi_info.stdout != ''
+
 - name: get npu desc
   set_fact:
     tmp_npu_desc: "{{ '300i' if cus_npu_info == '300i-pro' else '300v'}}"
   when:
     - ansible_local.npu_info.product == "A300i"
     - cus_npu_info is defined
     - (cus_npu_info == "300i-pro") or (cus_npu_info == "300v-pro")
@@ -42,18 +53,23 @@
   when:
     - ansible_user_uid == 0
     - ansible_local.npu_info.product == "A300i"
     - driver.matched > 0
     - tmp_npu_desc is defined
   ignore_errors: yes
 
-- name: display driver not match
-  debug:
-    msg:
-      - "you are installing driver of {{ cus_npu_info }} on hardware of {{ '300v-pro' if cus_npu_info == '300i-pro' else '300i-pro' }}"
+- name: set if not match
+  set_fact:
+    not_fit: true
+    test_dict: "{{test_dict|default({})|combine({'driver':'ERROR'})}}"
   when:
     - ansible_user_uid == 0
     - ansible_local.npu_info.product == "A300i"
     - driver.matched > 0
     - tmp_npu_desc is defined
     - npu_300vi_check_result_info is defined
     - npu_300vi_check_result_info.stdout == "0"
+
+- name: display driver not match
+  debug:
+    msg:  "you are installing driver of {{ cus_npu_info }} on hardware of {{ '300v-pro' if cus_npu_info == '300i-pro' else '300i-pro' }}"
+  when: not_fit is defined
```

## ascend_deployer/playbooks/test/case_firmware.yml

```diff
@@ -1,23 +1,44 @@
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'firmware':'ERROR'})}}"
+
+- name: check firmware installed
+  find:
+    path: /usr/local/Ascend/firmware/
+    recurse: yes
+    file_type: file
+    use_regex: yes
+    patterns: "version.info"
+  register: firmware_ver
+
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'firmware':'not installed'})}}"
+  when: firmware_ver.matched == 0
+
 - name: test if driver installed
   find:
     path: /usr/local/Ascend/driver
     recurse: yes
     file_type: file
     use_regex: yes
     patterns: "upgrade-tool"
   register: upgrade_tool
 
 - name: message
   debug:
     msg:
-    - "can not find upgrade tool"
+    - "cannot find upgrade tools"
   when: upgrade_tool.matched == 0
 
 - name: check firmware
   shell: /usr/local/Ascend/driver/tools/upgrade-tool --device_index -1 --system_version
   register: upgrade_tool_result
   when: upgrade_tool.matched > 0
 
 - name: print upgrade tool output
   debug: var=upgrade_tool_result
   when: upgrade_tool.matched > 0
+
+- name: set the output
+  set_fact:
+    test_dict: "{{test_dict|default({})|combine({'firmware':'OK'})}}"
+  when: "'succeed' in upgrade_tool_result.stdout"
```

## ascend_deployer/playbooks/test/case_mindspore.yml

```diff
@@ -1,7 +1,10 @@
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'mindspore':'ERROR'})}}"
+
 - name: check mindspore
   shell: python3 -m pip list | grep mindspore
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   failed_when: false
   changed_when: false
@@ -13,38 +16,51 @@
 
 - name: message
   debug:
     msg:
       - "mindspore not installed"
   when: mindspore_version.stdout == ""
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'mindspore':'not installed'})}}"
+  when: mindspore_version.stdout == ""
+
 - name: test import mindspore ascend
   shell: . {{ ascend_install_path }}/ascend-toolkit/set_env.sh && python3 -c "import mindspore as ms; print(ms.__version__)"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ascend_install_path }}/ascend-toolkit/latest/atc/ccec_compiler/bin/:{{ ansible_env.PATH }}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ local_path }}/gcc7.3.0/lib64:{{ ascend_install_path }}/ascend-toolkit/latest/acllib/lib64:{{ ascend_install_path }}/ascend-toolkit/latest/atc/lib64:{{ ascend_install_path }}/ascend-toolkit/latest/fwkacllib/lib64:{{ ascend_install_path }}/driver/lib64:{{ ascend_install_path }}/opp/op_impl/built-in/ai_core/tbe/op_tiling:{{ local_path }}/{{ python_version }}/lib/{{ python_version }}[:9]/site-packages/mindspore/lib:{{ ascend_install_path }}/ascend-toolkit/latest/opp/op_impl/built-in/ai_core/tbe/op_tiling:{{ansible_user_dir}}/Ascend/ascend-toolkit/latest/fwkacllib/lib64/plugin/opskernel"
     TBE_IMPL_PATH: "{{ ascend_install_path }}/ascend-toolkit/latest/opp/op_impl/built-in/ai_core/tbe"
     ASCEND_OPP_PATH: "{{ ascend_install_path }}/ascend-toolkit/latest/opp"
     PYTHONPATH: "{{ ascend_install_path }}/ascend-toolkit/latest/opp/op_impl/built-in/ai_core/tbe:{{ ascend_install_path }}/ascend-toolkit/latest/fwkacllib/python/site-packages/"
   register: mindspore_ascend_version
   when:
     - mindspore_version.stdout != ""
     - ansible_local.npu_info.scene != ""
 
+- name: print mindspore ascend version
+  debug: var=mindspore_ascend_version
+  when: mindspore_ascend_version is defined
+
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'mindspore':'OK'})}}"
+  when: mindspore_ascend_version.rc is defined and mindspore_ascend_version.rc == 0
+
 - name: test import mindspore cpu
   shell: python3 -c "import mindspore as ms; print(ms.__version__)"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: mindspore_cpu_version
   when:
     - mindspore_version.stdout != ""
     - ansible_local.npu_info.scene == ""
     - "'Ubuntu_18.04' in os_and_arch"
 
-- name: print mindspore ascend version
-  debug: var=mindspore_ascend_version
-  when: mindspore_ascend_version is defined
-
 - name: print mindspore cpu version
   debug: var=mindspore_cpu_version
   when: mindspore_cpu_version is not skipped
+
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'mindspore':'OK'})}}"
+  when: mindspore_cpu_version.rc is defined and mindspore_cpu_version.rc == 0
+
```

## ascend_deployer/playbooks/test/case_nnae.yml

```diff
@@ -1,7 +1,10 @@
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'nnae':'OK'})}}"
+
 - name: test if toolbox installed
   find:
     paths:
       - "{{ ascend_install_path }}/toolbox"
     recurse: yes
     file_type: file
     use_regex: yes
@@ -20,19 +23,11 @@
 
 - name: message
   debug:
     msg:
     - "toolbox or nnae not installed, please install first"
   when: ascend_dmi.matched == 0 or nnae.matched == 0
 
-- name: execute ascend-dmi -c
-  shell: ascend-dmi -c | grep nnae | awk '{print $6}'
-  environment:
-    PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ascend_install_path }}/toolbox/latest/Ascend-DMI/bin:{{ ansible_env.PATH }}"
-    LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ ascend_install_path }}/toolbox/latest/Ascend-DMI/lib64:/usr/local/dcmi:{{ ascend_install_path }}/nnae/latest/opp/fwkacllib/lib64:{{ ascend_install_path }}/nnrt/latest/acllib/lib64:{{ local_path }}/gcc7.3.0/lib64:{{ ascend_install_path }}/add-ons:/usr/local/Ascend/driver/lib64/common:/usr/local/Ascend/driver/lib64/driver"
-    ASCEND_OPP_PATH: "{{ ascend_install_path }}/nnae/latest/opp:{{ ascend_install_path }}/nnrt/latest/opp"
-  when: ascend_dmi.matched > 0 and nnae.matched > 0
-  register: nnae_status
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'nnae':'not installed'})}}"
+  when: nnae.matched == 0
 
-- name: print nnae status
-  debug: var=nnae_status
-  when: ascend_dmi.matched > 0 and nnae.matched > 0
```

## ascend_deployer/playbooks/test/case_nnrt.yml

```diff
@@ -1,7 +1,10 @@
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'nnrt':'OK'})}}"
+
 - name: test if toolbox installed
   find:
     paths:
       - "{{ ascend_install_path }}/toolbox"
     recurse: yes
     file_type: file
     use_regex: yes
@@ -20,19 +23,10 @@
 
 - name: message
   debug:
     msg:
     - "toolbox or nnrt not installed, please install first"
   when: ascend_dmi.matched == 0 or nnrt.matched == 0
 
-- name: execute ascend-dmi -c
-  shell: ascend-dmi -c | grep nnrt | awk '{print $6}'
-  environment:
-    PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ascend_install_path }}/toolbox/latest/Ascend-DMI/bin:{{ ansible_env.PATH }}"
-    LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ ascend_install_path }}/toolbox/latest/Ascend-DMI/lib64:/usr/local/dcmi:{{ ascend_install_path }}/nnae/latest/opp/fwkacllib/lib64:{{ ascend_install_path }}/nnrt/latest/acllib/lib64:{{ local_path }}/gcc7.3.0/lib64:{{ ascend_install_path }}/add-ons:/usr/local/Ascend/driver/lib64/common:/usr/local/Ascend/driver/lib64/driver"
-    ASCEND_OPP_PATH: "{{ ascend_install_path }}/nnae/latest/opp:{{ ascend_install_path }}/nnrt/latest/opp"
-  when: ascend_dmi.matched > 0 and nnrt.matched > 0
-  register: nnrt_status
-
-- name: print nnrt status
-  debug: var=nnrt_status
-  when: ascend_dmi.matched > 0 and nnrt.matched > 0
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'nnrt':'not installed'})}}"
+  when: nnrt.matched == 0
```

## ascend_deployer/playbooks/test/case_pytorch.yml

```diff
@@ -1,7 +1,10 @@
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'pytorch':'ERROR'})}}"
+
 - name: check torch
   shell: python3 -m pip list | grep torch
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   failed_when: false
   changed_when: false
@@ -13,14 +16,18 @@
 
 - name: message
   debug:
     msg:
       - "pytorch not installed"
   when: torch_version.stdout == ""
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'pytorch':'not installed'})}}"
+  when: torch_version.stdout == ""
+
 - name: check add_ons directory exists
   shell: find {{ ascend_install_path }} -type d | grep add-ons | wc -l
   register: add_ons_dir
   when: torch_version.stdout != ""
 
 - name: check add_ons directory contains libprotobuf.so
   shell: find {{ ascend_install_path }}/add-ons/ -type f | grep libprotobuf.so | wc -l
@@ -41,18 +48,22 @@
   when:
     - torch_version.stdout != ""
     - add_ons_dir.stdout == '0' or add_ons_dir_protobuf.stdout == '0'
   changed_when: false
 
 - name: print import pytorch result without add-ons
   debug: var=import_torch
-  when: 
+  when:
     - torch_version.stdout != ""
     - add_ons_dir.stdout == '0' or add_ons_dir_protobuf.stdout == '0'
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'pytorch':'OK'})}}"
+  when: import_torch.rc is defined and import_torch.rc == 0
+
 - name: test import pytorch with add-ons
   shell:
     if [ -f {{ ascend_install_path }}/ascend-toolkit/set_env.sh ];then . {{ ascend_install_path }}/ascend-toolkit/set_env.sh;fi
     if [ -f {{ ascend_install_path }}/nnae/set_env.sh ];then . {{ ascend_install_path }}/nnae/set_env.sh;fi
     python3 -c "import torch; print(torch.__version__)"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
@@ -66,7 +77,13 @@
 
 - name: print import pytorch result with add-ons
   debug: var=import_torch_with_add_ons
   when:
     - torch_version.stdout != ""
     - add_ons_dir.stdout != '0'
     - add_ons_dir_protobuf.stdout != '0'
+
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'pytorch':'OK'})}}"
+  when: import_torch_with_add_ons.rc is defined and import_torch_with_add_ons.rc == 0
+
+
```

## ascend_deployer/playbooks/test/case_tensorflow.yml

```diff
@@ -1,7 +1,10 @@
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'tensorflow':'ERROR'})}}"
+
 - name: check tensorflow
   shell: python3 -m pip list | grep -E "tensorflow |tensorflow-cpu"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   failed_when: false
   changed_when: false
@@ -13,14 +16,18 @@
 
 - name: message
   debug:
     msg:
       - "tensorflow not installed"
   when: tf_version.stdout == ""
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'tensorflow':'not installed'})}}"
+  when: tf_version.stdout == ""
+
 - name: check add_ons directory exists
   shell: find {{ ascend_install_path }} -type d | grep add-ons | wc -l
   register: add_ons_dir
   when: tf_version.stdout != ""
 
 - name: check add_ons directory contains libprotobuf.so
   shell: find {{ ascend_install_path }}/add-ons/ -type f | grep libprotobuf.so | wc -l
@@ -46,14 +53,18 @@
 
 - name: print npu_bridge without add_ons
   debug: var=import_npu_bridge
   when:
     - "'1.15.0' in tf_version.stdout"
     - add_ons_dir.stdout == '0' or add_ons_dir_protobuf.stdout == '0'
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'tensorflow':'OK'})}}"
+  when: import_npu_bridge.rc is defined and import_npu_bridge.rc == 0
+
 - name: test npu_device without add_ons
   shell: |
     if [ -f {{ ascend_install_path }}/ascend-toolkit/set_env.sh ];then . {{ ascend_install_path }}/ascend-toolkit/set_env.sh;fi
     if [ -f {{ ascend_install_path }}/nnae/set_env.sh ];then . {{ ascend_install_path }}/nnae/set_env.sh;fi
     . {{ ascend_install_path }}/tfplugin/set_env.sh
     python3 -c "import npu_device; from tensorflow.core.protobuf import rewriter_config_pb2"
   environment:
@@ -67,14 +78,18 @@
 
 - name: print npu_device without add_ons
   debug: var=import_npu_device
   when:
     - "'2.6.5' in tf_version.stdout"
     - add_ons_dir.stdout == '0' or add_ons_dir_protobuf.stdout == '0'
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'tensorflow':'OK'})}}"
+  when: import_npu_device.rc is defined and import_npu_device.rc == 0
+
 - name: test npu_bridge with add_ons
   shell: |
     if [ -f {{ ascend_install_path }}/ascend-toolkit/set_env.sh ];then . {{ ascend_install_path }}/ascend-toolkit/set_env.sh;fi
     if [ -f {{ ascend_install_path }}/nnae/set_env.sh ];then . {{ ascend_install_path }}/nnae/set_env.sh;fi
     . {{ ascend_install_path }}/tfplugin/set_env.sh
     python3 -c "import npu_bridge.estimator; import npu_bridge.hccl; from tensorflow.core.protobuf import rewriter_config_pb2"
   environment:
@@ -83,14 +98,18 @@
     PYTHONPATH: "{{ ascend_install_path }}/tfplugin/latest/tfplugin/python/site-packages:{{ ascend_install_path }}/ascend-toolkit/latest/fwkacllib/python/site-packages:{{ ascend_install_path }}/nnae/latest/fwkacllib/python/site-packages"
   register: import_npu_bridge_with_add_ons
   when:
     - "'1.15.0' in tf_version.stdout"
     - add_ons_dir.rc == 0 and add_ons_dir.stdout != '0'
     - add_ons_dir_protobuf.rc == 0 and add_ons_dir_protobuf.stdout != '0'
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'tensorflow':'OK'})}}"
+  when: import_npu_bridge_with_add_ons.rc is defined and import_npu_bridge_with_add_ons.rc == 0
+
 - name: print npu_bridge with add_ons
   debug: var=import_npu_bridge_with_add_ons
   when:
     - "'1.15.0' in tf_version.stdout"
     - add_ons_dir.rc == 0 and add_ons_dir.stdout != '0'
     - add_ons_dir_protobuf.rc == 0 and add_ons_dir_protobuf.stdout != '0'
 
@@ -106,13 +125,17 @@
     PYTHONPATH: "{{ ascend_install_path }}/tfplugin/latest/tfplugin/python/site-packages:{{ ascend_install_path }}/ascend-toolkit/latest/fwkacllib/python/site-packages:{{ ascend_install_path }}/nnae/latest/fwkacllib/python/site-packages"
   register: import_npu_device_with_add_ons
   when:
     - "'2.6.5' in tf_version.stdout"
     - add_ons_dir.rc == 0 and add_ons_dir.stdout != '0'
     - add_ons_dir_protobuf.rc == 0 and add_ons_dir_protobuf.stdout != '0'
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'tensorflow':'OK'})}}"
+  when: import_npu_device_with_add_ons.rc is defined and import_npu_device_with_add_ons.rc == 0
+
 - name: print npu_device with add_ons
   debug: var=import_npu_device_with_add_ons
   when:
     - "'2.6.5' in tf_version.stdout"
     - add_ons_dir.rc == 0 and add_ons_dir.stdout != '0'
     - add_ons_dir_protobuf.rc == 0 and add_ons_dir_protobuf.stdout != '0'
```

## ascend_deployer/playbooks/test/case_tfplugin.yml

```diff
@@ -1,7 +1,10 @@
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'tfplugin':'ERROR'})}}"
+
 - name: test if toolbox installed
   find:
     paths:
       - "{{ ascend_install_path }}/toolbox"
     recurse: yes
     file_type: file
     use_regex: yes
@@ -20,19 +23,23 @@
 
 - name: message
   debug:
     msg:
     - "toolbox or tfplugin not installed, please install first"
   when: ascend_dmi.matched == 0 or tfplugin.matched == 0
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'tfplugin':'not installed'})}}"
+  when: tfplugin.matched == 0
+
 - name: execute ascend-dmi -c
   shell: ascend-dmi -c | grep tfplugin | awk '{print $6}'
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ascend_install_path }}/toolbox/latest/Ascend-DMI/bin:{{ ansible_env.PATH }}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ ascend_install_path }}/toolbox/latest/Ascend-DMI/lib64:/usr/local/dcmi:{{ ascend_install_path }}/nnae/latest/opp/fwkacllib/lib64:{{ ascend_install_path }}/nnrt/latest/acllib/lib64:{{ local_path }}/gcc7.3.0/lib64:{{ ascend_install_path }}/add-ons:/usr/local/Ascend/driver/lib64/common:/usr/local/Ascend/driver/lib64/driver"
     ASCEND_OPP_PATH: "{{ ascend_install_path }}/nnae/latest/opp:{{ ascend_install_path }}/nnrt/latest/opp"
   when: ascend_dmi.matched > 0 and tfplugin.matched > 0
   register: tfplugin_status
 
-- name: print tfplugin status
-  debug: var=tfplugin_status
-  when: ascend_dmi.matched > 0 and tfplugin.matched > 0
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'tfplugin':'OK'})}}"
+  when: tfplugin_status.stdout is defined and tfplugin_status.stdout != ''
```

## ascend_deployer/playbooks/test/case_toolbox.yml

```diff
@@ -1,7 +1,10 @@
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'toolbox':'ERROR'})}}"
+
 - name: test if toolbox installed
   find:
     paths:
       - "{{ ascend_install_path }}/toolbox"
     recurse: yes
     file_type: file
     use_regex: yes
@@ -10,19 +13,24 @@
 
 - name: message
   debug:
     msg:
     - "toolbox not installed"
   when: ascend_dmi.matched == 0
 
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'toolbox':'not installed'})}}"
+  when: ascend_dmi.matched == 0
+
 - name: execute ascend-dmi -i
-  shell: ascend-dmi -i
+  shell: ascend-dmi -f -et 10
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ascend_install_path }}/toolbox/latest/Ascend-DMI/bin:{{ ansible_env.PATH }}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ ascend_install_path }}/toolbox/latest/Ascend-DMI/lib64:/usr/local/dcmi:{{ ascend_install_path }}/nnae/latest/opp/fwkacllib/lib64:{{ ascend_install_path }}/nnrt/latest/acllib/lib64:{{ local_path }}/gcc7.3.0/lib64:{{ ascend_install_path }}/add-ons:/usr/local/Ascend/driver/lib64/common:/usr/local/Ascend/driver/lib64/driver"
     ASCEND_OPP_PATH: "{{ ascend_install_path }}/nnae/latest/opp:{{ ascend_install_path }}/nnrt/latest/opp"
   when: ascend_dmi.matched > 0
   register: ascend_dmi_info
 
 - name: print ascend_dmi info
-  debug: var=ascend_dmi_info
-  when: ascend_dmi.matched > 0
+  set_fact:
+    test_dict: "{{test_dict|default({})|combine({'toolbox':'OK'})}}"
+  when: ascend_dmi_info.stdout is defined and ascend_dmi_info.stdout_lines|length > 1
```

## ascend_deployer/playbooks/test/case_toolkit.yml

```diff
@@ -1,7 +1,10 @@
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'toolkit':'OK'})}}"
+
 - name: test if toolbox installed
   find:
     paths:
       - "{{ ascend_install_path }}/toolbox"
     recurse: yes
     file_type: file
     use_regex: yes
@@ -20,19 +23,12 @@
 
 - name: message
   debug:
     msg:
     - "toolbox or toolkit not installed, please install first"
   when: ascend_dmi.matched == 0 or toolkit.matched == 0
 
-- name: execute ascend-dmi -c
-  shell: ascend-dmi -c | grep toolkit | awk '{print $6}'
-  environment:
-    PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ascend_install_path }}/toolbox/latest/Ascend-DMI/bin:{{ ansible_env.PATH }}"
-    LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ ascend_install_path }}/toolbox/latest/Ascend-DMI/lib64:/usr/local/dcmi:{{ ascend_install_path }}/nnae/latest/opp/fwkacllib/lib64:{{ ascend_install_path }}/nnrt/latest/acllib/lib64:{{ local_path }}/gcc7.3.0/lib64:{{ ascend_install_path }}/add-ons:/usr/local/Ascend/driver/lib64/common:/usr/local/Ascend/driver/lib64/driver"
-    ASCEND_OPP_PATH: "{{ ascend_install_path }}/nnae/latest/opp:{{ ascend_install_path }}/nnrt/latest/opp"
-  when: ascend_dmi.matched > 0 and toolkit.matched > 0
-  register: toolkit_status
-
-- name: print toolkit status
-  debug: var=toolkit_status
-  when: ascend_dmi.matched > 0 and toolkit.matched > 0
+- set_fact:
+    test_dict: "{{test_dict|default({})|combine({'toolkit':'not installed'})}}"
+  when: toolkit.matched == 0
+
+
```

## ascend_deployer/scripts/nexus.py

```diff
@@ -49,15 +49,15 @@
         self.root_dir = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
         self.config = f"{self.root_dir}/scripts/nexus_config.json"
         self.arch = platform.machine()
         os.environ.pop("http_proxy", "")
         os.environ.pop("https_proxy", "")
         with open(self.config, "r", encoding="utf-8") as f:
             self.config_content = json.load(f)
-        self.nexus_data_dir = os.path.join('/tmp', "nexus-data")
+        self.nexus_data_dir = os.path.join("/tmp", "nexus-data")
         self.nexus_image_name = self.config_content.get("image")
         try:
             self.nexus_image = glob.glob(
                 f'{os.path.join(self.root_dir, "resources", "nexus")}/nexus*{self.arch}.tar'
             )[0]
         except IndexError:
             raise FileNotFoundError("nexus image does not exist") from None
@@ -171,17 +171,25 @@
                 files.append(file_path)
         return files
 
     def _create_data_dir(self):
         try:
             os.makedirs(self.nexus_data_dir, mode=0o700)
         except FileExistsError:
-            shutil.rmtree(self.nexus_data_dir)
-            os.makedirs(self.nexus_data_dir, mode=0o700)
+            try:
+                shutil.rmtree(self.nexus_data_dir)
+            except OSError:
+                umount_data_dir_cmd = f"umount {self.nexus_data_dir}"
+                subprocess.run(shlex.split(umount_data_dir_cmd), shell=False, stderr=subprocess.DEVNULL)
+                shutil.rmtree(self.nexus_data_dir)
+            finally:
+                os.makedirs(self.nexus_data_dir, mode=0o700)
         os.chown(self.nexus_data_dir, 200, 200)
+        mount_data_dir_cmd = f"mount -t tmpfs tmpfs {self.nexus_data_dir}"
+        subprocess.run(shlex.split(mount_data_dir_cmd), shell=False, check=True)
 
     def _run_nexus(self):
         self._delete_nexus_container()
         self._create_data_dir()
         load_cmd = f"docker load -i {self.nexus_image}"
         subprocess.run(shlex.split(load_cmd), shell=False, stdout=subprocess.DEVNULL)
         run_cmd = (
```

## ascend_deployer/scripts/nexus_config.json

### Pretty-printed

 * *Similarity: 0.9702380952380952%*

 * *Differences: {"'codename'": "{delete: ['UOS_20-1020e_aarch64']}",*

 * * "'deb_os'": '{delete: [6]}',*

 * * "'rpm_os'": "{insert: [(13, 'UOS_20-1020e_aarch64')]}"}*

```diff
@@ -1,10 +1,9 @@
 {
     "codename": {
-        "UOS_20-1020e_aarch64": null,
         "Ubuntu_18.04_aarch64": "bionic",
         "Ubuntu_18.04_x86_64": "bionic",
         "Ubuntu_20.04_aarch64": "focal",
         "Ubuntu_20.04_x86_64": "focal",
         "Ubuntu_22.04_aarch64": "jammy",
         "Ubuntu_22.04_x86_64": "jammy"
     },
@@ -17,16 +16,15 @@
     ],
     "deb_os": [
         "Ubuntu_18.04_aarch64",
         "Ubuntu_18.04_x86_64",
         "Ubuntu_20.04_aarch64",
         "Ubuntu_20.04_x86_64",
         "Ubuntu_22.04_aarch64",
-        "Ubuntu_22.04_x86_64",
-        "UOS_20-1020e_aarch64"
+        "Ubuntu_22.04_x86_64"
     ],
     "euler_docker": [
         "docker-engine"
     ],
     "image": "nexus3:3.53.1",
     "rpm_os": [
         "CentOS_7.6_aarch64",
@@ -37,10 +35,11 @@
         "EulerOS_2.10_aarch64",
         "EulerOS_2.10_x86_64",
         "Kylin_V10Tercel_aarch64",
         "Kylin_V10Tercel_x86_64",
         "OpenEuler_20.03LTS_aarch64",
         "OpenEuler_20.03LTS_x86_64",
         "OpenEuler_22.03LTS_aarch64",
-        "OpenEuler_22.03LTS_x86_64"
+        "OpenEuler_22.03LTS_x86_64",
+        "UOS_20-1020e_aarch64"
     ]
 }
```

## ascend_deployer/scripts/prepare.sh

```diff
@@ -183,16 +183,16 @@
     elif [[ "${g_os_ver_arch}" =~ 2.9 ]]; then
         euler="eulerosv2r9.${arch}"
     else
         euler="eulerosv2r10.${arch}"
     fi
     local kh=$(rpm -qa kernel-headers | wc -l)
     local kd=$(rpm -qa kernel-devel | wc -l)
-    local kh_rpm=$(find ${BASE_DIR}/resources/kernel/ -name "kernel-headers*" | sort -r | grep -m1 ${euler})
-    local kd_rpm=$(find ${BASE_DIR}/resources/kernel/ -name "kernel-devel*" | sort -r | grep -m1 ${euler})
+    local kh_rpm=$(find ${BASE_DIR}/resources/${g_os_ver_arch}/kernel/ -name "kernel-headers*" | sort -r | grep -m1 ${euler})
+    local kd_rpm=$(find ${BASE_DIR}/resources/${g_os_ver_arch}/kernel/ -name "kernel-devel*" | sort -r | grep -m1 ${euler})
     if [ ${kh} -eq 0 ] && [ -f "${kh_rpm}" ]; then
         echo "install ${kh_rpm} when installing system packages" >>${BASE_DIR}/install.log
         rpm -ivh --force --nodeps --replacepkgs ${kh_rpm}
         if [[ $? != 0 ]]; then
             log_error "install kernel_header for euler fail"
             return 1
         fi
@@ -210,16 +210,16 @@
 function install_kernel_header_devel() {
     local have_rpm=$(command -v rpm | wc -l)
     if [ ${have_rpm} -eq 0 ]; then
         return
     fi
     local kh=$(rpm -q kernel-headers | grep ${kernel_version} | wc -l)
     local kd=$(rpm -q kernel-devel | grep ${kernel_version} | wc -l)
-    local kh_rpm=${BASE_DIR}/resources/kernel/kernel-headers-${kernel_version}.rpm
-    local kd_rpm=${BASE_DIR}/resources/kernel/kernel-devel-${kernel_version}.rpm
+    local kh_rpm=${BASE_DIR}/resources/${g_os_ver_arch}/kernel/kernel-headers-${kernel_version}.rpm
+    local kd_rpm=${BASE_DIR}/resources/${g_os_ver_arch}/kernel/kernel-devel-${kernel_version}.rpm
     if [ ${kh} -eq 0 ] && [ -f ${kh_rpm} ]; then
         echo "install ${kh_rpm} when installing system packages" >>${BASE_DIR}/install.log
         rpm -ivh --force --nodeps --replacepkgs ${kh_rpm}
         if [[ $? != 0 ]]; then
             log_error "install kernel_header fail"
             return 1
         fi
@@ -285,33 +285,30 @@
     fi
     if [[ "${g_os_ver_arch}" == "UOS_20-1021e_${arch}" ]]; then
         local have_rpm=1
     fi
 
     echo "install system packages are listed as follows:" >>${BASE_DIR}/install.log
     echo "$(ls ${BASE_DIR}/resources/${g_os_ver_arch} | grep -E "\.(rpm|deb)$")" >>${BASE_DIR}/install.log
-    if [ $(command -v docker | wc -l) -eq 1 ];then
-        log_warning "Docker is already installed on the system, and errors may occur when installing system dependencies"
-    fi
-    if [[ "${g_os_ver_arch}" =~ OpenEuler_22.03LTS ]]; then
-      yum install --skip-broken --disablerepo="*" -y ${BASE_DIR}/resources/${g_os_ver_arch}/*.rpm
-      if [ $(command -v docker | wc -l) -eq 0 ];then
-        yum install --skip-broken --disablerepo="*" -y ${BASE_DIR}/resources/${g_os_ver_arch}/docker/*.rpm
-        systemctl daemon-reload && systemctl restart docker
-      fi
-    elif [ ${have_rpm} -eq 1 ]; then
+    if [ ${have_rpm} -eq 1 ]; then
         rpm -ivh --force --nodeps --replacepkgs ${BASE_DIR}/resources/${g_os_ver_arch}/*.rpm
-        rpm -ivh --force --nodeps --replacepkgs ${BASE_DIR}/resources/${g_os_ver_arch}/docker/*.rpm
-        systemctl daemon-reload && systemctl restart docker
+        if [ $(command -v docker | wc -l) -eq 0 ];then
+            rpm -ivh --force --nodeps --replacepkgs ${BASE_DIR}/resources/${g_os_ver_arch}/docker/*.rpm
+            systemctl daemon-reload && systemctl restart docker
+            echo "install docker success" >>${BASE_DIR}/install.log
+        fi
     fi
     if [ ${have_rpm} -ne 1 ]; then
         export DEBIAN_FRONTEND=noninteractive && export DEBIAN_PRIORITY=critical
         dpkg --force-all -i ${BASE_DIR}/resources/${g_os_ver_arch}/*.deb
-        dpkg --force-all -i ${BASE_DIR}/resources/${g_os_ver_arch}/docker/*.deb
-        systemctl daemon-reload && systemctl restart docker
+        if [ $(command -v docker | wc -l) -eq 0 ];then
+            dpkg --force-all -i ${BASE_DIR}/resources/${g_os_ver_arch}/docker/*.deb
+            systemctl daemon-reload && systemctl restart docker
+            echo "install docker success" >>${BASE_DIR}/install.log
+        fi
     fi
     if [[ $? != 0 ]]; then
         log_error "install system packages fail"
         return 1
     fi
 }
```

## ascend_deployer/tools/hccn.py

```diff
@@ -46,16 +46,15 @@
     param = param.split("-")
     param_number = 8
     if len(param) == param_number:
         ips, netdetect_ips, gateways, netmask, roce_port, bitmap, dscp_tc, common_network = param
     else:
         print("parm size not right, exit...")
         raise Exception("param size not right")
-    
-    gateway_count = len(set(gateways.split(',')))
+
     info = {}
     gateway_set = set()
     npu_ids = []
     is_910b = False
     err_code, npu_info = get_statusoutput('npu-smi info -m')
     if err_code:
         raise Exception("npu-smi call failed!")
@@ -72,52 +71,52 @@
     for _id, (npu_id, ip, netdetect_ip) in enumerate(zip(npu_ids, ips.split(','), netdetect_ips.split(','))):
         matching_gateway, matching_network = get_gateway(ip, gateways, netmask)
         gateway_set.add(matching_gateway)
         info[npu_id] = {
             'id': _id, 'ip': ip, 'common_network': common_network, 'sub_network': matching_network, 
             'netdetect': netdetect_ip, 'gateway': matching_gateway
         }
-    if len(gateway_set) == 1:
-        full_connection = True
-    else:
-        full_connection = False
     common_info = {'netmask': netmask, 'roce_port': roce_port, 'dscp_tc': dscp_tc, 'bitmap': bitmap, 'is_910b': is_910b}
-    content = get_content(common_info, info, gateway_count, full_connection)
+    content = get_content(common_info, info, len(gateway_set))
     mode = 0o644
     fid = os.open("/etc/hccn.conf", os.O_RDWR | os.O_CREAT | os.O_TRUNC, mode)
     try:
         os.write(fid, content.encode('utf-8'))
     finally:
         os.close(fid)
 
     code, out = get_statusoutput("hccn_tool -a -cfg recovery")
     print(out)
     if code != 0:
         print("recovery hccn failed!")
         raise Exception("calling for hccn_tool failed")
 
 
-def get_content(common_info, info, gateway_count, full_connection):
+def get_content(common_info, info, gateway_count):
     content = ""
     macs = {}
     table_start = 104
     for dev_id in info.keys():
         err_code, mac = get_statusoutput('hccn_tool -i %s -mac -g' % dev_id)
         if not err_code:
             mac = mac.replace("mac addr: ", "").strip()
             macs[dev_id] = mac
     for dev_id in info.keys():
         table_id = table_start + int(dev_id)
         _info = info.get(dev_id, {})
         content += get_basic_defines(common_info, _info, dev_id)
         content += get_gateway_defines(gateway_count, _info, dev_id)
-        if not full_connection:
+        # 非全连接组网
+        if gateway_count > 1:
             continue
         if common_info.get('is_910b', False):
             continue
+        # 非模组形态
+        if len(info.keys()) < FIRST_CARD_IN_SECOND_GROUP:
+            continue
 
         content += IP_RULE_TEMPLATE % (dev_id, _info.get('ip'), table_id)
         content += IP_ROUTE_TEMPLATE % (dev_id, _info.get("common_network"), _info.get("gateway"), dev_id, table_id)
         content += IP_ROUTE_TEMPLATE % (dev_id, _info.get("sub_network"), _info.get("ip"), dev_id, table_id)
 
         for other_dev_id in info.keys():
             if int(dev_id) < SECOND_GROUP[0]:
@@ -194,18 +193,18 @@
     return_code = process.returncode
     stdout_str = stdout.decode('utf-8')
     stderr_str = stderr.decode('utf-8')
     return return_code, stdout_str + stderr_str
 
 
 if __name__ == "__main__":
-    err_existing = False
+    ERR_EXISTING = False
     try:
         if len(sys.argv) != 2:
             raise Exception("param size not right")
         main(sys.argv[1])
     except Exception as e:
         print("error happen!")
         print(e)
-        err_existing = True
-    if err_existing:
+        ERR_EXISTING = True
+    if ERR_EXISTING:
         sys.exit(RET_ERROR_CODE)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/get_k8s_version.yml` & `ascend_deployer/playbooks/roles/mindx.basic/tasks/get_k8s_version.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-- name: stat version
+- name: stat k8s version file
   stat:
     path: "{{resource_dir}}/k8s/version.json"
   register: version_stat
 
 - name: judge using old k8s version
   set_fact:
     use_old_k8s_version: true
```

## Comparing `ascend_deployer-5.0.0b8.data/scripts/ascend-deployer` & `ascend_deployer-5.0.0b9.data/scripts/ascend-deployer`

 * *Files identical despite different names*

## Comparing `ascend_deployer-5.0.0b8.dist-info/DESCRIPTION.rst` & `ascend_deployer-5.0.0b9.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `ascend_deployer-5.0.0b8.dist-info/metadata.json` & `ascend_deployer-5.0.0b9.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'5.0.0b9'"}*

```diff
@@ -28,9 +28,9 @@
     "generator": "bdist_wheel (0.30.0)",
     "license": "Apache",
     "license_file": "LICENSE",
     "metadata_version": "2.0",
     "name": "ascend-deployer",
     "requires_python": ">= 3.6",
     "summary": "ascend offline installer",
-    "version": "5.0.0b8"
+    "version": "5.0.0b9"
 }
```

## Comparing `ascend_deployer-5.0.0b8.dist-info/METADATA` & `ascend_deployer-5.0.0b9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: ascend-deployer
-Version: 5.0.0b8
+Version: 5.0.0b9
 Summary: ascend offline installer
 Home-page: https://gitee.com/ascend/ascend-deployer
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

## Comparing `ascend_deployer-5.0.0b8.dist-info/RECORD` & `ascend_deployer-5.0.0b9.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 ascend_deployer/__init__.py,sha256=3geaeGzhrlHQWFzpr3TqJSebV4Xzi1goFBjRH-QgqpQ,769
-ascend_deployer/ansible.cfg,sha256=_xFcFD4oavHhko4NCrmpx-9frb2Iyj0z3t7il0aPniw,348
-ascend_deployer/ascend_deployer.py,sha256=QhgLzjvP8Afnz09Eduh5xJupqxl2h3eYvtif3PlcrDw,7530
+ascend_deployer/ansible.cfg,sha256=NCJOn3Cpo3WS7iMosATJRcR_OaSQfXD7hIOLZ-NkiR8,371
+ascend_deployer/ascend_deployer.py,sha256=ub72laHRgn-Jkezm2RkSxFCiXcVJRbwVdN0MUXYa00o,7656
 ascend_deployer/ascend_download.py,sha256=p15pKv8Ge-W75w9sKufVnzvrBxw_DXrb4bb32qVWRVE,2145
 ascend_deployer/downloader_ui.py,sha256=mkdVdBwc5WoOP62740NApr0I3s-rDQEEzprxUaMfE5M,6023
-ascend_deployer/install.sh,sha256=7NNtHbL0s8RkLcxyj3higyXHDfm0DzZy63HPThkGVr8,4177
+ascend_deployer/install.sh,sha256=aWdW8nFCH5k2cvXaugb3b40N-EkoZmMbNYFUG07edn8,898
 ascend_deployer/inventory_file,sha256=enDa4J9rN3VFFf7lWTEP2cFr_hPZsvVQmZVaPaTN5lo,460
-ascend_deployer/jobs.py,sha256=GpYcyUGH4exharlll4gJIVHOP66Z0eufrU9LY2rwAwU,5090
+ascend_deployer/jobs.py,sha256=L58DVnwb0WXinANWTseAbR2pkruOD9Cdg7MpfZQp0U8,5375
 ascend_deployer/start_download.sh,sha256=xR8a9C34dzBRgLyNfjurvpA0OISpeF-rqG3guJO_fsQ,475
 ascend_deployer/start_download_ui.bat,sha256=S4Aporvo3W__1O77dLC7JY0y-v6I8petduDdM8gsNEQ,57
 ascend_deployer/utils.py,sha256=3A-J4RGiTXjn7qrnWjNdhiFYT8b67VJlDmvl5BBcYcE,5429
 ascend_deployer/version.json,sha256=HA6x_geHEIgQPolmzJ-qv1Zmt6ESu2S6xXnvn-gxAPk,54
-ascend_deployer/ansible_plugin/ansible_log.py,sha256=j9ZmsgtfY6gA8QHw-ipwYt9tsLbE3khxJC3S08_sfzk,13742
+ascend_deployer/ansible_plugin/ansible_log.py,sha256=5_hjwkWjJG2mlDY_P4IQVZVLsj2e16bhDNbdyMKR_tU,14646
 ascend_deployer/ansible_plugin/install_info.yaml,sha256=sv6NOIG0Ii2IRXCefbq2oCyz3BqAOG9r61FPg8JZ1fo,1123
 ascend_deployer/downloader/__init__.py,sha256=dkUA1a__TuPJAnwzar_z_njD2Jw8P9OGUhIiKZv05a4,2225
 ascend_deployer/downloader/config.ini,sha256=NvDponJ-1G_1iY2IpXhwP0DCdhBYpFRdPiwJH74OhzY,137
-ascend_deployer/downloader/deb_downloader.py,sha256=yZN5A3sQP-3oKXfNo05LuHU0wwVY2E1RjO9vITEnV4E,11014
+ascend_deployer/downloader/deb_downloader.py,sha256=-Z86jpSoDr3HfGkJL0NPIv5IvrsQUJ1JwJbuPTz_Ckc,11022
 ascend_deployer/downloader/dl_mef_dependency_downloader.py,sha256=oaCOb9K5S8kVa-s6wZJpQ3ts_Nz4HhndIXDlSc0OGm8,3923
-ascend_deployer/downloader/download_util.py,sha256=3fBP1xnZDzQZEplFBsaAZO5KURZamDos-13o2efK9nQ,18796
+ascend_deployer/downloader/download_util.py,sha256=skbpj81kNl5oDqa1ZZ1gpsRjFISHzvJp3px4iztj3aI,18816
 ascend_deployer/downloader/downloader.py,sha256=4marHbXRR-Mg1B2ayoXTXhL3TWX2Eqf0x97_PoS5ZzA,13079
-ascend_deployer/downloader/logger_config.py,sha256=EuUhFLUkMWkslKgNgzcDte_WxyJ6X6Lcv8gDPF2Se4o,4552
+ascend_deployer/downloader/logger_config.py,sha256=poczViEn7kdcbSU2FbmD4usux4VYJAjmZ2q6fBImWEs,4554
 ascend_deployer/downloader/obs_downloader.py,sha256=FSA2WP91NqBgDNCZiCJAwzYomihA2-4jhCraZPHRHtI,2839
 ascend_deployer/downloader/obs_resources.json,sha256=DY1ixcTYQRxFcWALN5C9WvPhRg5Hf7s91214Brs9MJ4,2730
 ascend_deployer/downloader/os_dep_downloader.py,sha256=OxvmabobxJ2Q7hfM7Iv8EHwej-rkiBDHYqTnPjTqxW4,4562
 ascend_deployer/downloader/other_downloader.py,sha256=IaiSB69KtNqCGCqO0ecj8q6YuS4RAopyqqIRGW4VUgk,14550
 ascend_deployer/downloader/other_resources.json,sha256=71S9vvoUol4vTdjkb5Rih7wftX2FxNaWEYKgwlISoms,2870
-ascend_deployer/downloader/pip_downloader.py,sha256=lFEfmAUJYXxJmcR266AKEylV2blF1y8QTU-H6f9xkWM,13377
+ascend_deployer/downloader/pip_downloader.py,sha256=_AsvTxaBP3Z6cZdOnc265l-2G4D3W9Zg8kh1Sk_08_c,13387
 ascend_deployer/downloader/python_version.json,sha256=9pSqHUoRuHczku4tbP66Io8q519P8zCnDbPd49mgX38,8754
 ascend_deployer/downloader/requirements.txt,sha256=6camZ9H2M60scc935IpL6edSsyKJNKVhN_tjX4fHwxM,1775
-ascend_deployer/downloader/rpm_downloader.py,sha256=KBFLBDltYR4HWh5ku5IIiSiRXP4lYMU-606r_GWiJEM,20876
-ascend_deployer/downloader/software_mgr.py,sha256=5JIjLKwSmkh6QjlXmLon_2AFjhd0_onJGvurhc45BBE,8430
+ascend_deployer/downloader/rpm_downloader.py,sha256=3k0KTnADUehbsvRu_324zidmL1C0Tk7p-mBL8V2UYI4,20157
+ascend_deployer/downloader/software_mgr.py,sha256=3h8Lw_4oY9d0TVSjecIZVpqjMsBKEllLCwuiGc1-ruA,8446
 ascend_deployer/downloader/version_match.json,sha256=MmfaS9IxeRVCvzpdS2l-9d_23v3KIqypACGRw6Y6SJw,462
 ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json,sha256=CZ6-sQmpwyZb1F0uifYkgLzLM1EqhJuj_jyhn_W6dlI,8690
 ascend_deployer/downloader/config/CentOS_7.6_aarch64/source.repo,sha256=MXAKWne-AouqA4H0T3YO1gmRCsOKwY-TeG5MbBDqff8,234
 ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json,sha256=X-S-xPgrlgGmVXpGBjdGWh0t1QLZRTkDMLql0PzWmf4,10223
 ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo,sha256=oOiLtW45sOuZZ_P_pugv7LhrEgs3uw_xrRY5-FOjNtM,371
 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/installed.txt,sha256=nKuC_VfjU73aukPARJMi1U9a9ZdUItqZCcvz0W_edaQ,43257
-ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json,sha256=Z4Qyn3_SFLYrrhApOUnA98OimISEcl0J4Kx9_wSrvWo,4596
+ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json,sha256=jTIBpH6S0OGfxdrVAALohDZCDe8RZ_FM9s5BObbdncQ,5838
 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/source.repo,sha256=eysNjtYexsTQGiWpLqXoN9BYfCgLxfQN8cjcb8GDQtg,131
 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/installed.txt,sha256=s_R0_DEUFrxq40paa3aDFxOeqFAiyq1G0K-kLOwAEMg,42707
-ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json,sha256=54rvT7MMq9gqOEeVsRo2eHfCoYLVN32JiVCRkC8rsPE,3668
+ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json,sha256=sax4N4lUPXYjrpou5RxCGY15enw0YqkiPIDa5_7xzjQ,5062
 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/source.repo,sha256=4C0abYxsv25uVugAAdc4mPhbMxiaO-4vN8TnNgwqBXY,65
 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/installed.txt,sha256=RABC9Ydam7O91w4uymLiO04HCDgSG8RigE_2u1Sx6Iw,65900
-ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json,sha256=43TNgHse2fYxbWu2Yjm_PIZrcsRCAaAOPpCWW27gWYg,6028
+ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json,sha256=mYdF8O-Bik74GYcedLlYikvBTp5TCheEodnTA96S_U0,9438
 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/source.repo,sha256=-4n539gqg17t4JRpUyqctcJ0eQK5-1KZuHqDFLvtKqM,130
 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/installed.txt,sha256=B1qfqvax5MY4ZBvzHa0z9cZNPgjymCcqOV9mDz-RdAE,42840
-ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json,sha256=ijfqWmNevX6JwNp7hHijKIRpfuMYtUjaFtqFsYTaa8A,4518
+ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json,sha256=QLPYS5jwlRv9Kg9evNBrOLpGYIvVCReXxkdc4c12rms,8487
 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/source.repo,sha256=Cvl3U3MpU0IQc8gTvS6HdkDGIzRQzKsWChIMQhfTEyQ,130
 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/installed.txt,sha256=JAcDXwKy_6MSFPVc_5ntA_JTlP3VpfWE0P6NHLlRECw,42208
-ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json,sha256=zTTYc2gZ7uokYNaIumr5QU0ssitOXsDSXpf0_xpmRhQ,3827
+ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json,sha256=fWf4ofYW-ytrertquqOiabAvs9xrkitdhCkm_yIwB20,8029
 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/source.repo,sha256=44o98hE2tl4xd0ScyHk89RYwk58p7Eq92qysQZ_PmgY,65
 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/installed.txt,sha256=sItZv2m9qFp8vdh6xsopvEQICxIsyKCWkrGMudbBmNI,60396
 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/pkg_info.json,sha256=vJFfEC0Kl2oWZ3ECObcqRhHkkommx15ed0SvlhC_-ew,3388
 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo,sha256=qzbPi9gTz9pPFmXH_7Vbp7saSm_ivgRK6DkMOkUORIc,264
 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/installed.txt,sha256=_wVdEw615qxHMyxH06QJPIuvBLapIG9r46oK6XY0pck,60964
 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json,sha256=paIq645CQ2wCSYSRvcKINTxJnfl-jM2jZh8DAyHYSvc,3201
 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo,sha256=ui74lUzSLFVRgr9NGZm0638JrJvflQNHtDbmvdbWDvQ,253
@@ -63,45 +63,45 @@
 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/source.repo,sha256=F17X4kGY5WKb76bn6wbLK8qSbV7c4qTJa44aJMgZ7Ao,445
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/installed.txt,sha256=kNV9sbRHNGfDPh44gJRfKeT_1ixx1G5AVsk2lF-rziQ,51351
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json,sha256=7w8QiW99KBuSANC613IVPImWsiNUAAySucQBdh_TbNA,5439
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/source.repo,sha256=koyb7uyQaYLNckSFx2dipEQME7k29Qz9YJYRo-UslvU,458
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/installed.txt,sha256=dTh1kpyfwd7wD2-6YypziUtVmDMBiLSOMQPaAuo10K0,43010
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json,sha256=zWvYiYFtRgB0w6TRznJ1bmPK13E-fsKP52-gyo3m0Ic,3220
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo,sha256=dckwsHk8V5ZZYeJBG5Y-_KE9lztKhBEn4Fi7rLAN6_g,445
-ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt,sha256=pvn_9ISn9UwCwLTuSanehgzyEamY80SGUC8jjtWdNCs,57488
-ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json,sha256=ekkYSxtur5m2PyKMyyEHpc1v_9JIvIzTWldbqAGxJYQ,2460
-ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo,sha256=FvnrmUSa31HWb0rHRYASmHQKmH8769lem8t0-XzBj00,186
+ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt,sha256=WfZIn1u2qhzTR2tJhECdiX1d6sCPgwWepEVBn5HBx-c,56970
+ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json,sha256=nxi3gwHX2cjC4Gdeh1L7WicmHGzL10F9eNI-n1Mag9I,3134
+ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo,sha256=6HDMnrFt-aUP60MEN6Tv5nJCokJcBvyS_jHmq8QT6dY,268
 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json,sha256=EioQ8UoZob8E_NEPJH0x3CvOI05Wr3ezJJxFxGyQzDE,4204
 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list,sha256=hDXHX8w0fwit1D2njIhhBTOjCzwehVkd5INGTmmwSFU,370
 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json,sha256=Xz2lcOo2wyeZ_NPrQa83UDvNN87uOK7nSQZ_0JU7Wg4,5718
 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/source.list,sha256=-ZN1Y__CqGtpqogO3QHVnOVl04MBxQvu9CQn3wNJt_I,352
 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json,sha256=RRiP8OF_dHEn1ery_e7Q7U9iHlJypeGg4OwGKmx15hA,5172
 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/source.list,sha256=8QbZP5aNc9uYxYVTe7WmeGYZljWPZ_Av6bvkgb4hwqE,366
 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json,sha256=zMxaixQq6kAzk7_E47lgS3W-cacp1SqGtkEZ6GpnqkE,6256
 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/source.list,sha256=Fpa9xHLXJBSoHonzvop98ucN4yOE2q9FAuu06UKHFL4,348
 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json,sha256=DWYwHqCM0lOl6maAIXuN9fN9CMu5LbskGQtOzyoJtr0,5891
 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/source.list,sha256=dVuItkYL-4PTn0tTbcBbObkaXOYD7JlBOid9LHoAlWk,366
 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json,sha256=M1FJ19iufi9kDn2J3r3eyddF0HCFR1KXnI0boZcLVBs,6644
 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list,sha256=CZWl_Rw_Qdy_qpekt40YqzeDtmS3GEjmsF-6HIntiGM,348
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json,sha256=DYMsA6_5rXyZ4F3LToIaZEmU78UndNestPVTQ5ui9YA,3637
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json,sha256=xbJVgd6Sh0O_KexpojcH51t-yNyKRr-TIzNBifqoIMs,3621
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64/resource.json,sha256=YCF4r-9K8D9QYYQhUm57q-0BPhRJrRzhhgnkqCtX0pw,3629
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64/resource.json,sha256=F1KcbMwldNXc9Xdd2bmjmjfgX499N5l8dOKr1g2jNlk,3613
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json,sha256=jxUaxUpLOoXfVo_MFvOY2Rf4WznE5NtVNvjTJcbVfRI,3709
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json,sha256=yAKoGfD3EqGAPCzPOmmjmjCP_yR11H5oKFpteliMspY,3693
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json,sha256=8eAobjXKq1G3laod-mZBZWy0MIM93MDTkc4Vgif8poA,3709
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json,sha256=9CAWQe66z18Z_X0ppg8jLliBfp_BjbcYUgVNk2DuxHM,3693
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json,sha256=QIWhWLjrVzEUVjWr9z68JyBLmGDoqRAie_K4c4afa18,3653
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json,sha256=4_J-wAwzAE58Ob_oBWwr0PGOlQhsUUR5skwiLfabEY8,3637
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json,sha256=UOnCZrLcPU0Hy_PGBayDxy62dtT7fmpg40BnLAgrW-g,3653
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json,sha256=MKDEQ6uEhZ5eATBhp8cAUnzW_bRds6F6ddlPbKHEo54,3637
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json,sha256=OgWoCRdv66DxgA2NdmM_JKHVLuU8ZvAouwRYZY72KMQ,3621
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64/resource.json,sha256=unHm5l0veqww9ZIzcPwdNIy3fEJk_Su7pEEleOx-Hq4,3629
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64/resource.json,sha256=I2Ilqx1bhchzU8xQNrDaabM-Mf9UuGs2qu23ZVCsK5E,3613
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json,sha256=RQfMdn3ImpoJTXFKL0ZIImiIkii7LybAi7o3cM39RgQ,3709
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json,sha256=qBTA9MSEfEKnh9emKnV9qBMjtMYcZRWNae3SOQKmngE,3693
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json,sha256=u-9iQnjYK8QHknA35ksxykdUKvGoLHtVzW0BNW2koNo,3709
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json,sha256=PGzq3OCj6hSQViZdZZ5d1-JTGltq8xrh1MPAoC8cqGA,3693
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json,sha256=R-49237wc3uofT2TbpYUIuSBee6hHj19VauJQuk6Z4I,3653
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json,sha256=xaLiTwoERyukIkybwbmYNhrKGxhBZoPUR2SIpnIORdI,3637
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json,sha256=UI79o1eT4FXm8ibeY4kb9gGdwLeQiz9oT19vtYMY3fI,3653
 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_x86_64/resource.json,sha256=Lq91KCxwj5uK7lyQ9B-xraEjzi8SUf71S1-ZaywMIM4,3637
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_aarch64/resource.json,sha256=Oi6tpz1laDHxCpbGjZvP1eP_U_GXrZzRXLy8f-6ACIw,3653
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json,sha256=arBEGi00sYcjDMJHPQA8UjB4EzdUE03Xun2BukoUMvU,3637
-ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json,sha256=EOmqMLkD0ajzYirHIUkKwf8zUjIOoouhUiG_I7iHCRw,3616
-ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json,sha256=9yq5tTBSnyERwRy8yNfXHyEYPcxNwOMjfSj4NDz6kDg,3584
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_aarch64/resource.json,sha256=YqPQIo9SIap4o6png8OuGr4A4uuw7qN2WpIkcrfVNfk,3653
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json,sha256=IsQ1PCQco4tYF1YVa73KyshKMySYIrFh7Grc70e_rIA,3637
+ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json,sha256=gQjCN4pz5zY4pSBrEzuhcToiAA9nfNFETM_DyxqM_oQ,4358
+ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json,sha256=4fT11nvQjraKs0lPOc4IIa2phj5Epf7ainXSuejaPTA,4324
 ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json,sha256=jmGTn41DdL-5zRhI_gGYDTonLDbYDEd7v9z8xw_kAog,853
 ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json,sha256=y1k3e_IYmaKi-MZ-HWpzyCBLOL4O0-b5LBK1Os4or9Y,847
 ascend_deployer/downloader/software/CANN_6.0.1.json,sha256=0ub3A-Z2gHgcxRnOhLOZ_kIs-91N7WaeeoQrROQdBVM,6044
 ascend_deployer/downloader/software/CANN_6.0.RC1.json,sha256=ntbdXO06JuoFc4K8-QR0NlapNqnIfNXEq7vFFtYEFTg,6358
 ascend_deployer/downloader/software/CANN_6.3.RC1.json,sha256=XKY96RaddcCytpumL-RAAvqgp7VZdd5N7TAa3h2yJKo,5435
 ascend_deployer/downloader/software/DL_5.0.RC1.json,sha256=3KtJsNus91RJbf4PEpA16iP3F6v0a6wI3eumDpRgQyw,84
 ascend_deployer/downloader/software/MEF_5.0.RC1.json,sha256=FC8X1k_m6MeY-wJGsIJM4U29bRUMtITebbzukZeat5s,85
@@ -113,158 +113,164 @@
 ascend_deployer/downloader/software/MindStudio_6.0.RC1.json,sha256=MK1ArxrjmC5XdWXv3i4bZ6tH4cMEYeCf5j0jQ6QDoYQ,48368
 ascend_deployer/downloader/software/Torch-npu_1.11.0.json,sha256=UQMLBvcgtnbnWv91-GRfZP0vJ82W3eifHNfAAMT1ePI,2890
 ascend_deployer/downloader/software/Torch-npu_1.11.0rc2.json,sha256=bb0bDdL4XRILfnFu4mpEg5asVXUGRls5uCNTwt98cHY,2906
 ascend_deployer/downloader/software/Torch-npu_1.8.1.json,sha256=BpRKP5Rfa5BEOG2n959ebvUWFQqVdLHDA8MxG8uqpLI,2895
 ascend_deployer/downloader/software/Torch-npu_1.8.1.post1.json,sha256=SK07iWwoeL7HiMy8uYsrNzW7tJmfOv-MtcaAz9MGUBo,2920
 ascend_deployer/downloader/yum_metadata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ascend_deployer/downloader/yum_metadata/create_yum_metadata_primary_db.sql,sha256=4TE3bYIpTQ0uFUhEHO94OBpU81WN3YygtrkUjd38DQw,1772
-ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py,sha256=cypQrOYhYRvhOAXGBbcYcHyVTaJC1d6GB6dylMnvnvw,11330
-ascend_deployer/group_vars/all.yaml,sha256=V9fcd1bWMasnu8zug9E4sdExb02yOuaOpBhl_V8FDY0,1709
+ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py,sha256=fi1rzqdF16qGLRKrLV6dK-DyLP_zi_vm8IvRWmE7Bco,11352
+ascend_deployer/group_vars/all.yaml,sha256=R5llGlUKfcwSqHw5-peOLhlNETQh56bGEfKQl-oyZp8,1870
 ascend_deployer/patch/selenium_firefox.patch,sha256=MD5-UZ717Hca32fdmKa21g_JnbxKRM4BlVx-U-EPALA,807
 ascend_deployer/patch/selenium_firefox_profile.patch,sha256=K89iaIG9x0RX9qO0_LXISXSGDsG9QdzgvflrQWsrqYk,1127
 ascend_deployer/playbooks/basic.yaml,sha256=Ou1DidGhODBKq82i31KLe1HpOjMqo320AJndcSL3yMQ,236
 ascend_deployer/playbooks/check.yaml,sha256=FGf3L5QqmSTxpS7C_Ofe0S13_0NroU10CAjlXXkB5dg,479
 ascend_deployer/playbooks/check_pkgs.yml,sha256=vFej41gd3l3fq8khqR6jtsLPw0NU9JM1POQpbx4qmzE,94
-ascend_deployer/playbooks/clean_nexus.yml,sha256=E68dBOSAPjZBrWkKl_RkBHDIUbYY0lRAD-uSstP83sU,203
+ascend_deployer/playbooks/clean_nexus.yml,sha256=EuikbLGDpzRJRMscLIfltXA9p2pLtJPe9mc2ey0CcQI,249
 ascend_deployer/playbooks/create_nexus.yml,sha256=0UjBWCHO5Mgxa8k4wxrzVu7Ox5WUXiZiXTwzhVlWIJM,611
 ascend_deployer/playbooks/create_user.yml,sha256=If1dyZgM2xEn34Mq2aVBg2W3uJWDefgJLnylkKyMkXg,1136
 ascend_deployer/playbooks/distribution.yml,sha256=javypj3rHcn6Rxx4kBqDx8MAkdbnqTJyZNE-w2fXz3A,663
-ascend_deployer/playbooks/docker.yaml,sha256=OjJ3rcnQRZ_aRsE-Pg1ygAcRFJzs1Vi7PMErFjxpoi8,672
+ascend_deployer/playbooks/docker.yaml,sha256=eWPUlkjONNAGMIPoD5hxHCs8iYPg1V0_-Zy7QYks5vQ,921
 ascend_deployer/playbooks/gather_app_info.yml,sha256=Bmhjybkgks8NKxwwyTJtGHXeJqbOW66hn9uByAt2xJE,1021
 ascend_deployer/playbooks/gather_facts.yaml,sha256=UtX8qT8HT0RIThtEFEPmMHUu8dVUYZTvfI-4pACA2O0,3487
 ascend_deployer/playbooks/gather_npu_fact.yml,sha256=sorWPdMf08gnqxV0_-sHUiB_audLdrxCgwali0epKUk,1019
 ascend_deployer/playbooks/harbor.yaml,sha256=_MLo4qg26_e9Nu1lVxK8zduhieyd1gY9oq7AfmJAuuY,121
-ascend_deployer/playbooks/hccn.yaml,sha256=hX6LLQxYvaB4NHN-GKbHzmFlyF1SsdUhi7LPnAJRkNQ,122
+ascend_deployer/playbooks/hccn.yaml,sha256=VtkSnfHyq7wL9WRZ1FAhK6mpBjSFPRle8LCqTy8TE-4,193
 ascend_deployer/playbooks/image_load.yaml,sha256=LnuzoVRFz2Tx9Iyl8tKFx_SihI-TtOqZjcyHOnCx9ig,134
-ascend_deployer/playbooks/k8s.yaml,sha256=Mwg6Z5QolEsJTfgdF_dVVFpo00jmZD0zxw7kuUsF6c4,2213
+ascend_deployer/playbooks/k8s.yaml,sha256=o0t1_IH6RkDmd3m9gflabGF9SqpZDG1rhadhn2Tpdic,2142
 ascend_deployer/playbooks/kubeedge.yaml,sha256=bcF_WC6RqCBTA38P-hNWeCvBP38yIS-MdB333e08Lok,85
-ascend_deployer/playbooks/mindxdl.yaml,sha256=w4KV2_Xy3408FilwEsjOnP-ECES6P8nT0SDm5rkISpk,1654
+ascend_deployer/playbooks/mindxdl.yaml,sha256=nckG_xc4BK9eR422mkRrj6jjpT6PsLUZuHEJbKD3bMM,2180
 ascend_deployer/playbooks/modify_user_group.yml,sha256=nFrPwxyL9wzrslWPcjz-w2mOZmqMrui4_-sPJmWpx3U,491
 ascend_deployer/playbooks/os_map.yaml,sha256=gvdLP3qgFyHOkB3afyUR4PhAhz4TMH-Ad9_AVG27oN8,225
 ascend_deployer/playbooks/os_map.yml,sha256=oZM6qaOYNbhJw3VvQ2o1V-lAQr5QJuKtPXUsftCQI3I,2065
-ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml,sha256=Az8oJzhsZLYh14r67nhykgb9tXONmDXfiHefyzUJ5tU,1073
-ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml,sha256=Az8oJzhsZLYh14r67nhykgb9tXONmDXfiHefyzUJ5tU,1073
-ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_aarch64.yml,sha256=CH05HXbqDV3zQddGY4krQyFODQuRhWwmmH3sKs9v_HE,1687
-ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_x86_64.yml,sha256=CH05HXbqDV3zQddGY4krQyFODQuRhWwmmH3sKs9v_HE,1687
-ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml,sha256=s1A2FkFxrY3IVsJHHmplmCGlU7Cum9q4j5-lXKg72pc,1076
-ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml,sha256=s1A2FkFxrY3IVsJHHmplmCGlU7Cum9q4j5-lXKg72pc,1076
+ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml,sha256=nXMok4k-2PZBhv0JKbsP6yRiesABOdB_uEHqmH72d5E,1056
+ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml,sha256=nXMok4k-2PZBhv0JKbsP6yRiesABOdB_uEHqmH72d5E,1056
+ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_aarch64.yml,sha256=FGUOd26iZV-tzjYlY09vDDvN0HXXHC2T2pVbd0eHUD0,1653
+ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_x86_64.yml,sha256=FGUOd26iZV-tzjYlY09vDDvN0HXXHC2T2pVbd0eHUD0,1653
+ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml,sha256=eXZ-OCGV9uR8NUuJssaXCDBsRgk-Ja3As7RNbCMotFI,1652
+ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml,sha256=eXZ-OCGV9uR8NUuJssaXCDBsRgk-Ja3As7RNbCMotFI,1652
 ascend_deployer/playbooks/report.yaml,sha256=dUjp7DIOhyOGavCdvP9W-da1sRDWbDjZ4lVJBXuxtMc,422
 ascend_deployer/playbooks/set_facts_cache_permission.yml,sha256=vMTb7wIDN5utqsrGd8myI2l8U-hQVloe-AJZIrJTAC8,139
 ascend_deployer/playbooks/sync_time.yml,sha256=jiN-5XLWhK8YCkP8A4_h9ay4pDgDrWtvgxqpIgsSW-o,349
 ascend_deployer/playbooks/task_set_custom_fact.yml,sha256=gVsxg5vZVqOufhDDS77PLegbIG7mK-5Iyha-op9Fhqs,6051
 ascend_deployer/playbooks/uninstall_mef_kubeedge.yaml,sha256=n3PyVh4k72KzXuJEbBvtWGRcSGV_iDloiDp5TpJHFBI,155
 ascend_deployer/playbooks/uninstall_mef_releate.yaml,sha256=TZraFst-Ykc0wHKAoswYe3tW2a_yUGIS4CjFt631UHc,246
 ascend_deployer/playbooks/facts/app_info.fact.j2,sha256=KdVRCDzhLtGMqpKo1USq4YXrS3rxi-aSoKeV02YZT1A,5199
 ascend_deployer/playbooks/facts/npu_info.fact.j2,sha256=JW2YROvpmeepYvP0umQvx4xeZv3K69DY5jeatnKdxF0,6392
-ascend_deployer/playbooks/install/install_atlasedge.yml,sha256=wJ7bJESZnRWwV2qlmFmgSN8RexVxWr1rnhv2Ht3Ut3c,549
-ascend_deployer/playbooks/install/install_device_plugin.yml,sha256=OU6hUOy34hxms5tmSdeWZ4YOixXgxdvCpJ3KacL4vV0,107
+ascend_deployer/playbooks/install/install_ascend-device-plugin.yml,sha256=OU6hUOy34hxms5tmSdeWZ4YOixXgxdvCpJ3KacL4vV0,107
+ascend_deployer/playbooks/install/install_ascend-docker-runtime.yml,sha256=sIK2tC3pr9zkw1Vl2IeZ8unbYXMNbr0pZ6hldsmluqg,109
+ascend_deployer/playbooks/install/install_ascend-operator.yml,sha256=I5v148ZJAtrn1enEi0aVSUaQ4XRAjYOxIDfx8FDkLrk,110
+ascend_deployer/playbooks/install/install_atlasedge.yml,sha256=YGrqgIlpG1lJzVfa6hqfQ8iuj8bQPcF2xsqkyNQvOp8,549
 ascend_deployer/playbooks/install/install_docker_images.yml,sha256=nQzKJxuabMmlxAMrsHfbyTxKD0vxz5iLAkMc3mgGNTw,467
-ascend_deployer/playbooks/install/install_docker_runtime.yml,sha256=sIK2tC3pr9zkw1Vl2IeZ8unbYXMNbr0pZ6hldsmluqg,109
-ascend_deployer/playbooks/install/install_driver.yml,sha256=naawG2xnqE8qJTfsRhyJWsTkxWSM8rYaP_jvEw2ZCTk,1265
-ascend_deployer/playbooks/install/install_firmware.yml,sha256=kqUprZ3ZOY0USinSuOdcSUw2dJ09A9NtHCZ9hG9Y08c,1298
+ascend_deployer/playbooks/install/install_driver.yml,sha256=AOd48Sc0QWIGuJ6R32IAHi5ld1BQVMKCsRZrPDg1s4o,1264
+ascend_deployer/playbooks/install/install_firmware.yml,sha256=L8C7WRQv9991bjt7QDzNANGMAElJzyqHpjrf-SyCXGI,1297
 ascend_deployer/playbooks/install/install_gcc.yml,sha256=wzsJ1usrYuSG1tvFe829VWRbAsqmyVKDa41F9bfWd54,896
-ascend_deployer/playbooks/install/install_ha.yml,sha256=h9JVzO2U7h_Eql7Qjc8IPGjAt9xhedzSA2NjITKBx4g,521
-ascend_deployer/playbooks/install/install_hccl.yml,sha256=cwnYSmZ16cbjUQIOIYkFwRIGPOKYuqsAE1P31QlphN0,99
-ascend_deployer/playbooks/install/install_ief.yml,sha256=8og4Qo_pYBuRxYPclhZGzh-b1qLFGWd8IyNUCVjxmBs,427
+ascend_deployer/playbooks/install/install_ha.yml,sha256=9eiIb_7LKcsbKfnd1Kxlp7fij_Oh-sMAZAShwEI66IU,522
+ascend_deployer/playbooks/install/install_hccl-controller.yml,sha256=cwnYSmZ16cbjUQIOIYkFwRIGPOKYuqsAE1P31QlphN0,99
+ascend_deployer/playbooks/install/install_ief.yml,sha256=swvZfZp6ujvRQlV4IvAUfVUCSiBsNMLCXPKlgEXpKDE,427
 ascend_deployer/playbooks/install/install_kernels.yml,sha256=GLwjT3L0VAKJtcdOC_zcbs8Zb95-a-jZEnRRDGDGoAg,216
 ascend_deployer/playbooks/install/install_mindspore.yml,sha256=ES_cvT_lIMsxdW0NVsQMgoxUdu1a-JZ5X91npdEGGuA,927
 ascend_deployer/playbooks/install/install_mindstudio.yml,sha256=Az3GPggTWMyNZSLGT_Z2SqjX_rXzUfjy-T0erOygRt0,9154
 ascend_deployer/playbooks/install/install_nnae.yml,sha256=Uxp-GvbbdcBe7c7vHRnuS10u804G0z2WA867bfMSYwk,96
 ascend_deployer/playbooks/install/install_nnrt.yml,sha256=pZ9uamO_fg25jmOOmH7ka9eRCztniDpWgoy4sNuEEJc,210
 ascend_deployer/playbooks/install/install_noded.yml,sha256=kBFswQNjODf6ULxhFPBwKzoKyzjM-TN89tFKAuwUlvs,100
+ascend_deployer/playbooks/install/install_npu-exporter.yml,sha256=Ky0j_AypNX-YgBr480eUtZy3sR-EnT9pmKPf5P3G6Wk,107
 ascend_deployer/playbooks/install/install_npu.yml,sha256=WP7-_H0GRGoM2ei9Lb05exf_LWIBiEZ65533Ia5PTIc,1398
-ascend_deployer/playbooks/install/install_npu_exporter.yml,sha256=Ky0j_AypNX-YgBr480eUtZy3sR-EnT9pmKPf5P3G6Wk,107
 ascend_deployer/playbooks/install/install_python.yml,sha256=62I2D8DdE178Mum9k32gTFCNPXsMeGB5bA0RbSIe5iM,105
-ascend_deployer/playbooks/install/install_pytorch.yml,sha256=-J7lrbOZlYu_0K4q3U6iWnuVKfUDsJwouPNx3O6myvY,2523
+ascend_deployer/playbooks/install/install_pytorch.yml,sha256=zUBDP_jWJrVdJkC8RyddsFL7aPL0cagkTNE1eW2rr_0,2524
+ascend_deployer/playbooks/install/install_resilience-controller.yml,sha256=WOkqOqkm_YHJcdlj5Ri5byFUFVOo9IcorNFpx1XTqqE,116
 ascend_deployer/playbooks/install/install_sys_pkg.yml,sha256=PowQ8gJeftXF4_SxZKiqx2p7TZyct_BupE83IsHrIVQ,452
 ascend_deployer/playbooks/install/install_tensorflow.yml,sha256=0boJQsq64VO8-jTnZ9oKLTm4H6UZtQwGo8fbqsYn3kE,3280
 ascend_deployer/playbooks/install/install_tfplugin.yml,sha256=gVqt5EkpXApkLxeG8KBx87oGraCpkF3hfgoJenXSsAM,104
 ascend_deployer/playbooks/install/install_toolbox.yml,sha256=V5aXG6MHAyNbh1N6HQF1h5E69yBEwz8MsZMT7LBuwxU,102
 ascend_deployer/playbooks/install/install_toolkit.yml,sha256=dkg6uB8hWXjG5SGXxNbRzDHlLLOw_YauhGMi1DE3Erc,216
 ascend_deployer/playbooks/install/install_volcano.yml,sha256=rA-OvYCbwbF_vkW3LfAppew5skvWa6GX6DyTLqopTAM,115
 ascend_deployer/playbooks/install/task_atlasedge.yml,sha256=3759ZqrIGmYoCFEENheucZ-VR1WSlJ63-4uthxic_ps,1456
 ascend_deployer/playbooks/install/task_cmake.yml,sha256=ue2t4_13xOEt9nRbEt6iCRHemHDH8_FaNz4doUAfhq0,663
 ascend_deployer/playbooks/install/task_dl.yml,sha256=x0XG9ZolQf2IIsrrC1qAhWO_QCAsIezXDKZOoZpPwpM,653
 ascend_deployer/playbooks/install/task_docker_images.yml,sha256=16iwil91p9Xo0l3dBZruEo-RotRpBEJsAWxjyCJLrPg,818
 ascend_deployer/playbooks/install/task_driver.yml,sha256=sb3MuzsVmFLqIRDc-Dzu96QZKojtT_ojz_QPSl3gBMY,239
-ascend_deployer/playbooks/install/task_driver_bcinux.yml,sha256=zpRde0_77c3fiFzW6uXNyfiT4BjZuq9JLQn8smMeXAI,6360
-ascend_deployer/playbooks/install/task_driver_common.yml,sha256=FCQPCBggiuBzPLuuUc1mIXyV7YIiE7hpJbOGOBBu79o,6443
-ascend_deployer/playbooks/install/task_firmware.yml,sha256=OKEbLYcmWD440J3HE6MnPYEQnWK__Zo7XDzQiUuklxY,5660
+ascend_deployer/playbooks/install/task_driver_bcinux.yml,sha256=BjBz1cNW4UfPtGKhKv9nmlyw2joPrkgRzaP2iqW4evQ,6278
+ascend_deployer/playbooks/install/task_driver_common.yml,sha256=YjobOrt_04lDTM9aZ7Pyg0LTduWH_YxnxLQxP-6TVwM,6361
+ascend_deployer/playbooks/install/task_firmware.yml,sha256=DaCmyoMiIcmzoeNluUayxiHkrbDJRbaxuAUFpjyikuw,5578
 ascend_deployer/playbooks/install/task_gcc.yml,sha256=nPcCmo6N30E00uV9-8vpokgLA06uetpbc81Whfl_yas,2210
 ascend_deployer/playbooks/install/task_get_npu_scene.yml,sha256=aa6P4mAcn9ExFxEwCOyg8leM7dssZbQC3FWMo-c_OdQ,3055
-ascend_deployer/playbooks/install/task_ha.yml,sha256=fLGyKt19WtdX9G6qbcyDxf8z3F4oykEeQyRsWX3_xM4,1227
+ascend_deployer/playbooks/install/task_ha.yml,sha256=csnZk9qMlMi3-1MDMl5Fnl9NUtKeZ-TvgSqgr1XQihI,1227
 ascend_deployer/playbooks/install/task_ief.yml,sha256=M-BG1Imq-9jfQ0JR4Scy7l9xlld1J5YWYp3sKQNFvEA,670
-ascend_deployer/playbooks/install/task_ief_a500.yml,sha256=pksT6Zd940oASIdjCO-j4hNhr4RqvikNsrQ6NPiDfoI,2793
-ascend_deployer/playbooks/install/task_ief_a500pro.yml,sha256=jjFT8edQB6ff7vWosWmdd98Pwza8L9RmU3haEQDHjRY,1681
-ascend_deployer/playbooks/install/task_kernel.yml,sha256=a7i2WhK6d-zCO9R5E8WI1frktRMcZBoxl0KATzXxv3s,1395
-ascend_deployer/playbooks/install/task_kernel_euleros.yml,sha256=AAtwILRPMJhFjfSbiDDZRk_ELfqgVBcJSsUMJQp4gLw,1317
-ascend_deployer/playbooks/install/task_kernels.yml,sha256=3KdyeVtXrxIDFeM2d4oQGaGl5ipzv8v-n23ksSDdaIY,9161
-ascend_deployer/playbooks/install/task_mindspore.yml,sha256=8Zn3z22X6xjd57rK-OZVO_iIEomsMyAlfYJbkvlbTyU,2044
-ascend_deployer/playbooks/install/task_nnae.yml,sha256=HoDgfzTMD4Qd9pySHQ-BZGn0gfIaUbJ61PZO6Q9ZU9c,3890
-ascend_deployer/playbooks/install/task_nnrt.yml,sha256=4UGmUGLZDfY4hklyL0WrdrJUHxALARLYIIms9DERp4c,3890
+ascend_deployer/playbooks/install/task_ief_a500.yml,sha256=yguTfoZxiVjeeCNjdoB8bZNRrPimzjGuaM3fUo4nET4,2777
+ascend_deployer/playbooks/install/task_ief_a500pro.yml,sha256=Ow70QwooJge5P8NeFE17UuWx2S2Y2sWVZ6ZWbXuYBJg,1665
+ascend_deployer/playbooks/install/task_kernel.yml,sha256=CLs5wxnsJtdWb7LjWnrpsj8KqzVH8Ynn9H-H5gNnTdc,1337
+ascend_deployer/playbooks/install/task_kernel_euleros.yml,sha256=OYbrDSOwzkOCc1N3Qw-oh1ESO3V1NMNM9hN1tj8KVWw,1242
+ascend_deployer/playbooks/install/task_kernels.yml,sha256=7uy42cNwlPcraZnANBuh32OIrQuhY3C6TFdMKzV6oj8,9377
+ascend_deployer/playbooks/install/task_mindspore.yml,sha256=glCXgIyjT7AVv18uaZLXoO7ecTf3AlPkTD1_fHiJuXU,2083
+ascend_deployer/playbooks/install/task_nnae.yml,sha256=lTZyG42HjrQF0s3yz0JVtZB_fD4W_7DXqcw7EKeUJGA,3767
+ascend_deployer/playbooks/install/task_nnrt.yml,sha256=6iARF8Dx4W7wR_v2ZInAAmHOTfBfH7_X0GofUXLg-4w,3768
 ascend_deployer/playbooks/install/task_protobuf.yml,sha256=wisHWXln-3KJNKNAEujdEyG4R34xd8tPie9C1JpoEPU,709
 ascend_deployer/playbooks/install/task_python.yml,sha256=8757_kb8MqLYikXQGtuTVYt6dtQGqidk9hutOUIJkUk,3209
 ascend_deployer/playbooks/install/task_pytorch.yml,sha256=M9g3OQLMDUpQrwNvyK7nk_XiybgB15SNn0sOVevj7ec,1265
-ascend_deployer/playbooks/install/task_sys_apt.yml,sha256=NtrrpMQyyUnCJJXiAkCmVBDUV7dkqML77mqCFb_JPb8,1894
-ascend_deployer/playbooks/install/task_sys_dnf.yml,sha256=6_TLVJcUjK7uHKERjuVlkQ9OA5Ico2SnEpjBkVtfkEo,2108
+ascend_deployer/playbooks/install/task_sys_apt.yml,sha256=jYzG3GbYszcfKXpaStIt-dQyN21847c4RKfXddJGseM,1812
+ascend_deployer/playbooks/install/task_sys_dnf.yml,sha256=An4VWAJtICsMYPBDMhYPnnW9S6Jy4ZwIbUYaXCo-TDI,2263
 ascend_deployer/playbooks/install/task_sys_pkg.yml,sha256=yQt__pF0q_6OtiSQanMU71U1prFmg2Jql96yJv9ACi8,3230
-ascend_deployer/playbooks/install/task_sys_yum.yml,sha256=2mu3kTDExcLp9f5cJN_I9ypGiGI5x7XaOFaiQPCuh5I,2112
+ascend_deployer/playbooks/install/task_sys_yum.yml,sha256=Ke1BoXmFSDAvEsY-5epfsKJ_XituEQAuFMvMDI3RkYg,2267
 ascend_deployer/playbooks/install/task_tensorflow.yml,sha256=-JHHIg7YlvxPHe7zzDn3pXY2hbRH9in_21SmuWOHuIA,1073
-ascend_deployer/playbooks/install/task_tfplugin.yml,sha256=UtqDG8tiUFhcj9hFoF0lgDer_se3xM6oyu1gw2pxNEY,4120
-ascend_deployer/playbooks/install/task_toolbox.yml,sha256=cU2OihHbFff6Gx2gm4a977zMyIkzkuUau2znu6GT9Lo,3426
-ascend_deployer/playbooks/install/task_toolkit.yml,sha256=f_h_S3JJZykTviifDNZeU8fkWKnamwd7S7LEreoH1h8,7662
+ascend_deployer/playbooks/install/task_tfplugin.yml,sha256=jC4qegIKP8GP_qcB0M8eS0dXenpoQ1qlPFJ2QFDn374,3997
+ascend_deployer/playbooks/install/task_toolbox.yml,sha256=an715FHLzScQX2trjxRMAWcLc5R2LPpMki7dGj-Rgqo,3262
+ascend_deployer/playbooks/install/task_toolkit.yml,sha256=qWqJXt3g1Cx7rbww7D2JEg2_KBxNHgz8rg5m9cRQUMo,7416
 ascend_deployer/playbooks/install/patch/install_nnae.yml,sha256=Bjt_L7j-afhIo4wNzHYz-x8tGdk4JJZDzEjI_bTEgU0,102
 ascend_deployer/playbooks/install/patch/install_nnrt.yml,sha256=xBqvjCC-rxEtPppD9YyvIV85EGCNzrzqluVH6lb3kc8,219
 ascend_deployer/playbooks/install/patch/install_tfplugin.yml,sha256=aly9mNlv0lFBjLNpyS_IhiFJiRs3l4Ob3ImtAJcsavI,110
 ascend_deployer/playbooks/install/patch/install_toolkit.yml,sha256=K4ZbG5y58eheZm6u7G6di8vbmZUs2pLVOIWfUtYXwTs,225
 ascend_deployer/playbooks/install/patch/rollback_nnae.yml,sha256=8ZcPKniMaYMUS5LvCRrMf2kuAHPJnnnI6p-XzryA4IU,106
 ascend_deployer/playbooks/install/patch/rollback_nnrt.yml,sha256=YzUDHNq4aINfO3T4Fy6jQYiM1R4D9kE3r9xTipia9qM,106
 ascend_deployer/playbooks/install/patch/rollback_tfplugin.yml,sha256=w7KvXXOjckJpCdxRinjdNLM9QslTwsm7kddO-2a8CT0,114
 ascend_deployer/playbooks/install/patch/rollback_toolkit.yml,sha256=IzqjJTqQg3FMTbQB1ZZ3GNk4-nLb_bifyWLyjKgGvoY,112
-ascend_deployer/playbooks/install/patch/task_nnae.yml,sha256=7WQdjMZQf1UXe72LYec-d_ePx5xoMlmQCCRN0WDRRIo,1375
-ascend_deployer/playbooks/install/patch/task_nnrt.yml,sha256=wwp4OcbYyFshKAkAL68BvV_yo-fnnLCxDpkGE126qnE,1375
-ascend_deployer/playbooks/install/patch/task_rollback_nnae.yml,sha256=fFJjCTuUpWpQaCRWelpS0WC9FsUy0vro_s1uLszKNb4,675
-ascend_deployer/playbooks/install/patch/task_rollback_nnrt.yml,sha256=L2FnKRSwugurYx8kVu7P-FXTF3EmWLI1Q2OZ55mLh70,1653
-ascend_deployer/playbooks/install/patch/task_rollback_tfplugin.yml,sha256=furf3k_1GTSUgigXJ4Gg1MWgaNOKlGX3gFiWqE5a4uY,734
-ascend_deployer/playbooks/install/patch/task_rollback_toolkit.yml,sha256=KpCuIa1zb7CZCIa5aghNBAj_JoINByXEOJXvYfWRa8M,1743
-ascend_deployer/playbooks/install/patch/task_tfplugin.yml,sha256=-2jZ1PjIhjNWWQkI9ZQkOCcIPH7sl6ZFJVjKCmGUwyk,1438
-ascend_deployer/playbooks/install/patch/task_toolkit.yml,sha256=q9lLBI3fs-8Y5Utg7Ihjy5J-8T5l1ypJh156JRiGNys,1311
+ascend_deployer/playbooks/install/patch/task_nnae.yml,sha256=_aw_K0OL3HqgkxwQvspwi_FO-WSfX0EBElx0kzEIK14,1334
+ascend_deployer/playbooks/install/patch/task_nnrt.yml,sha256=28AL2dxSVc_2wkeBcfIo_nRJa92jMFe1gBlEDKROf4I,1334
+ascend_deployer/playbooks/install/patch/task_rollback_nnae.yml,sha256=6RhbzR02J2LKFtXgRHH5yt6ua8wR_WWG0Aqcz1D4Fqc,634
+ascend_deployer/playbooks/install/patch/task_rollback_nnrt.yml,sha256=ok-qSsU0t0E4jR3jLhENkFuav014Hr-zFwBLYvtyj-M,1651
+ascend_deployer/playbooks/install/patch/task_rollback_tfplugin.yml,sha256=Sj0CzdFv84Pdf5gUq0uS4whXiEyarUDw2eifZXAmeCk,693
+ascend_deployer/playbooks/install/patch/task_rollback_toolkit.yml,sha256=Ow5puL6Vu5K3sQ7l4-222otav_Gah8Uw1gqYCOvLjTA,1661
+ascend_deployer/playbooks/install/patch/task_tfplugin.yml,sha256=cAlpOw-VVMm_MJ2sqtnngE8V7VuB8SqlFxDG6PZ3NCU,1397
+ascend_deployer/playbooks/install/patch/task_toolkit.yml,sha256=-q2ajokPjjbsbI-GXod3Ac2OH_tZ_1nkEnmw_VHLm08,1270
 ascend_deployer/playbooks/process/process_check.yml,sha256=iDv0yzMTVaBYtMEZpditZr5Pf2xECbxhTMl7TXgPijg,369
-ascend_deployer/playbooks/process/process_install.yml,sha256=fiMQcb33B26MErbu5mnnn93OjVeAur965G_kf8CFUBY,3155
+ascend_deployer/playbooks/process/process_install.yml,sha256=FN23bW40vP6wfpcRcbwWisnFnKPp_f5G3-QeYXzObn4,3539
 ascend_deployer/playbooks/process/process_patch.yml,sha256=V6zDjtcRbkwew51LTUvbd-HmvgD7ojnCjSyMNTv-1V0,783
 ascend_deployer/playbooks/process/process_patch_rollback.yml,sha256=do01GGNQJRQXMbWdBpktQreDfI4GIIIJtOLuVlsIg88,787
 ascend_deployer/playbooks/process/process_scene.yml,sha256=tJsnA2JKzd5_W2JJ57TqdljcPjy_S5AvJGSTqhUJV48,2144
-ascend_deployer/playbooks/process/process_test.yml,sha256=qq5GizvizDfZcioh3T0uwqqeIU_NvR1cMZ8_cSvkaoM,969
+ascend_deployer/playbooks/process/process_test.yml,sha256=ZwAZx62Tr85jRZU3jOjg23hReUQlqgPk5taZ0xIFpNM,1049
 ascend_deployer/playbooks/roles/mindx.basic/defaults/main.yml,sha256=O8bMeN1kpRuHIr9qqpKnI3JhULaafjTpnVeVYVnB-WU,310
 ascend_deployer/playbooks/roles/mindx.basic/files/space.sh,sha256=sweRsZwzkCcoCWy5iWd2msj4oJdop3OraLOde-vytG0,1258
 ascend_deployer/playbooks/roles/mindx.basic/tasks/check.yml,sha256=nxX9FqpRjCMoxl5eE4kWRVRPjxcsyp0BG0VnQSXXBhg,4154
-ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml,sha256=pAdpt8prs3dVHLr6aoC0S5rkBbRe1tSAYykOMnG2ffg,1437
-ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml,sha256=HeWb-d16GqoIrYyG8iWLnbd7UQas6NJO2zB2e-HCC6U,4660
+ascend_deployer/playbooks/roles/mindx.basic/tasks/get_k8s_version.yml,sha256=m3m0nVd2FUmp25DsnRAIGXWQJHZtwnP8xNh4bm1dLH4,702
+ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml,sha256=kVD56Yh2ZIZU9k2pVCIVzLoAULmKie0iFJvy1z6DSRk,2170
+ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml,sha256=_kX7kQiDoVyzZJpk2r84_69iPohjpdPi2v3zqsDEq_g,4723
 ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_status_check.yml,sha256=NYYrJKbJwsDC_mqbDhOKZrbQxYj73gwpYnDVPfxfDXo,4892
-ascend_deployer/playbooks/roles/mindx.check/defaults/compatibility_map.yml,sha256=wu5Cc2y1_aokTKONPg2HCdY1baGIWK46gemDD_AbJf0,10079
-ascend_deployer/playbooks/roles/mindx.check/tasks/compatibility_check.yml,sha256=_KWeRtBO2e2vBeflAtDUyJxfaE70bWvxO1jNx1hORXE,363
+ascend_deployer/playbooks/roles/mindx.check/defaults/compatibility_map.yml,sha256=tJtzwJhhKR8I_7xaSe37ItfN12ERhOvqBb9kvm4eajs,12487
+ascend_deployer/playbooks/roles/mindx.check/tasks/compatibility_check.yml,sha256=ZSUXe5ifcgEI_kVGuatvm-VPRJxpkxAMA0kPAFqpG1o,335
 ascend_deployer/playbooks/roles/mindx.dl/README.md,sha256=zVYAP3TfVYfVeqkuiCUs0hnhSID2Vx7xLc4ObZvIMnw,76
 ascend_deployer/playbooks/roles/mindx.dl/defaults/main.yml,sha256=LSbRMwZkChnKnzh7bxJ-E_eGRtHUU8XM3M2M99lC4No,1296
 ascend_deployer/playbooks/roles/mindx.dl/meta/main.yml,sha256=e4vPgX79HlfSjygJhGVEQT_g3qIMPWhV5P2j3D3t1rM,181
-ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml,sha256=CyzaKIZOFdU0ZHm1b9rSG87IJpJtRGi-bDLkSn3Ow_8,9771
+ascend_deployer/playbooks/roles/mindx.dl/tasks/ascend-operator.yaml,sha256=EmKoyIUAuO41UTUKV4i3g0WIVwZTMUfSmjxJHpMgPZI,3822
+ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml,sha256=axluEbbbA5q4GPAqivQiqNQht7q41KHNxiavjSZQV1I,10933
 ascend_deployer/playbooks/roles/mindx.dl/tasks/create_user.yaml,sha256=PfNpGclq1umyPnX0mc_nvi9tj6DZpVEEJBx6pbz-Nrk,675
 ascend_deployer/playbooks/roles/mindx.dl/tasks/deviceplugin.yaml,sha256=GS_E0y0KodLIOEI2KWwjL-Rvl-UUqJrnJnPmOfxFkWk,12772
-ascend_deployer/playbooks/roles/mindx.dl/tasks/distribute_soft_package.yaml,sha256=3f24D9cAFb5upAlEplCQOm2iD3aHPPSg4M8K2yJVBtU,7226
-ascend_deployer/playbooks/roles/mindx.dl/tasks/dl_common.yaml,sha256=TcT8JtY3MlTyrCAbQnUhghRdm-QShISHNGkQZtxvAZ8,726
+ascend_deployer/playbooks/roles/mindx.dl/tasks/distribute_soft_package.yaml,sha256=5qFYgDaEUk_BUDFofppiwKWZVRo3OTfmJK6vNIfQY64,7220
+ascend_deployer/playbooks/roles/mindx.dl/tasks/dl_common.yaml,sha256=YNsaD29A11oq7H1_61su_qg3HIfQD5QGc_cwKUPet8U,484
 ascend_deployer/playbooks/roles/mindx.dl/tasks/docker-runtime.yaml,sha256=yJe-9f0baw4tqCoGRrSsHS0Sa8ZgCR0XiAUQ1pd2OPI,1517
 ascend_deployer/playbooks/roles/mindx.dl/tasks/hccl.yaml,sha256=0vb8kxSHNHq_WyTV9KSQ1dXP0lhjprY7xFj9JJ2cTXA,5612
 ascend_deployer/playbooks/roles/mindx.dl/tasks/noded.yaml,sha256=pvOiiubZM-WML9I4D4tNpwoIAsc9jve0Mk3huMwXqlQ,5867
 ascend_deployer/playbooks/roles/mindx.dl/tasks/npu-exporter.yaml,sha256=zJNnlI_hrk8yhBwKaLBOdiA9dPUt27RjQ_aWFkMPeIY,5511
 ascend_deployer/playbooks/roles/mindx.dl/tasks/push_image.yaml,sha256=CM-AxhXAE4zIhk46IXMMED9dR1QSnSUw0k1Iw2lZpjY,4347
-ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml,sha256=W14-OeTw2FptQmwCX4Hz9las62wBWZaRZf6DwRZgpTU,7379
+ascend_deployer/playbooks/roles/mindx.dl/tasks/resilience-controller.yaml,sha256=P7mMJVVjDrlWww3jAHZEuYPjm1NcvXkqNUSl3MnHyww,4105
+ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml,sha256=YOgsaLzV5tlJHEzMnGzhRaVkBu41geTRmlsvwG7DY10,8879
 ascend_deployer/playbooks/roles/mindx.docker/README.md,sha256=_rk-uEyhUIyM1X9hFmBoR0cVNsCPjaFutgnLGY7Jnk8,67
 ascend_deployer/playbooks/roles/mindx.docker/meta/main.yml,sha256=HIK4udfQ5FIDSBZCHGmRI2fXksD_gpJZaYmTy6_s6ZQ,171
 ascend_deployer/playbooks/roles/mindx.docker/tasks/copy.yml,sha256=zhYaNVRkPWLkGUjlFAlOfuNVzp13LA5gKr3l08BaX14,500
 ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml,sha256=j8wMPI5_9498O-jVrvSbpONp96Jr-ODqYVdtF8Qya0A,418
-ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml,sha256=1S_zHployo8HJe7xz56YriqqBeT91kr_g97YW_znX7Y,892
+ascend_deployer/playbooks/roles/mindx.docker/tasks/install_containerd.yml,sha256=kXZqEDiVSOjljsHQTgVGlc358EBF-8Oel-NroOvnwt4,446
+ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml,sha256=Aoz2pzP4XWsVn_84DRxCPIwngwPOrpEzD5RJ7BxXZUE,1135
 ascend_deployer/playbooks/roles/mindx.docker/tasks/post_install.yml,sha256=bXsWWUxC9WmfBUZCmT6eMS8daSSVkjCEl-5lpUAuZ5w,1160
 ascend_deployer/playbooks/roles/mindx.docker/tests/ansible.cfg,sha256=o8K2az-hZ6dLhzVrfJdrpqKfXUpBBOAsHjneWGeuq4M,55
 ascend_deployer/playbooks/roles/mindx.docker/tests/inventory,sha256=yKsxPZwunWReo9UF4Yeuzhktj9QBBOmrryHZukdAyak,37
 ascend_deployer/playbooks/roles/mindx.docker/tests/test.yml,sha256=OfjTIOR1OLIp-jTG-H0JGrAgFfKgNFb9k40OwGZwwcI,116
 ascend_deployer/playbooks/roles/mindx.docker/vars/main.yml,sha256=1poZSfGzwYW8O_Lr-LRkYySUOPP4mr2zv_y3tnD7NDc,99
 ascend_deployer/playbooks/roles/mindx.harbor/tasks/check.yml,sha256=O-OHocr3VY8qFwybYKvzCrj5c5kRZyUujncLhBxllBg,1314
 ascend_deployer/playbooks/roles/mindx.harbor/tasks/http.yml,sha256=wDiwJIfN95dQ0PXvQv_UDxw6Kzr6bZghpxwZAhnUKqg,1158
@@ -275,17 +281,16 @@
 ascend_deployer/playbooks/roles/mindx.image/tasks/image_load.yaml,sha256=WNOEhlXVDW5t0KAdO392ljVs_ne93Q1Tm-YmMbzGHxY,660
 ascend_deployer/playbooks/roles/mindx.k8s/README.md,sha256=yEssYhqELC5UiHFN7ooAN3vB48OZIc4EHaMucUfvQSE,536
 ascend_deployer/playbooks/roles/mindx.k8s/defaults/main.yml,sha256=2JbJVXoWYha-hy0_w9eKfQpSkLgNp4Ua1yy2PgMogjI,234
 ascend_deployer/playbooks/roles/mindx.k8s/files/10-kubeadm.conf,sha256=ICh5R0gs5GbvEdItYXv4XzgVOOsPKjdNjqQmBxzYyTI,929
 ascend_deployer/playbooks/roles/mindx.k8s/files/kubelet.service,sha256=SMj1pqE9QXn-FW9IExZ6WQF3z92nPBuWgf7H49FZtwk,283
 ascend_deployer/playbooks/roles/mindx.k8s/meta/main.yml,sha256=BRFTshnlZZPPYEvfccG4xZD4bvRLfA5JoWfEl2UZcIE,179
 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/containerd.yml,sha256=1PCjhnosJZnTMAQwbRckw9pujMCWyNfGzgt4DXnDtRs,691
-ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml,sha256=15W8Lrl0JQQWRPyB40aoPToE500BuV-ge9fyv8-DcNU,1599
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml,sha256=RS9YQCpUgBC7ktEFq2NJ2Iio4bk2IRAlOqKgnutR11o,1321
 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml,sha256=vEN389NHfkegFNqf1621Dorujrf8-9SCJB_kmMmvaM8,774
-ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/get_k8s_version.yml,sha256=VGrqBEl-dsLfIRNwyoh5TgTXhEh4xSRL9LauE4FJ67s,693
 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml,sha256=rU7jbJ-ESswn9jI-MkM2PxgLlDQQjJvj6jDeEmnDEd4,869
 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml,sha256=2K3ePs0GGJf0pFz0EcSU89EAUZYeTVDMqLrC1icbH_8,1235
 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/os_setting.yml,sha256=NCw5rn4vEzk1fnbpsk_wrqLeb8fbxOcvtegD3pzgI_o,897
 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/push_image.yml,sha256=ZglMCqX7x5QlfKlNmdItMOAGDcaPYxQtxB8_xqmjxy4,4727
 ascend_deployer/playbooks/roles/mindx.k8s/tasks/kubevip/main.yml,sha256=M0cSfb4BJfDtI9WpxTgMxULuHr2u4LWriDF0rP7difw,1805
 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master/main.yml,sha256=sM7RArm6wVKNqbuCLQN_tKjqEBIgJwTMSfCim4Yy7eM,3557
 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master_backup/main.yml,sha256=bp02sszuA7KbwzaUgRq9flfWwC8_yaNYDapjTMXRkhs,1596
@@ -293,59 +298,59 @@
 ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.20.2.yaml,sha256=0IuV_4dsttpiTK0gmRZrINL22Gj6-pW1nW553aT1naw,202740
 ascend_deployer/playbooks/roles/mindx.k8s/tests/ansible.cfg,sha256=o8K2az-hZ6dLhzVrfJdrpqKfXUpBBOAsHjneWGeuq4M,55
 ascend_deployer/playbooks/roles/mindx.k8s/tests/inventory,sha256=yKsxPZwunWReo9UF4Yeuzhktj9QBBOmrryHZukdAyak,37
 ascend_deployer/playbooks/roles/mindx.k8s/tests/test.yml,sha256=OfjTIOR1OLIp-jTG-H0JGrAgFfKgNFb9k40OwGZwwcI,116
 ascend_deployer/playbooks/roles/mindx.k8s/vars/main.yml,sha256=Qz0ltVfvffbwEuSEBB5_EBXNoRqAbzrqUIfz52yfCTs,485
 ascend_deployer/playbooks/roles/mindx.kubeedge/README.md,sha256=GR4-d5SLMMehmWBbBNrzcN9GQ6fJa19VYPNOdbsu55I,78
 ascend_deployer/playbooks/roles/mindx.kubeedge/defaults/main.yml,sha256=oPyGFMkifGhQuic6xMeZcjq1stZwz5beoIwHghXxwZk,243
-ascend_deployer/playbooks/roles/mindx.kubeedge/files/certgen.sh,sha256=vGH1cb9rmzK2BcYQCsTeSugcOnejAowZotqcbmKi93E,3498
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cloudcore.service,sha256=xxxJLX5WTE0IJrige-s8s6jnmkq-pCm09VqDQrvYpkM,162
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cluster_objectsync_v1alpha1.yaml,sha256=vCVJRNNwuleGKWaoYz77DEYDst8Uv_Sw3lDfgV1EwAw,1896
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_device.yaml,sha256=ImwcEivucISHilWW2Qcf2YJcHF6O7XICmwzNq6MNcZw,8715
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_devicemodel.yaml,sha256=XXm1lB_aU1KOshj1Fi9if2jA98pMFdu1ISNbg-vvyy4,10576
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/objectsync_v1alpha1.yaml,sha256=h6btWq1S2NXWFLJUyIdaSSjpo699-ovF-nI_oWWqWxY,1877
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_rule.yaml,sha256=nry_fOwbj5epjvzi9ItjdwwCHudYz3NcGt84KHrlk5g,2443
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_ruleEndpoint.yaml,sha256=K2QGKpuGUgDuK5EbsWI5UTXaGwu_-TS8sOfcLslXvYo,1355
 ascend_deployer/playbooks/roles/mindx.kubeedge/meta/main.yml,sha256=EfM1TxOjLrD1JvVMnJI0hOrGGGXW8ukPeFU-i4CvVg4,176
-ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml,sha256=gNZJMTDj5FZbZzyArecuiiiR3SN5PQmXmkZjn2-rzzM,5153
+ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml,sha256=Asqvk7sLBFtRifuy8EjwsdELfNtk3XL4ix8MAj6zxac,4625
 ascend_deployer/playbooks/roles/mindx.rep/defaults/main.yml,sha256=a5xqx4dWRzMmrNs99mpt875vWZVqixR1y6wYz-0CE8E,144
 ascend_deployer/playbooks/roles/mindx.rep/tasks/get_npu_info.py,sha256=pKNZpC9IRYRstrQsp4kQVpg-duUF6AGABO3CL98mJn0,528
-ascend_deployer/playbooks/roles/mindx.rep/tasks/hccn_rep.yaml,sha256=SvAA_aKoU5EZ0oeERDC41l4XIdthgdJ5JZRv68jfjTw,2046
-ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py,sha256=AkkYNfy2u4nv_JhXkVvJ6FIVPA3mEYLjnjjRbgbT9eg,2268
-ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py,sha256=GzFoQG97RubW7sciJXRpc1lMY6y1BwsVxbuZrfWSJVE,6312
-ascend_deployer/playbooks/roles/mindx.rep/tasks/local_rep.yaml,sha256=7feyvSbmb9j4O3xB98m6k_endsDh3EOhK53lJM84_5s,1146
+ascend_deployer/playbooks/roles/mindx.rep/tasks/hccn_rep.yaml,sha256=1EqGjqf9yl1FC86DzXZHSlk8gvNa9oM9yZWzZyGyOFg,2089
+ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py,sha256=pQRge-mVSOf5NKw1qQ5suIM2JG9zzO8ebaxz7cop4HE,2856
+ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py,sha256=5UKMlePsKFZwNVb7XJH15nB5-_M3QDuT2JAyA6iw6pY,8254
+ascend_deployer/playbooks/roles/mindx.rep/tasks/local_rep.yaml,sha256=0jHxdbDyCrOpAoxxd-PbEqFMaA0AwyvOTIi7KTqDB4E,1218
 ascend_deployer/playbooks/roles/mindx.rep/tasks/ls_format.py,sha256=KjjDJDv1rzCM7kVkUBg7C0sdcdTZEP8BQ2YMGQ_aYjY,1011
 ascend_deployer/playbooks/roles/mindx.rep/tasks/output_json.py,sha256=W0gdfG9JksCkYJQIS-XZyBdvCTXQbqRNyXX0oV-UUSs,786
-ascend_deployer/playbooks/roles/mindx.rep/tasks/packages_rep.yaml,sha256=VZAhY5AVaphnzGccpTapN4Rcbgery0zTutYMUwvkiwU,1839
+ascend_deployer/playbooks/roles/mindx.rep/tasks/packages_rep.yaml,sha256=_Tg0tyNhSgTcz1oypJBg6xijg8qMSywMdu2ticbGSm4,1942
 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_k8s_docker.yaml,sha256=JDDiO0oedEzlSRz1uNeBPMrhWw86vhNtI2fN4PgKT7Q,389
 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_mef_kubeedge.yaml,sha256=z55v95_ueyFs3zQmUnkRt9ixoZcCZI0PsjD-w3ULxHM,390
 ascend_deployer/playbooks/scene/scene_auto.yml,sha256=tEPEu4K10RQZS3yw41r_Xjmt2vatlecQeIqPytSc6Bo,960
 ascend_deployer/playbooks/scene/scene_dl.yml,sha256=C5drgWAcympg1E478-1vde4HTZyCQFzhuCtpis89Q7w,613
 ascend_deployer/playbooks/scene/scene_edge.yml,sha256=w3idz1HuKo6qKcJr-m44iTDOP4wOiBYdQlXvCDSsUYw,259
 ascend_deployer/playbooks/scene/scene_mef.yml,sha256=bQaBhe6D-b75X-k0jXkfuiaPhnBq-XLLJzJTj8x1AyI,357
 ascend_deployer/playbooks/scene/scene_mindspore.yml,sha256=N8jl61OrdJ3Petl0irWUEXiDX4brIScPLa5il-UDNAw,514
 ascend_deployer/playbooks/scene/scene_offline_dev.yml,sha256=SEO7UmhRiBtoN_n9HJJyXaJs7bGe2BRR6pyYHI0OBkc,435
 ascend_deployer/playbooks/scene/scene_offline_run.yml,sha256=6aD5f1mua65hL8tB4osBmElFkW88PYosFsmR4OFYN1s,354
 ascend_deployer/playbooks/scene/scene_pytorch_dev.yml,sha256=jC69LyU98npgE1GIHMwaAvBKj5hnWQkeqNou5jdXr0I,510
 ascend_deployer/playbooks/scene/scene_pytorch_run.yml,sha256=em4k3qeeh_-qN8n-QJ2Oh1DQMUU9slsOTdg29eoUBkw,504
 ascend_deployer/playbooks/scene/scene_tensorflow_dev.yml,sha256=D4_mrI4NKLMD_4fsC7Njb2op103Ym9TzLVwaBlT65Xg,593
 ascend_deployer/playbooks/scene/scene_tensorflow_run.yml,sha256=usd-zORtPFqmsHEz3I1EMsCsvhm383eo2-EY2v8_BJg,587
 ascend_deployer/playbooks/scene/scene_vmhost.yml,sha256=g9ffCyxfOnsgTkUW3lwmYaps9ndwpTOqsy_MQtQA6Y4,273
-ascend_deployer/playbooks/test/case_driver.yml,sha256=9HlGjFD4sqpe-1OTObGUEO4ljKedTnsMwkis346CvMc,2180
-ascend_deployer/playbooks/test/case_firmware.yml,sha256=WEF3Lre7cxcCsPKLpgZFS5aCXAB6Yeyv-hIw2Ho-woA,567
-ascend_deployer/playbooks/test/case_mindspore.yml,sha256=NBPwPp1EI0yhepkjEiD5ThcSTfwcttpugnIPQ4pn_3M,2614
-ascend_deployer/playbooks/test/case_nnae.yml,sha256=Yl-8OpMOHDnYhfrZbrYu9jPQjmbnX39FQQbLegFs2zM,1466
-ascend_deployer/playbooks/test/case_nnrt.yml,sha256=BSc8ub1z3G6jfIl5pf61nQX1SZTeg6cXTz18ZtuJYV8,1466
-ascend_deployer/playbooks/test/case_pytorch.yml,sha256=BjrWe331g-WtyeAVl2rpYwK6OBu8U5_APzt22204Hi0,3095
-ascend_deployer/playbooks/test/case_tensorflow.yml,sha256=8Dol5heNZbkKxREft6PKaPBbQePUxZ6_Nqv1zITjiJg,6827
-ascend_deployer/playbooks/test/case_tfplugin.yml,sha256=IGcA-rEcDddrvq5e2Inc4xqM3nQunLwKtCnAAwRjLhA,1514
-ascend_deployer/playbooks/test/case_toolbox.yml,sha256=HEitC89js0ipsl0JqynfyU0YL16nn8og8uO2SN8GloE,1149
-ascend_deployer/playbooks/test/case_toolkit.yml,sha256=vQ-vWSYPeF9pRond8i3g61GVkCnd7DTPEvvw3jzeQXI,1509
+ascend_deployer/playbooks/test/case_driver.yml,sha256=Ta-ZhkDsvO103V689L4pWKHBbh0ax6YJUbmuylJ2Dn0,2642
+ascend_deployer/playbooks/test/case_firmware.yml,sha256=Pnjq7FArgiijtM9m5eH-19xNi7mZudjImhw-YB1jvOI,1127
+ascend_deployer/playbooks/test/case_mindspore.yml,sha256=0iIbZctMK3pyc8iN3EPUj5hIQ32BguP6rFtnRTsKO4M,3166
+ascend_deployer/playbooks/test/case_nnae.yml,sha256=Ms2ltzylGrcVr65Rkq7q9fWVOsxQa2G_7EyZDvsXH-o,753
+ascend_deployer/playbooks/test/case_nnrt.yml,sha256=rGTXww0qK2_DHTDgiHQLOEowaPHXYLC52QBci6IKs-w,751
+ascend_deployer/playbooks/test/case_pytorch.yml,sha256=V5DfpiUFDQs0xgJko3Zuq7MTsEyi_C3iddQ0vh01PGk,3619
+ascend_deployer/playbooks/test/case_tensorflow.yml,sha256=eYQvPOsxsHCkwUM9_xas_9KKW-Lpj9NY8AmZ6lpJFK4,7715
+ascend_deployer/playbooks/test/case_tfplugin.yml,sha256=FT6DGHNyw4NZIzsE3qtaW5ZVHf2A8YbqnsW307oyAZk,1766
+ascend_deployer/playbooks/test/case_toolbox.yml,sha256=wjoHGWj2I1MjXBC01m4sjVJ3C_XYw9RRTYghQPkyNCk,1473
+ascend_deployer/playbooks/test/case_toolkit.yml,sha256=JETTbrVs6RANDSLVs8uae4YkTrGy7prX6CSM0kvOTz0,788
 ascend_deployer/playbooks/test/test_all.yml,sha256=Iiuze5fGq9axRaPFv-fdRyFRLaCJHk4zH3FqiAyct5E,608
 ascend_deployer/playbooks/test/test_driver.yml,sha256=b5pGl8GVfIWtqKrHbXmmtcqr-mskZ0Hm5fy1_1YCHy8,284
+ascend_deployer/playbooks/test/test_exhibit.yml,sha256=W3XeZjzNcv5dRA_M6VZKYtMjkZunjWgLs0iu-YMReI0,114
 ascend_deployer/playbooks/test/test_firmware.yml,sha256=q3FlDhQiPi3VKIkQHjiPwy-bxfmAfL75hf9CzyxBL4M,284
 ascend_deployer/playbooks/test/test_mindspore.yml,sha256=mOTaFGiOm8pOmjGUwdZQl9kyU_MsdGhA_vIJyzM-vz0,99
 ascend_deployer/playbooks/test/test_nnae.yml,sha256=XoQXcfFppRtu29ntX96xbP_EmjwkplqUvGRB2HITM4A,90
 ascend_deployer/playbooks/test/test_nnrt.yml,sha256=K1VWj2uRXfKqcjuMyU2PuOqLbzstgm-S5hwz5P8t2Rc,89
 ascend_deployer/playbooks/test/test_pytorch.yml,sha256=2hZXx8jklP6bmApcRNYelFwx7i9oGEak5-_Ag0pmH0c,96
 ascend_deployer/playbooks/test/test_tensorflow.yml,sha256=xVVNWd_c0DByGfi_jnwpe6vJgDrnBdYUDwGtcPkK6Wg,101
 ascend_deployer/playbooks/test/test_tfplugin.yml,sha256=fm-IvOolhycuY45svRn-cXt3cYcnwLKYzxtObWNR7Gg,97
@@ -353,28 +358,29 @@
 ascend_deployer/playbooks/test/test_toolkit.yml,sha256=YfwXJlVmRewWXuSzeUK5Mi28LfXU9ytNvWbWbXEErBo,95
 ascend_deployer/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ascend_deployer/scripts/check_pkgs.sh,sha256=_CF5zylsdYKY1EsCKO51B6Z6vCk5mD_Qy6uMSlU_Whw,20831
 ascend_deployer/scripts/hccn_set.sh,sha256=j8oTcJmKe9fa6_Gm4lsIMBFQIeSUCXJJFNoTFOdOo-0,1116
 ascend_deployer/scripts/image_load.sh,sha256=qWdGBVy0_c60yDYmPAtnRPFwiCD_X-eOK7bROL-yyP8,1142
 ascend_deployer/scripts/install.sh,sha256=u-mtTLGfx_0FOuqrF0qV2QZD_oFwDeDf6_XMlNFiZ4g,969
 ascend_deployer/scripts/install_ansible.sh,sha256=DEXh1Acvs3gheDoVN8tuIKV8h_Tg9oHJpppnvxQ1Dhs,3587
-ascend_deployer/scripts/nexus.py,sha256=WOnuggqktKAqmz5nlbJN0fD18kXoNjyErDO5fhHEIvs,14207
-ascend_deployer/scripts/nexus_config.json,sha256=yZ4oy6BkuBdVmoheGBw7yTs7FLnnE66o-ut34lcyT0Q,1257
-ascend_deployer/scripts/prepare.sh,sha256=Dhksr4z-yb-JwlGcQ4DPCN9OBEw-nC6FdU9htsjIMI8,15393
+ascend_deployer/scripts/nexus.py,sha256=HlnwcqNndrZe8OLenNaMYaweEV_H2tirSjf_XMv5bfg,14663
+ascend_deployer/scripts/nexus_config.json,sha256=7s7HeSrwgKzAqaDtsS98XWLGHwZcBz8EphqYSfrPRhc,1219
+ascend_deployer/scripts/prepare.sh,sha256=LQba5DpLPUMMrtYwlUmT0dlSBkPzGOeWz23dnwbYECA,15176
 ascend_deployer/scripts/uninstall_k8s_docker.sh,sha256=nSY6GniAuiaDI3Emj-BCRY38IRPHklYZ2OIMDgDVf90,535
 ascend_deployer/scripts/uninstall_mef_kubeedge.sh,sha256=8g3Yni8tl1Rgy5slpNIqdJozZcmp5O9x0b7TBAjX2j4,643
 ascend_deployer/scripts/uninstall_mef_related.sh,sha256=7tu9AcnPMxpbsjBMicW3udsKn8_aIcA9Za9h75xp11c,679
 ascend_deployer/scripts/utils.sh,sha256=sHVwhZydgv2vF1GQ9QBPjWwCtWccb_Q5IGSeIbjWaOA,5723
 ascend_deployer/tools/DeviceIP-conf.sh,sha256=R74aTgi2D2TqggSvXLj6tViTC7FwTODvA5rSx26eCW8,10900
 ascend_deployer/tools/ascend-deployer,sha256=7KBABYrGdNiIJFzRpA90YMi7v9BDchcsDAji3JoCTOE,1409
 ascend_deployer/tools/check.py,sha256=cu3uzA14apAt1DqK273XWkfABwxTUafDmRLN35tiI14,4049
-ascend_deployer/tools/hccn.py,sha256=dY0TejYI-8jJO4LUETpvL3Jdd9gEqKSh05kR0a4LY1E,7740
+ascend_deployer/tools/hccn.py,sha256=o5dTZucvFX5SuNt8PCJFeKhC0SBO9mdHMNAuy7gaYNU,7684
 ascend_deployer/tools/update_crl.sh,sha256=VwBHBTughh1qOxqqurddYS37blB96iH2eTkBSHpcgaE,9930
 ascend_deployer/tools/hccn/main/go.mod,sha256=YgIwnIERMSUYwOhf99p-SJRh8X__2XsNQVJOHMMx0eA,21
 ascend_deployer/tools/hccn/main/hccn.go,sha256=robmOcfv1cHeM__UTnU2-sP6wDRBcId4UwSP8hkbGVc,6863
+ascend_deployer/tools/nexus/Dockerfile,sha256=r9sloQ5C5HMVo7TWnuttIcTEssUKGuG51m1BNc3hSKU,4260
 ascend_deployer/tools/report/main/go.mod,sha256=T_4E5SwIfDiUuU3LukbU4QKLaPEFaZ1lgb-GQcsNRuA,142
 ascend_deployer/tools/report/main/main.go,sha256=MnVc5U17AAEu150DdFrziPgRtfgqxLsav2PbOiagr80,18729
 ascend_deployer/tools/unzip/main/go.mod,sha256=YgIwnIERMSUYwOhf99p-SJRh8X__2XsNQVJOHMMx0eA,21
 ascend_deployer/tools/unzip/main/unzip.go,sha256=-Z0ihIicC_3GihItvhc1it3PQoyFLSz0ycGuKj82wlk,1587
 ascend_deployer/yamls/basic.yaml,sha256=LMbvOfJ78T5dXk0YEhATGNGiMe4_sSnzt6MoT_bu4I0,46
 ascend_deployer/yamls/check.yaml,sha256=74W_bQT1to6tJGK2FPrggJuFbogaAzXK7oDDLaR3xrk,46
 ascend_deployer/yamls/docker.yaml,sha256=4OEYn9_0xxyMCpl1qdJhiTZ3MctxhUdz3uXYRxzYwwY,132
@@ -382,15 +388,15 @@
 ascend_deployer/yamls/harbor.yaml,sha256=4YmjA4UTdAhNLB4pH2d8G2jTnIiNELbMYY-VCqxO2y0,72
 ascend_deployer/yamls/hccn.yaml,sha256=5VuwXcGseHty7iA7s4z8YKlupyu0HRe9j_WvjLTCRKk,45
 ascend_deployer/yamls/image_load.yaml,sha256=8P1n5bl4dZo-F5Q_7-F2JIMngGnWESzEr3qzIC4JaPw,51
 ascend_deployer/yamls/k8s.yaml,sha256=OwWlFC9IPOYT-2GT4LJUYMZCC2qKSI1o9X1dw8vvEpo,126
 ascend_deployer/yamls/k8s_reset.yaml,sha256=BUkmH2NmaIPzevXbf6c_S8jT7kL7sHfVq9YILxqswVk,234
 ascend_deployer/yamls/mindxdl.yaml,sha256=xvHRj2q-tMw8G0x6CcXZ8gbdKuyEvsxEDj02u_1es4A,74
 ascend_deployer/yamls/report.yaml,sha256=OABhE8u336Y0ILTBln4mSw3s8llyDRnA1B5ZdVzmExY,47
-ascend_deployer-5.0.0b8.data/scripts/ascend-deployer,sha256=7KBABYrGdNiIJFzRpA90YMi7v9BDchcsDAji3JoCTOE,1409
-ascend_deployer-5.0.0b8.dist-info/DESCRIPTION.rst,sha256=PDOp6VeO5ALmb1fAHownSdYsCQmeh1EDRj7k8r1LZDU,2739
-ascend_deployer-5.0.0b8.dist-info/METADATA,sha256=3yNmmWlybMndb8dZZTthU7taaTAzErUFoUYQRWjm6GQ,3183
-ascend_deployer-5.0.0b8.dist-info/RECORD,,
-ascend_deployer-5.0.0b8.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-ascend_deployer-5.0.0b8.dist-info/entry_points.txt,sha256=HjyLLr0zJ_k7sWdPoQgJB-Tc2jKReTuJDbM-6LqbKbc,74
-ascend_deployer-5.0.0b8.dist-info/metadata.json,sha256=Xqfs_jvSyCP2Jx5ZWeuSKLnRd4A9OfXz-_OuOf32fMQ,777
-ascend_deployer-5.0.0b8.dist-info/top_level.txt,sha256=T3GbQwFRI8Cl3QuJELdNLLkq3kGZrvYBykFox-L0XCw,16
+ascend_deployer-5.0.0b9.data/scripts/ascend-deployer,sha256=7KBABYrGdNiIJFzRpA90YMi7v9BDchcsDAji3JoCTOE,1409
+ascend_deployer-5.0.0b9.dist-info/DESCRIPTION.rst,sha256=PDOp6VeO5ALmb1fAHownSdYsCQmeh1EDRj7k8r1LZDU,2739
+ascend_deployer-5.0.0b9.dist-info/METADATA,sha256=FWeVA99XwBwZYICHZCdCXhJchJvxnl50A3GJfIm3Lzs,3183
+ascend_deployer-5.0.0b9.dist-info/RECORD,,
+ascend_deployer-5.0.0b9.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+ascend_deployer-5.0.0b9.dist-info/entry_points.txt,sha256=HjyLLr0zJ_k7sWdPoQgJB-Tc2jKReTuJDbM-6LqbKbc,74
+ascend_deployer-5.0.0b9.dist-info/metadata.json,sha256=QMr_jIzvwUSK_ivpPcuycBejq3Ny3pK3aY0HfiT0a3s,777
+ascend_deployer-5.0.0b9.dist-info/top_level.txt,sha256=T3GbQwFRI8Cl3QuJELdNLLkq3kGZrvYBykFox-L0XCw,16
```


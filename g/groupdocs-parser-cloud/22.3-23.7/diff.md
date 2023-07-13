# Comparing `tmp/groupdocs-parser-cloud-22.3.tar.gz` & `tmp/groupdocs-parser-cloud-23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\groupdocs-parser-cloud-22.3.tar", last modified: Mon Mar 14 13:52:58 2022, max compression
+gzip compressed data, was "dist\groupdocs-parser-cloud-23.7.tar", last modified: Thu Jul 13 12:06:28 2023, max compression
```

## Comparing `groupdocs-parser-cloud-22.3.tar` & `groupdocs-parser-cloud-23.7.tar`

### file list

```diff
@@ -1,99 +1,104 @@
-drwxrwxrwx   0        0        0        0 2022-03-14 13:52:58.000000 groupdocs-parser-cloud-22.3/
--rw-rw-rw-   0        0        0     1105 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/LICENSE
--rw-rw-rw-   0        0        0     2875 2022-03-14 13:52:58.000000 groupdocs-parser-cloud-22.3/PKG-INFO
--rw-rw-rw-   0        0        0     2005 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/README.md
-drwxrwxrwx   0        0        0        0 2022-03-14 13:52:56.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/
--rw-rw-rw-   0        0        0     4953 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/__init__.py
--rw-rw-rw-   0        0        0    26222 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/api_client.py
--rw-rw-rw-   0        0        0     2870 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/api_exception.py
-drwxrwxrwx   0        0        0        0 2022-03-14 13:52:56.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/
--rw-rw-rw-   0        0        0      443 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/__init__.py
--rw-rw-rw-   0        0        0    38644 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/file_api.py
--rw-rw-rw-   0        0        0    36254 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/folder_api.py
--rw-rw-rw-   0        0        0    17273 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/info_api.py
--rw-rw-rw-   0        0        0    19064 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/parse_api.py
--rw-rw-rw-   0        0        0    26570 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/storage_api.py
--rw-rw-rw-   0        0        0    19354 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/template_api.py
--rw-rw-rw-   0        0        0     3303 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/auth.py
--rw-rw-rw-   0        0        0     7677 2022-03-14 13:50:10.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/configuration.py
-drwxrwxrwx   0        0        0        0 2022-03-14 13:52:58.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/
--rw-rw-rw-   0        0        0     3559 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/__init__.py
--rw-rw-rw-   0        0        0     6510 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/container_item.py
--rw-rw-rw-   0        0        0     5085 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/container_item_info.py
--rw-rw-rw-   0        0        0     3713 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/container_options.py
--rw-rw-rw-   0        0        0     4549 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/container_result.py
--rw-rw-rw-   0        0        0     6918 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/coordinates.py
--rw-rw-rw-   0        0        0     5871 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/create_template_options.py
--rw-rw-rw-   0        0        0     9078 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/detector_parameters.py
--rw-rw-rw-   0        0        0     5187 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     6291 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/error.py
--rw-rw-rw-   0        0        0     4905 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/error_details.py
--rw-rw-rw-   0        0        0     6120 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/field.py
--rw-rw-rw-   0        0        0     6604 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/field_data.py
--rw-rw-rw-   0        0        0    14082 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/field_position.py
--rw-rw-rw-   0        0        0     5626 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/file_info.py
--rw-rw-rw-   0        0        0     5131 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/file_type.py
--rw-rw-rw-   0        0        0     5409 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/file_version.py
--rw-rw-rw-   0        0        0     4151 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4171 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/files_list.py
--rw-rw-rw-   0        0        0     4884 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     4876 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/format.py
--rw-rw-rw-   0        0        0     4211 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/formats_result.py
--rw-rw-rw-   0        0        0     4205 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/formatted_text_options.py
--rw-rw-rw-   0        0        0     8089 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/image.py
--rw-rw-rw-   0        0        0     5050 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/image_page.py
--rw-rw-rw-   0        0        0     6495 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/images_options.py
--rw-rw-rw-   0        0        0     4898 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/images_result.py
--rw-rw-rw-   0        0        0     3682 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/info_options.py
--rw-rw-rw-   0        0        0     6653 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/info_result.py
--rw-rw-rw-   0        0        0     5178 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/object_exist.py
--rw-rw-rw-   0        0        0     4912 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/page.py
--rw-rw-rw-   0        0        0     7147 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/page_area.py
--rw-rw-rw-   0        0        0     6507 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/page_table_area.py
--rw-rw-rw-   0        0        0     8001 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/page_table_area_cell.py
--rw-rw-rw-   0        0        0     6658 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/page_text_area.py
--rw-rw-rw-   0        0        0     5575 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/parse_options.py
--rw-rw-rw-   0        0        0     5082 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/parse_result.py
--rw-rw-rw-   0        0        0     5233 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/parser_options.py
--rw-rw-rw-   0        0        0     4843 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/point.py
--rw-rw-rw-   0        0        0     5735 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/rectangle.py
--rw-rw-rw-   0        0        0     5014 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/size.py
--rw-rw-rw-   0        0        0     4276 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7173 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/storage_file.py
--rw-rw-rw-   0        0        0     7350 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/table.py
--rw-rw-rw-   0        0        0     5527 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/table_layout.py
--rw-rw-rw-   0        0        0     4838 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/template.py
--rw-rw-rw-   0        0        0     5111 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/template_options.py
--rw-rw-rw-   0        0        0     4994 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/template_result.py
--rw-rw-rw-   0        0        0     6797 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/text_options.py
--rw-rw-rw-   0        0        0     4957 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/text_page.py
--rw-rw-rw-   0        0        0     4765 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/text_result.py
--rw-rw-rw-   0        0        0     7617 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/text_style.py
--rw-rw-rw-   0        0        0    13735 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/rest.py
-drwxrwxrwx   0        0        0        0 2022-03-14 13:52:56.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud.egg-info/
--rw-rw-rw-   0        0        0     2875 2022-03-14 13:52:49.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3627 2022-03-14 13:52:51.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-14 13:52:49.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2022-03-14 13:52:50.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2022-03-14 13:52:50.000000 groupdocs-parser-cloud-22.3/groupdocs_parser_cloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-14 13:52:58.000000 groupdocs-parser-cloud-22.3/setup.cfg
--rw-rw-rw-   0        0        0     1699 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-14 13:52:58.000000 groupdocs-parser-cloud-22.3/test/
--rw-rw-rw-   0        0        0      118 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/JsonUtils.py
--rw-rw-rw-   0        0        0        0 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-14 13:52:58.000000 groupdocs-parser-cloud-22.3/test/apis/
--rw-rw-rw-   0        0        0        0 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/__init__.py
--rw-rw-rw-   0        0        0     3001 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/test_auth_api.py
--rw-rw-rw-   0        0        0     3783 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/test_file_api.py
--rw-rw-rw-   0        0        0     3137 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/test_folder_api.py
--rw-rw-rw-   0        0        0     4532 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/test_parser_container_api.py
--rw-rw-rw-   0        0        0     2026 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/test_parser_formats_api.py
--rw-rw-rw-   0        0        0     6295 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/test_parser_image_api.py
--rw-rw-rw-   0        0        0     3890 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/test_parser_info_api.py
--rw-rw-rw-   0        0        0     5904 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/test_parser_parse_api.py
--rw-rw-rw-   0        0        0     5873 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/test_parser_template_api.py
--rw-rw-rw-   0        0        0     5493 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/test_parser_text_api.py
--rw-rw-rw-   0        0        0     2721 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/apis/test_storage_api.py
--rw-rw-rw-   0        0        0     5026 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/test_context.py
--rw-rw-rw-   0        0        0     5110 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/test_file.py
--rw-rw-rw-   0        0        0     1702 2022-03-11 08:22:11.000000 groupdocs-parser-cloud-22.3/test/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/
+-rw-rw-rw-   0        0        0     1105 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/LICENSE
+-rw-rw-rw-   0        0        0     2836 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2005 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/
+-rw-rw-rw-   0        0        0     4953 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/__init__.py
+-rw-rw-rw-   0        0        0    26221 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/api_client.py
+-rw-rw-rw-   0        0        0     2870 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/api_exception.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/
+-rw-rw-rw-   0        0        0      443 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/__init__.py
+-rw-rw-rw-   0        0        0    38644 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/file_api.py
+-rw-rw-rw-   0        0        0    36254 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/folder_api.py
+-rw-rw-rw-   0        0        0    17273 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/info_api.py
+-rw-rw-rw-   0        0        0    24330 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/parse_api.py
+-rw-rw-rw-   0        0        0    26570 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/storage_api.py
+-rw-rw-rw-   0        0        0    19354 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/template_api.py
+-rw-rw-rw-   0        0        0     3303 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/auth.py
+-rw-rw-rw-   0        0        0     7677 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/
+-rw-rw-rw-   0        0        0     3836 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/__init__.py
+-rw-rw-rw-   0        0        0     5758 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/barcode.py
+-rw-rw-rw-   0        0        0     4107 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/barcode_page.py
+-rw-rw-rw-   0        0        0     6511 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/barcodes_options.py
+-rw-rw-rw-   0        0        0     4221 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/barcodes_result.py
+-rw-rw-rw-   0        0        0     6510 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/container_item.py
+-rw-rw-rw-   0        0        0     5085 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/container_item_info.py
+-rw-rw-rw-   0        0        0     3713 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/container_options.py
+-rw-rw-rw-   0        0        0     4549 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/container_result.py
+-rw-rw-rw-   0        0        0     6918 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/coordinates.py
+-rw-rw-rw-   0        0        0     5871 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/create_template_options.py
+-rw-rw-rw-   0        0        0     9078 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/detector_parameters.py
+-rw-rw-rw-   0        0        0     5187 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     6291 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/error.py
+-rw-rw-rw-   0        0        0     4905 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/error_details.py
+-rw-rw-rw-   0        0        0     6120 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/field.py
+-rw-rw-rw-   0        0        0     6604 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/field_data.py
+-rw-rw-rw-   0        0        0    14082 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/field_position.py
+-rw-rw-rw-   0        0        0     5626 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/file_info.py
+-rw-rw-rw-   0        0        0     5131 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/file_type.py
+-rw-rw-rw-   0        0        0     5409 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4151 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4171 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4884 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     4876 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/format.py
+-rw-rw-rw-   0        0        0     4211 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/formats_result.py
+-rw-rw-rw-   0        0        0     4205 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/formatted_text_options.py
+-rw-rw-rw-   0        0        0     8089 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/image.py
+-rw-rw-rw-   0        0        0     5050 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/image_page.py
+-rw-rw-rw-   0        0        0     6495 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/images_options.py
+-rw-rw-rw-   0        0        0     4898 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/images_result.py
+-rw-rw-rw-   0        0        0     3682 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/info_options.py
+-rw-rw-rw-   0        0        0     6653 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/info_result.py
+-rw-rw-rw-   0        0        0     5178 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     4912 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/page.py
+-rw-rw-rw-   0        0        0     7147 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/page_area.py
+-rw-rw-rw-   0        0        0     6507 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/page_table_area.py
+-rw-rw-rw-   0        0        0     8001 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/page_table_area_cell.py
+-rw-rw-rw-   0        0        0     6658 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/page_text_area.py
+-rw-rw-rw-   0        0        0     5575 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/parse_options.py
+-rw-rw-rw-   0        0        0     5082 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/parse_result.py
+-rw-rw-rw-   0        0        0     5233 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/parser_options.py
+-rw-rw-rw-   0        0        0     4843 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/point.py
+-rw-rw-rw-   0        0        0     5735 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/rectangle.py
+-rw-rw-rw-   0        0        0     5014 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/size.py
+-rw-rw-rw-   0        0        0     4276 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7173 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/storage_file.py
+-rw-rw-rw-   0        0        0     7350 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/table.py
+-rw-rw-rw-   0        0        0     5527 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/table_layout.py
+-rw-rw-rw-   0        0        0     4838 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/template.py
+-rw-rw-rw-   0        0        0     5111 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/template_options.py
+-rw-rw-rw-   0        0        0     4994 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/template_result.py
+-rw-rw-rw-   0        0        0     6797 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/text_options.py
+-rw-rw-rw-   0        0        0     4957 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/text_page.py
+-rw-rw-rw-   0        0        0     4765 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/text_result.py
+-rw-rw-rw-   0        0        0     7617 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/text_style.py
+-rw-rw-rw-   0        0        0    13735 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/rest.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud.egg-info/
+-rw-rw-rw-   0        0        0     2836 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3850 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/groupdocs_parser_cloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/setup.cfg
+-rw-rw-rw-   0        0        0     1699 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/test/
+-rw-rw-rw-   0        0        0      118 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/JsonUtils.py
+-rw-rw-rw-   0        0        0        0 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:06:28.000000 groupdocs-parser-cloud-23.7/test/apis/
+-rw-rw-rw-   0        0        0        0 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/__init__.py
+-rw-rw-rw-   0        0        0     3001 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_auth_api.py
+-rw-rw-rw-   0        0        0     3783 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_file_api.py
+-rw-rw-rw-   0        0        0     3137 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_folder_api.py
+-rw-rw-rw-   0        0        0     2401 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_parser_barcode_api.py
+-rw-rw-rw-   0        0        0     4521 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_parser_container_api.py
+-rw-rw-rw-   0        0        0     2026 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_parser_formats_api.py
+-rw-rw-rw-   0        0        0     6295 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_parser_image_api.py
+-rw-rw-rw-   0        0        0     3890 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_parser_info_api.py
+-rw-rw-rw-   0        0        0     5904 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_parser_parse_api.py
+-rw-rw-rw-   0        0        0     5873 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_parser_template_api.py
+-rw-rw-rw-   0        0        0     5493 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_parser_text_api.py
+-rw-rw-rw-   0        0        0     2721 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/apis/test_storage_api.py
+-rw-rw-rw-   0        0        0     5026 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/test_context.py
+-rw-rw-rw-   0        0        0     5428 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/test_file.py
+-rw-rw-rw-   0        0        0     1588 2023-07-13 12:04:07.000000 groupdocs-parser-cloud-23.7/test/test_settings.py
```

### Comparing `groupdocs-parser-cloud-22.3/LICENSE` & `groupdocs-parser-cloud-23.7/LICENSE`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/PKG-INFO` & `groupdocs-parser-cloud-23.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: groupdocs-parser-cloud
-Version: 22.3
+Version: 23.7
 Summary: GroupDocs.Parser Cloud Python SDK
 Home-page: http://github.com/groupdocs-parser-cloud/groupdocs-parser-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
-License: UNKNOWN
 Keywords: groupdocs,parser,cloud,python,sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -75,8 +73,7 @@
 + [**Product Home**](https://products.groupdocs.cloud/parser)
 + [**Documentation**](https://docs.groupdocs.cloud/display/parsercloud/Home)
 + [**Free Support Forum**](https://forum.groupdocs.cloud/c/parser)
 + [**Blog**](https://blog.groupdocs.cloud/category/parser)
 
 ## Contact Us
 Your feedback is very important to us. Please feel free to contact us using our [Support Forums](https://forum.groupdocs.cloud/c/parser).
-
```

### Comparing `groupdocs-parser-cloud-22.3/README.md` & `groupdocs-parser-cloud-23.7/README.md`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/__init__.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/api_client.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="api_client.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -70,20 +70,20 @@
     }
 
     def __init__(self, configuration, header_name=None, header_value=None,
                  cookie=None):
         self.configuration = configuration
         self.pool = None
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '22.3'}
+        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '23.7'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 22.3'
+        self.user_agent = 'python sdk 23.7'
 
     def __del__(self):
         if self.pool is not None:
             self.pool.close()
             self.pool.join()
 
     @property
@@ -451,15 +451,15 @@
 
         if files:
             for k, v in files:
                 if not v:
                     continue
                 file_names = v if type(v) is list else [v]
                 for n in file_names:
-                    with open(n, 'r+b') as f:
+                    with open(n, 'rb') as f:
                         filename = os.path.basename(f.name)
                         filedata = f.read()
                         mimetype = (mimetypes.guess_type(filename)[0] or
                                     'application/octet-stream')
                         params.append(
                             tuple([k, tuple([filename, filedata, mimetype])]))
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/api_exception.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/api_exception.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/file_api.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/file_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="parser_api.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -634,15 +634,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="copy_file_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -678,15 +678,15 @@
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_file_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -718,15 +718,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="download_file_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -758,15 +758,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="move_file_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -802,15 +802,15 @@
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="upload_file_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/folder_api.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/folder_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="parser_api.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -610,15 +610,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="copy_folder_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -652,15 +652,15 @@
         self.dest_path = dest_path
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="create_folder_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -690,15 +690,15 @@
         """Initializes new instance of CreateFolderRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_folder_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -730,15 +730,15 @@
         self.path = path
         self.storage_name = storage_name
         self.recursive = recursive
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_files_list_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -768,15 +768,15 @@
         """Initializes new instance of GetFilesListRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="move_folder_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/info_api.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/info_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="parser_api.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -356,15 +356,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="container_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -392,15 +392,15 @@
     def __init__(self, options):
         """Initializes new instance of ContainerRequest."""  # noqa: E501
         self.options = options
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_info_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/parse_api.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/parse_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="parser_api.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -79,14 +79,105 @@
         """
         Initializes new instance of ParseApi with configuration options
 
         :param configuration API configuration
         """
         return ParseApi(configuration)
 
+    def barcodes(self, request,**kwargs):  # noqa: E501
+        """Extract barcodes from document.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param BarcodesOptions options: Extract barcode options. (required)
+        :return: BarcodesResult
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+
+        if kwargs.get('is_async'):
+            return self._barcodes_with_http_info(request, **kwargs)  # noqa: E501
+        
+        (data) = self._barcodes_with_http_info(request, **kwargs)  # noqa: E501
+        return data
+
+    def _barcodes_with_http_info(self, request, **kwargs):  # noqa: E501
+        """Extract barcodes from document.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param BarcodesRequest request object with parameters
+        :return: BarcodesResult
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        params = locals()
+        params['is_async'] = ''
+        params['_return_http_data_only'] = False
+        params['_preload_content'] = True
+        params['_request_timeout'] = ''
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method barcodes" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'options' is set
+        if request.options is None:
+            raise ValueError("Missing the required parameter `options` when calling `barcodes`")  # noqa: E501
+
+        collection_formats = {}
+        path = '/parser/barcodes'
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = []
+
+        body_params = None
+        if request.options is not None:
+            body_params = request.options
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        call_kwargs = {
+            'resource_path':path, 
+            'method':'POST',
+            'path_params':path_params,
+            'query_params':query_params,
+            'header_params':header_params,
+            'body':body_params,
+            'post_params':form_params,
+            'files':local_var_files,
+            'response_type':'BarcodesResult',  # noqa: E501
+            'auth_settings':self.auth.get_auth_settings(),
+            'is_async':params.get('is_async'),
+            '_return_http_data_only':params.get('_return_http_data_only'),
+            '_preload_content':params.get('_preload_content', True),
+            '_request_timeout':params.get('_request_timeout'),
+            'collection_formats':collection_formats
+        }
+
+        return self.api_client.call_api(**call_kwargs)  # noqa: E501
+
     def images(self, request,**kwargs):  # noqa: E501
         """Extract images from document.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
 
         :param is_async bool
@@ -361,16 +452,52 @@
             return str
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
+# <copyright company="Aspose Pty Ltd" file="barcodes_request.py">
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
+# </copyright>
+# <summary>
+#   Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
+# 
+#  The above copyright notice and this permission notice shall be included in all
+#  copies or substantial portions of the Software.
+# 
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+#  SOFTWARE.
+# </summary>
+# --------------------------------------------------------------------------------
+
+class BarcodesRequest(object):
+    """
+    Request model for barcodes operation.
+    :param options Extract barcode options.
+    """
+
+    def __init__(self, options):
+        """Initializes new instance of BarcodesRequest."""  # noqa: E501
+        self.options = options
+# coding: utf-8
+
+# --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="images_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -398,15 +525,15 @@
     def __init__(self, options):
         """Initializes new instance of ImagesRequest."""  # noqa: E501
         self.options = options
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="parse_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -434,15 +561,15 @@
     def __init__(self, options):
         """Initializes new instance of ParseRequest."""  # noqa: E501
         self.options = options
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="text_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/storage_api.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/storage_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="parser_api.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -471,15 +471,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_disc_usage_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -507,15 +507,15 @@
     def __init__(self, storage_name=None):
         """Initializes new instance of GetDiscUsageRequest."""  # noqa: E501
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_file_versions_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -545,15 +545,15 @@
         """Initializes new instance of GetFileVersionsRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="object_exists_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -585,15 +585,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="storage_exists_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/apis/template_api.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/apis/template_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="parser_api.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -362,15 +362,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="create_template_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -398,15 +398,15 @@
     def __init__(self, options):
         """Initializes new instance of CreateTemplateRequest."""  # noqa: E501
         self.options = options
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_template_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -434,15 +434,15 @@
     def __init__(self, options):
         """Initializes new instance of DeleteTemplateRequest."""  # noqa: E501
         self.options = options
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_template_request.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/auth.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/auth.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/configuration.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="configuration.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -198,10 +198,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 22.3\n"\
-               "SDK Package Version: 22.3".\
+               "Version of the API: 23.7\n"\
+               "SDK Package Version: 23.7".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/__init__.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # coding: utf-8
 
 # flake8: noqa
 from __future__ import absolute_import
 
 # import models
+from groupdocs_parser_cloud.models.barcode import Barcode
+from groupdocs_parser_cloud.models.barcode_page import BarcodePage
+from groupdocs_parser_cloud.models.barcodes_result import BarcodesResult
 from groupdocs_parser_cloud.models.container_item import ContainerItem
 from groupdocs_parser_cloud.models.container_item_info import ContainerItemInfo
 from groupdocs_parser_cloud.models.container_result import ContainerResult
 from groupdocs_parser_cloud.models.coordinates import Coordinates
 from groupdocs_parser_cloud.models.create_template_options import CreateTemplateOptions
 from groupdocs_parser_cloud.models.detector_parameters import DetectorParameters
 from groupdocs_parser_cloud.models.disc_usage import DiscUsage
@@ -45,13 +48,14 @@
 from groupdocs_parser_cloud.models.table_layout import TableLayout
 from groupdocs_parser_cloud.models.template import Template
 from groupdocs_parser_cloud.models.template_options import TemplateOptions
 from groupdocs_parser_cloud.models.template_result import TemplateResult
 from groupdocs_parser_cloud.models.text_page import TextPage
 from groupdocs_parser_cloud.models.text_result import TextResult
 from groupdocs_parser_cloud.models.text_style import TextStyle
+from groupdocs_parser_cloud.models.barcodes_options import BarcodesOptions
 from groupdocs_parser_cloud.models.container_options import ContainerOptions
 from groupdocs_parser_cloud.models.file_version import FileVersion
 from groupdocs_parser_cloud.models.images_options import ImagesOptions
 from groupdocs_parser_cloud.models.info_options import InfoOptions
 from groupdocs_parser_cloud.models.parse_options import ParseOptions
 from groupdocs_parser_cloud.models.text_options import TextOptions
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/container_item.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/container_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ContainerItem.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/container_item_info.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/container_item_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ContainerItemInfo.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/container_options.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/container_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ContainerOptions.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/container_result.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/container_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ContainerResult.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/coordinates.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/coordinates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Coordinates.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/create_template_options.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/create_template_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="CreateTemplateOptions.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/detector_parameters.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/detector_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DetectorParameters.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/disc_usage.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/disc_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DiscUsage.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/error.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Error.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/error_details.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/error_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ErrorDetails.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/field.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Field.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/field_data.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/field_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FieldData.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/field_position.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/field_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FieldPosition.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/file_info.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileInfo.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/file_type.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/file_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileType.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/file_version.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/file_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileVersion.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/file_versions.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/file_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileVersions.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/files_list.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/files_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FilesList.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/files_upload_result.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/files_upload_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FilesUploadResult.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/format.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Format.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/formats_result.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/formats_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FormatsResult.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/formatted_text_options.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/formatted_text_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FormattedTextOptions.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/image.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Image.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/image_page.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/image_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ImagePage.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/images_options.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/images_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ImagesOptions.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/images_result.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/images_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ImagesResult.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/info_options.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/info_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="InfoOptions.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/info_result.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/info_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="InfoResult.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/object_exist.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/object_exist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ObjectExist.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/page.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Page.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/page_area.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/page_area.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PageArea.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/page_table_area.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/page_table_area.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PageTableArea.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/page_table_area_cell.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/page_table_area_cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PageTableAreaCell.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/page_text_area.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/page_text_area.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PageTextArea.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/parse_options.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/parse_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ParseOptions.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/parse_result.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/parse_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ParseResult.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/parser_options.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/parser_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ParserOptions.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/point.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Point.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/rectangle.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/rectangle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Rectangle.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/size.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/size.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Size.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/storage_exist.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/storage_exist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StorageExist.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/storage_file.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/storage_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StorageFile.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/table.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Table.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/table_layout.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/table_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TableLayout.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/template.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Template.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/template_options.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/template_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TemplateOptions.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/template_result.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/template_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TemplateResult.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/text_options.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/text_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TextOptions.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/text_page.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/text_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TextPage.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/text_result.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/text_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TextResult.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/models/text_style.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/models/text_style.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TextStyle.py">
-#   Copyright (c) 2003-2019 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud/rest.py` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud/rest.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud.egg-info/PKG-INFO` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: groupdocs-parser-cloud
-Version: 22.3
+Version: 23.7
 Summary: GroupDocs.Parser Cloud Python SDK
 Home-page: http://github.com/groupdocs-parser-cloud/groupdocs-parser-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
-License: UNKNOWN
 Keywords: groupdocs,parser,cloud,python,sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -75,8 +73,7 @@
 + [**Product Home**](https://products.groupdocs.cloud/parser)
 + [**Documentation**](https://docs.groupdocs.cloud/display/parsercloud/Home)
 + [**Free Support Forum**](https://forum.groupdocs.cloud/c/parser)
 + [**Blog**](https://blog.groupdocs.cloud/category/parser)
 
 ## Contact Us
 Your feedback is very important to us. Please feel free to contact us using our [Support Forums](https://forum.groupdocs.cloud/c/parser).
-
```

### Comparing `groupdocs-parser-cloud-22.3/groupdocs_parser_cloud.egg-info/SOURCES.txt` & `groupdocs-parser-cloud-23.7/groupdocs_parser_cloud.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 groupdocs_parser_cloud/apis/file_api.py
 groupdocs_parser_cloud/apis/folder_api.py
 groupdocs_parser_cloud/apis/info_api.py
 groupdocs_parser_cloud/apis/parse_api.py
 groupdocs_parser_cloud/apis/storage_api.py
 groupdocs_parser_cloud/apis/template_api.py
 groupdocs_parser_cloud/models/__init__.py
+groupdocs_parser_cloud/models/barcode.py
+groupdocs_parser_cloud/models/barcode_page.py
+groupdocs_parser_cloud/models/barcodes_options.py
+groupdocs_parser_cloud/models/barcodes_result.py
 groupdocs_parser_cloud/models/container_item.py
 groupdocs_parser_cloud/models/container_item_info.py
 groupdocs_parser_cloud/models/container_options.py
 groupdocs_parser_cloud/models/container_result.py
 groupdocs_parser_cloud/models/coordinates.py
 groupdocs_parser_cloud/models/create_template_options.py
 groupdocs_parser_cloud/models/detector_parameters.py
@@ -76,14 +80,15 @@
 test/test_context.py
 test/test_file.py
 test/test_settings.py
 test/apis/__init__.py
 test/apis/test_auth_api.py
 test/apis/test_file_api.py
 test/apis/test_folder_api.py
+test/apis/test_parser_barcode_api.py
 test/apis/test_parser_container_api.py
 test/apis/test_parser_formats_api.py
 test/apis/test_parser_image_api.py
 test/apis/test_parser_info_api.py
 test/apis/test_parser_parse_api.py
 test/apis/test_parser_template_api.py
 test/apis/test_parser_text_api.py
```

### Comparing `groupdocs-parser-cloud-22.3/setup.py` & `groupdocs-parser-cloud-23.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import datetime
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "groupdocs-parser-cloud"
-VERSION = "22.3"
+VERSION = "23.7"
 
 # Append current time to the version when publishing to test environment
 if "--test" in sys.argv:
     VERSION += "." + datetime.datetime.now().strftime("%Y%m%d%H%M")
     sys.argv.remove("--test")
 
 # To install the library, run the following
```

### Comparing `groupdocs-parser-cloud-22.3/test/apis/test_auth_api.py` & `groupdocs-parser-cloud-23.7/test/apis/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/test/apis/test_file_api.py` & `groupdocs-parser-cloud-23.7/test/apis/test_file_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/test/apis/test_folder_api.py` & `groupdocs-parser-cloud-23.7/test/apis/test_folder_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/test/apis/test_parser_container_api.py` & `groupdocs-parser-cloud-23.7/test/apis/test_parser_container_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,19 +57,19 @@
         request = ContainerRequest(container_options)
         with self.assertRaises(ApiException) as context:
             self.info_api.container(request)
         self.assertEqual("Can't find file located at 'folder\\file-not-exist.pdf'.", get_error_message(context.exception.message))
 
     def test_get_container_item_info_unsupported_file(self):
         container_options = ContainerOptions()
-        container_options.file_info = TestFile.four_pages().ToFileInfo()
+        container_options.file_info = TestFile.video().ToFileInfo()
         request = ContainerRequest(container_options)
         with self.assertRaises(ApiException) as context:
             self.info_api.container(request)
-        self.assertEqual("The specified file 'words\\docx\\four-pages.docx' has type which is not currently supported.", get_error_message(context.exception.message))
+        self.assertEqual("The specified file 'video\\avi\\sample.avi' has type which is not currently supported.", get_error_message(context.exception.message))
 
     def test_get_container_item_info_rar(self):
             """
             Test case for test_get_container_item_info_rar
 
             Retrieve information about document.
             """
```

### Comparing `groupdocs-parser-cloud-22.3/test/apis/test_parser_formats_api.py` & `groupdocs-parser-cloud-23.7/test/apis/test_parser_formats_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/test/apis/test_parser_image_api.py` & `groupdocs-parser-cloud-23.7/test/apis/test_parser_image_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/test/apis/test_parser_info_api.py` & `groupdocs-parser-cloud-23.7/test/apis/test_parser_info_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/test/apis/test_parser_parse_api.py` & `groupdocs-parser-cloud-23.7/test/apis/test_parser_parse_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/test/apis/test_parser_template_api.py` & `groupdocs-parser-cloud-23.7/test/apis/test_parser_template_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/test/apis/test_parser_text_api.py` & `groupdocs-parser-cloud-23.7/test/apis/test_parser_text_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/test/apis/test_storage_api.py` & `groupdocs-parser-cloud-23.7/test/apis/test_storage_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/test/test_context.py` & `groupdocs-parser-cloud-23.7/test/test_context.py`

 * *Files identical despite different names*

### Comparing `groupdocs-parser-cloud-22.3/test/test_file.py` & `groupdocs-parser-cloud-23.7/test/test_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,21 @@
 
     @classmethod
     def four_pages(cls):
         f = TestFile()
         f.file_name = "four-pages.docx"
         f.folder = "words\\docx\\"
         return f
+    
+    @classmethod
+    def barcode(cls):
+        f = TestFile()
+        f.file_name = "barcodes.docx"
+        f.folder = "words\\docx\\"
+        return f
 
     @classmethod
     def one_page(cls):
         f = TestFile()
         f.file_name = "one-page.docx"
         f.folder = "words\\docx\\"
         return f
@@ -137,14 +144,21 @@
     def md(cls):
         f = TestFile()
         f.file_name = "sample.md"
         f.folder = "words\\docx\\"
         return f
 
     @classmethod
+    def video(cls):
+        f = TestFile()
+        f.file_name = "sample.avi"
+        f.folder = "video\\avi\\"
+        return f
+
+    @classmethod
     def not_exist(cls):
         f = TestFile()
         f.file_name = "file-not-exist.pdf"
         f.folder = "folder\\"
         return f
 
     @classmethod
```

### Comparing `groupdocs-parser-cloud-22.3/test/test_settings.py` & `groupdocs-parser-cloud-23.7/test/test_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_context.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2019 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -22,11 +22,12 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 # </summary>
 # -----------------------------------------------------------------------------------
 
 class TestSettings:
-# Get your AppSID and AppKey at https://dashboard.groupdocs.cloud (free registration is required).
-    APP_SID="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
-    APP_KEY="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
-    API_BASE_URL="https://api.groupdocs.cloud"
+    """Test settings"""
+
+    APP_SID="parser.cloud"
+    APP_KEY="parser.cloud"
+    API_BASE_URL="https://api-qa.groupdocs.cloud"
```


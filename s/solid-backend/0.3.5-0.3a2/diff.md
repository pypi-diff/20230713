# Comparing `tmp/solid_backend-0.3.5.tar.gz` & `tmp/solid_backend-0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solid_backend-0.3.5.tar", max compression
+gzip compressed data, was "solid_backend-0.3a2.tar", max compression
```

## Comparing `solid_backend-0.3.5.tar` & `solid_backend-0.3a2.tar`

### file list

```diff
@@ -1,167 +1,166 @@
--rw-r--r--   0        0        0     1084 2022-11-17 14:17:18.883941 solid_backend-0.3.5/LICENSE
--rw-r--r--   0        0        0     5327 2022-11-17 14:17:18.883941 solid_backend-0.3.5/README.md
--rw-r--r--   0        0        0     1232 2023-07-13 10:16:13.583134 solid_backend-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      111 2023-06-29 13:15:59.169552 solid_backend-0.3.5/solid_backend/__init__.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/contact/__init__.py
--rw-r--r--   0        0        0      103 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/contact/apps.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/contact/migrations/__init__.py
--rw-r--r--   0        0        0      238 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/contact/serializers.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/contact/tests/__init__.py
--rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/contact/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/contact/tests/conftest_files/__init__.py
--rw-r--r--   0        0        0      178 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/contact/tests/conftest_files/general_conftest.py
--rw-r--r--   0        0        0     1515 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/contact/tests/test_serializers.py
--rw-r--r--   0        0        0      133 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/contact/urls.py
--rw-r--r--   0        0        0     1441 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/contact/views.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/__init__.py
--rw-r--r--   0        0        0      156 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/admin.py
--rw-r--r--   0        0        0      103 2022-12-12 10:34:03.668113 solid_backend-0.3.5/solid_backend/content/apps.py
--rw-r--r--   0        0        0     5449 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/fields.py
--rw-r--r--   0        0        0     1776 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/migrations/0001_create_tree_node_model.py
--rw-r--r--   0        0        0      306 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/migrations/0002_remove_treenode_is_top_level.py
--rw-r--r--   0        0        0      352 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/migrations/0003_rename_treenode_node_name.py
--rw-r--r--   0        0        0      349 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/migrations/0004_rename_treenode_info_text.py
--rw-r--r--   0        0        0     1030 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/migrations/0005_alter_treenode_name_attributes.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/migrations/__init__.py
--rw-r--r--   0        0        0     2273 2022-12-08 19:51:54.045396 solid_backend-0.3.5/solid_backend/content/models.py
--rw-r--r--   0        0        0     1102 2023-06-29 09:52:23.534706 solid_backend-0.3.5/solid_backend/content/serializers.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/tests/__init__.py
--rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/tests/conftest_files/__init__.py
--rw-r--r--   0        0        0      218 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/tests/conftest_files/general_conftest.py
--rw-r--r--   0        0        0     3201 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/content/tests/test_base_models.py
--rw-r--r--   0        0        0      240 2023-06-29 09:52:23.534706 solid_backend-0.3.5/solid_backend/content/urls.py
--rw-r--r--   0        0        0     1365 2023-06-29 12:37:55.571166 solid_backend-0.3.5/solid_backend/content/views.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/__init__.py
--rw-r--r--   0        0        0      281 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/admin.py
--rw-r--r--   0        0        0      105 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/apps.py
--rw-r--r--   0        0        0      520 2022-12-05 17:35:54.547219 solid_backend-0.3.5/solid_backend/glossary/forms.py
--rw-r--r--   0        0        0     1152 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/migrations/0001_implement_glossary_entry_model.py
--rw-r--r--   0        0        0      435 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/migrations/0002_update_image_upload_path.py
--rw-r--r--   0        0        0      415 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/migrations/0003_add_verbose_name_to_text_field.py
--rw-r--r--   0        0        0      388 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/migrations/0004_remove_img_fields.py
--rw-r--r--   0        0        0      693 2022-12-05 17:35:54.555220 solid_backend-0.3.5/solid_backend/glossary/migrations/0005_fields_optional.py
--rw-r--r--   0        0        0      339 2022-12-08 14:22:00.611634 solid_backend-0.3.5/solid_backend/glossary/migrations/0006_auto_20220217_1858.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/migrations/__init__.py
--rw-r--r--   0        0        0      469 2022-12-05 17:35:54.547219 solid_backend-0.3.5/solid_backend/glossary/models.py
--rw-r--r--   0        0        0      209 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/serializers.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/tests/__init__.py
--rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/tests/conftest_files/__init__.py
--rw-r--r--   0        0        0      148 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/tests/conftest_files/general_conftest.py
--rw-r--r--   0        0        0     1596 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/tests/test_base_models.py
--rw-r--r--   0        0        0      240 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/urls.py
--rw-r--r--   0        0        0      536 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/glossary/views.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/__init__.py
--rw-r--r--   0        0        0     3659 2022-12-08 14:22:00.611634 solid_backend-0.3.5/solid_backend/media_object/admin.py
--rw-r--r--   0        0        0      112 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/apps.py
--rw-r--r--   0        0        0     5296 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/forms.py
--rw-r--r--   0        0        0     4584 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/migrations/0001_initial.py
--rw-r--r--   0        0        0      672 2022-12-05 17:35:54.555220 solid_backend-0.3.5/solid_backend/media_object/migrations/0002_audiovideomediaobject_imagemediaobject.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/migrations/__init__.py
--rw-r--r--   0        0        0     6269 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/media_object/models.py
--rw-r--r--   0        0        0     2021 2023-07-06 14:06:58.349792 solid_backend-0.3.5/solid_backend/media_object/serializers.py
--rw-r--r--   0        0        0       52 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/static/media_object/css/radio.css
--rw-r--r--   0        0        0     1922 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/static/media_object/js/hide_elements.js
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/tests/__init__.py
--rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/tests/conftest_files/__init__.py
--rw-r--r--   0        0        0      218 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/tests/conftest_files/general_conftest.py
--rw-r--r--   0        0        0     5753 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/tests/test_base_models.py
--rw-r--r--   0        0        0      238 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/urls.py
--rw-r--r--   0        0        0      383 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/media_object/views.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/__init__.py
--rw-r--r--   0        0        0      790 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/admin.py
--rw-r--r--   0        0        0      103 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/apps.py
--rw-r--r--   0        0        0     1580 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/migrations/0001_implement_message_model.py
--rw-r--r--   0        0        0      503 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/migrations/0002_correct_typo.py
--rw-r--r--   0        0        0      391 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/migrations/0003_make_valid_to_optional.py
--rw-r--r--   0        0        0     2870 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/migrations/0004_assign_photograph_as_img_field.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/migrations/__init__.py
--rw-r--r--   0        0        0      731 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/models.py
--rw-r--r--   0        0        0      310 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/serializers.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/tests/__init__.py
--rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/tests/conftest_files/__init__.py
--rw-r--r--   0        0        0      253 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/tests/conftest_files/general_conftest.py
--rw-r--r--   0        0        0     2465 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/tests/test_base_models.py
--rw-r--r--   0        0        0      220 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/message/urls.py
--rw-r--r--   0        0        0      669 2022-12-05 17:35:54.563220 solid_backend-0.3.5/solid_backend/message/views.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/openzoom/__init__.py
--rw-r--r--   0        0        0    22308 2022-12-08 19:51:54.045396 solid_backend-0.3.5/solid_backend/openzoom/deepzoom.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/__init__.py
--rw-r--r--   0        0        0     2395 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/admin.py
--rw-r--r--   0        0        0      109 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/apps.py
--rw-r--r--   0        0        0     2378 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/forms.py
--rw-r--r--   0        0        0     2097 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/migrations/0001_implement_photograph_model.py
--rw-r--r--   0        0        0      602 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/migrations/0002_add_audio_fields.py
--rw-r--r--   0        0        0      788 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/migrations/0003_create_generic_foreign_key.py
--rw-r--r--   0        0        0      730 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/migrations/0004_add_verbose_names.py
--rw-r--r--   0        0        0      674 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/migrations/0005_implement_deep_zoom_fields.py
--rw-r--r--   0        0        0      433 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/migrations/0006_add_profile_position_field.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/migrations/__init__.py
--rw-r--r--   0        0        0     4320 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/models.py
--rw-r--r--   0        0        0     1870 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/serializers.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/tests/__init__.py
--rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/tests/conftest_files/__init__.py
--rw-r--r--   0        0        0      216 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/tests/conftest_files/general_conftest.py
--rw-r--r--   0        0        0     5640 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/tests/test_base_models.py
--rw-r--r--   0        0        0      232 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/urls.py
--rw-r--r--   0        0        0      376 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/photograph/views.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/quiz/__init__.py
--rw-r--r--   0        0        0      888 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/admin.py
--rw-r--r--   0        0        0       97 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/quiz/apps.py
--rw-r--r--   0        0        0     6168 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/forms.py
--rw-r--r--   0        0        0     2217 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/quiz/migrations/0001_implement_quiz_question_model.py
--rw-r--r--   0        0        0     1450 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/quiz/migrations/0002_implement_quiz_answer_model.py
--rw-r--r--   0        0        0      601 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/quiz/migrations/0003_add_verbose_name_to_text_fields.py
--rw-r--r--   0        0        0     2748 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/quiz/migrations/0004_assign_photograph_as_img_field.py
--rw-r--r--   0        0        0     2861 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/migrations/0005_auto_20220222_1829.py
--rw-r--r--   0        0        0     4410 2022-12-08 19:52:19.737717 solid_backend-0.3.5/solid_backend/quiz/migrations/0006_auto_20220308_1744.py
--rw-r--r--   0        0        0      294 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/migrations/0007_remove_quizquestion_img.py
--rw-r--r--   0        0        0     2046 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/migrations/0008_quizquestion_new_tags.py
--rw-r--r--   0        0        0      496 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/migrations/0009_auto_20220315_1718.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/quiz/migrations/__init__.py
--rw-r--r--   0        0        0     2462 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/models.py
--rw-r--r--   0        0        0     1789 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/serializers.py
--rw-r--r--   0        0        0     1440 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/static/quiz/js/hide_columns.js
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/quiz/tests/__init__.py
--rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/quiz/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/quiz/tests/conftest_files/__init__.py
--rw-r--r--   0        0        0      355 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/tests/conftest_files/general_conftest.py
--rw-r--r--   0        0        0     4865 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/tests/test_base_models.py
--rw-r--r--   0        0        0      508 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/urls.py
--rw-r--r--   0        0        0     2763 2022-12-08 14:22:00.615635 solid_backend-0.3.5/solid_backend/quiz/views.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/__init__.py
--rw-r--r--   0        0        0     2319 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/admin.py
--rw-r--r--   0        0        0      107 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/apps.py
--rw-r--r--   0        0        0     1717 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/forms.py
--rw-r--r--   0        0        0      663 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/0001_implement_slideshow_model.py
--rw-r--r--   0        0        0     1246 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/0002_implement_slideshow_page_model.py
--rw-r--r--   0        0        0     1414 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/0003_implement_slideshow_image_model.py
--rw-r--r--   0        0        0      659 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/0004_add_verbose_name_to_text_fields.py
--rw-r--r--   0        0        0      612 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/0005_add_img_fields_slideshow_model.py
--rw-r--r--   0        0        0     2899 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/0006_assign_photograph_as_img_field_slideshow_model.py
--rw-r--r--   0        0        0     2947 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/0007_assign_photograph_as_img_field_slideshow_image_model.py
--rw-r--r--   0        0        0      957 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/0008_add_active_and_position_field_slideshow_model.py
--rw-r--r--   0        0        0      754 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/0009_remove_default_from_position_fields.py
--rw-r--r--   0        0        0      363 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/0010_rename_slideshow_img.py
--rw-r--r--   0        0        0      347 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/0011_rename_slideshowimage_img.py
--rw-r--r--   0        0        0      662 2022-12-05 17:37:02.248116 solid_backend-0.3.5/solid_backend/slideshow/migrations/0012_add_taggit_tags.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/migrations/__init__.py
--rw-r--r--   0        0        0     1709 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/models.py
--rw-r--r--   0        0        0     2344 2023-03-06 15:03:23.115802 solid_backend-0.3.5/solid_backend/slideshow/serializers.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/tests/__init__.py
--rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/tests/conftest_files/__init__.py
--rw-r--r--   0        0        0      448 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/tests/conftest_files/general_conftest.py
--rw-r--r--   0        0        0     6891 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/slideshow/tests/test_base_models.py
--rw-r--r--   0        0        0      481 2022-12-08 14:26:29.080008 solid_backend-0.3.5/solid_backend/slideshow/urls.py
--rw-r--r--   0        0        0     2895 2022-12-08 14:27:17.761609 solid_backend-0.3.5/solid_backend/slideshow/views.py
--rw-r--r--   0        0        0      666 2022-11-17 14:17:18.887941 solid_backend-0.3.5/solid_backend/urls.py
--rw-r--r--   0        0        0        0 2023-06-29 12:46:50.307354 solid_backend-0.3.5/solid_backend/utils/__init__.py
--rw-r--r--   0        0        0     3737 2023-07-13 10:16:13.583134 solid_backend-0.3.5/solid_backend/utils/drf_spectacular_extensions.py
--rw-r--r--   0        0        0     1813 2023-07-13 10:11:44.371128 solid_backend-0.3.5/solid_backend/utils/serializers.py
--rw-r--r--   0        0        0     7849 1970-01-01 00:00:00.000000 solid_backend-0.3.5/setup.py
--rw-r--r--   0        0        0     6494 1970-01-01 00:00:00.000000 solid_backend-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-11-17 14:17:18.883941 solid_backend-0.3a2/LICENSE
+-rw-r--r--   0        0        0     5327 2022-11-17 14:17:18.883941 solid_backend-0.3a2/README.md
+-rw-r--r--   0        0        0     1164 2022-12-08 20:00:59.272211 solid_backend-0.3a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/contact/__init__.py
+-rw-r--r--   0        0        0      103 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/contact/apps.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/contact/migrations/__init__.py
+-rw-r--r--   0        0        0      238 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/contact/serializers.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/contact/tests/__init__.py
+-rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/contact/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/contact/tests/conftest_files/__init__.py
+-rw-r--r--   0        0        0      178 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/contact/tests/conftest_files/general_conftest.py
+-rw-r--r--   0        0        0     1515 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/contact/tests/test_serializers.py
+-rw-r--r--   0        0        0      133 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/contact/urls.py
+-rw-r--r--   0        0        0     1441 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/contact/views.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/__init__.py
+-rw-r--r--   0        0        0      156 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/admin.py
+-rw-r--r--   0        0        0      103 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/apps.py
+-rw-r--r--   0        0        0     5449 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/fields.py
+-rw-r--r--   0        0        0     1776 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/migrations/0001_create_tree_node_model.py
+-rw-r--r--   0        0        0      306 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/migrations/0002_remove_treenode_is_top_level.py
+-rw-r--r--   0        0        0      352 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/migrations/0003_rename_treenode_node_name.py
+-rw-r--r--   0        0        0      349 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/migrations/0004_rename_treenode_info_text.py
+-rw-r--r--   0        0        0     1030 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/migrations/0005_alter_treenode_name_attributes.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/migrations/__init__.py
+-rw-r--r--   0        0        0     2273 2022-12-08 19:51:54.045396 solid_backend-0.3a2/solid_backend/content/models.py
+-rw-r--r--   0        0        0     1268 2022-12-08 19:51:54.045396 solid_backend-0.3a2/solid_backend/content/serializers.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/tests/__init__.py
+-rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/tests/conftest_files/__init__.py
+-rw-r--r--   0        0        0      218 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/tests/conftest_files/general_conftest.py
+-rw-r--r--   0        0        0     3201 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/tests/test_base_models.py
+-rw-r--r--   0        0        0      240 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/urls.py
+-rw-r--r--   0        0        0     1398 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/content/views.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/__init__.py
+-rw-r--r--   0        0        0      281 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/admin.py
+-rw-r--r--   0        0        0      105 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/apps.py
+-rw-r--r--   0        0        0      520 2022-12-05 17:35:54.547219 solid_backend-0.3a2/solid_backend/glossary/forms.py
+-rw-r--r--   0        0        0     1152 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/migrations/0001_implement_glossary_entry_model.py
+-rw-r--r--   0        0        0      435 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/migrations/0002_update_image_upload_path.py
+-rw-r--r--   0        0        0      415 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/migrations/0003_add_verbose_name_to_text_field.py
+-rw-r--r--   0        0        0      388 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/migrations/0004_remove_img_fields.py
+-rw-r--r--   0        0        0      693 2022-12-05 17:35:54.555220 solid_backend-0.3a2/solid_backend/glossary/migrations/0005_fields_optional.py
+-rw-r--r--   0        0        0      339 2022-12-08 14:22:00.611634 solid_backend-0.3a2/solid_backend/glossary/migrations/0006_auto_20220217_1858.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/migrations/__init__.py
+-rw-r--r--   0        0        0      469 2022-12-05 17:35:54.547219 solid_backend-0.3a2/solid_backend/glossary/models.py
+-rw-r--r--   0        0        0      209 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/serializers.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/tests/__init__.py
+-rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/tests/conftest_files/__init__.py
+-rw-r--r--   0        0        0      148 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/tests/conftest_files/general_conftest.py
+-rw-r--r--   0        0        0     1596 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/tests/test_base_models.py
+-rw-r--r--   0        0        0      240 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/urls.py
+-rw-r--r--   0        0        0      536 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/glossary/views.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/__init__.py
+-rw-r--r--   0        0        0     3659 2022-12-08 14:22:00.611634 solid_backend-0.3a2/solid_backend/media_object/admin.py
+-rw-r--r--   0        0        0      112 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/apps.py
+-rw-r--r--   0        0        0     5296 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/forms.py
+-rw-r--r--   0        0        0     4584 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/migrations/0001_initial.py
+-rw-r--r--   0        0        0      672 2022-12-05 17:35:54.555220 solid_backend-0.3a2/solid_backend/media_object/migrations/0002_audiovideomediaobject_imagemediaobject.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/migrations/__init__.py
+-rw-r--r--   0        0        0     6269 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/media_object/models.py
+-rw-r--r--   0        0        0     2021 2022-12-05 17:35:54.583220 solid_backend-0.3a2/solid_backend/media_object/serializers.py
+-rw-r--r--   0        0        0       52 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/static/media_object/css/radio.css
+-rw-r--r--   0        0        0     1922 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/static/media_object/js/hide_elements.js
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/tests/__init__.py
+-rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/tests/conftest_files/__init__.py
+-rw-r--r--   0        0        0      218 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/tests/conftest_files/general_conftest.py
+-rw-r--r--   0        0        0     5753 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/tests/test_base_models.py
+-rw-r--r--   0        0        0      238 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/urls.py
+-rw-r--r--   0        0        0      383 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/media_object/views.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/__init__.py
+-rw-r--r--   0        0        0      790 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/admin.py
+-rw-r--r--   0        0        0      103 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/apps.py
+-rw-r--r--   0        0        0     1580 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/migrations/0001_implement_message_model.py
+-rw-r--r--   0        0        0      503 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/migrations/0002_correct_typo.py
+-rw-r--r--   0        0        0      391 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/migrations/0003_make_valid_to_optional.py
+-rw-r--r--   0        0        0     2870 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/migrations/0004_assign_photograph_as_img_field.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/migrations/__init__.py
+-rw-r--r--   0        0        0      731 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/models.py
+-rw-r--r--   0        0        0      310 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/serializers.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/tests/__init__.py
+-rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/tests/conftest_files/__init__.py
+-rw-r--r--   0        0        0      253 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/tests/conftest_files/general_conftest.py
+-rw-r--r--   0        0        0     2465 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/tests/test_base_models.py
+-rw-r--r--   0        0        0      220 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/message/urls.py
+-rw-r--r--   0        0        0      669 2022-12-05 17:35:54.563220 solid_backend-0.3a2/solid_backend/message/views.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/openzoom/__init__.py
+-rw-r--r--   0        0        0    22308 2022-12-08 19:51:54.045396 solid_backend-0.3a2/solid_backend/openzoom/deepzoom.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/__init__.py
+-rw-r--r--   0        0        0     2395 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/admin.py
+-rw-r--r--   0        0        0      109 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/apps.py
+-rw-r--r--   0        0        0     2378 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/forms.py
+-rw-r--r--   0        0        0     2097 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/migrations/0001_implement_photograph_model.py
+-rw-r--r--   0        0        0      602 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/migrations/0002_add_audio_fields.py
+-rw-r--r--   0        0        0      788 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/migrations/0003_create_generic_foreign_key.py
+-rw-r--r--   0        0        0      730 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/migrations/0004_add_verbose_names.py
+-rw-r--r--   0        0        0      674 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/migrations/0005_implement_deep_zoom_fields.py
+-rw-r--r--   0        0        0      433 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/migrations/0006_add_profile_position_field.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/migrations/__init__.py
+-rw-r--r--   0        0        0     4320 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/models.py
+-rw-r--r--   0        0        0     1870 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/serializers.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/tests/__init__.py
+-rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/tests/conftest_files/__init__.py
+-rw-r--r--   0        0        0      216 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/tests/conftest_files/general_conftest.py
+-rw-r--r--   0        0        0     5640 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/tests/test_base_models.py
+-rw-r--r--   0        0        0      232 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/urls.py
+-rw-r--r--   0        0        0      376 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/photograph/views.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/quiz/__init__.py
+-rw-r--r--   0        0        0      888 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/admin.py
+-rw-r--r--   0        0        0       97 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/quiz/apps.py
+-rw-r--r--   0        0        0     6168 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/forms.py
+-rw-r--r--   0        0        0     2217 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/quiz/migrations/0001_implement_quiz_question_model.py
+-rw-r--r--   0        0        0     1450 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/quiz/migrations/0002_implement_quiz_answer_model.py
+-rw-r--r--   0        0        0      601 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/quiz/migrations/0003_add_verbose_name_to_text_fields.py
+-rw-r--r--   0        0        0     2748 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/quiz/migrations/0004_assign_photograph_as_img_field.py
+-rw-r--r--   0        0        0     2861 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/migrations/0005_auto_20220222_1829.py
+-rw-r--r--   0        0        0     4410 2022-12-08 19:52:19.737717 solid_backend-0.3a2/solid_backend/quiz/migrations/0006_auto_20220308_1744.py
+-rw-r--r--   0        0        0      294 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/migrations/0007_remove_quizquestion_img.py
+-rw-r--r--   0        0        0     2046 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/migrations/0008_quizquestion_new_tags.py
+-rw-r--r--   0        0        0      496 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/migrations/0009_auto_20220315_1718.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/quiz/migrations/__init__.py
+-rw-r--r--   0        0        0     2462 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/models.py
+-rw-r--r--   0        0        0     1789 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/serializers.py
+-rw-r--r--   0        0        0     1440 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/static/quiz/js/hide_columns.js
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/quiz/tests/__init__.py
+-rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/quiz/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/quiz/tests/conftest_files/__init__.py
+-rw-r--r--   0        0        0      355 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/tests/conftest_files/general_conftest.py
+-rw-r--r--   0        0        0     4865 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/tests/test_base_models.py
+-rw-r--r--   0        0        0      508 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/urls.py
+-rw-r--r--   0        0        0     2763 2022-12-08 14:22:00.615635 solid_backend-0.3a2/solid_backend/quiz/views.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/__init__.py
+-rw-r--r--   0        0        0     2319 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/admin.py
+-rw-r--r--   0        0        0      107 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/apps.py
+-rw-r--r--   0        0        0     1717 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/forms.py
+-rw-r--r--   0        0        0      663 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/0001_implement_slideshow_model.py
+-rw-r--r--   0        0        0     1246 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/0002_implement_slideshow_page_model.py
+-rw-r--r--   0        0        0     1414 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/0003_implement_slideshow_image_model.py
+-rw-r--r--   0        0        0      659 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/0004_add_verbose_name_to_text_fields.py
+-rw-r--r--   0        0        0      612 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/0005_add_img_fields_slideshow_model.py
+-rw-r--r--   0        0        0     2899 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/0006_assign_photograph_as_img_field_slideshow_model.py
+-rw-r--r--   0        0        0     2947 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/0007_assign_photograph_as_img_field_slideshow_image_model.py
+-rw-r--r--   0        0        0      957 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/0008_add_active_and_position_field_slideshow_model.py
+-rw-r--r--   0        0        0      754 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/0009_remove_default_from_position_fields.py
+-rw-r--r--   0        0        0      363 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/0010_rename_slideshow_img.py
+-rw-r--r--   0        0        0      347 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/0011_rename_slideshowimage_img.py
+-rw-r--r--   0        0        0      662 2022-12-05 17:37:02.248116 solid_backend-0.3a2/solid_backend/slideshow/migrations/0012_add_taggit_tags.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/migrations/__init__.py
+-rw-r--r--   0        0        0     1709 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/models.py
+-rw-r--r--   0        0        0     2344 2022-12-05 17:35:54.591220 solid_backend-0.3a2/solid_backend/slideshow/serializers.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/tests/__init__.py
+-rw-r--r--   0        0        0       47 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/tests/conftest_files/__init__.py
+-rw-r--r--   0        0        0      448 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/tests/conftest_files/general_conftest.py
+-rw-r--r--   0        0        0     6891 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/slideshow/tests/test_base_models.py
+-rw-r--r--   0        0        0      481 2022-12-08 14:26:29.080008 solid_backend-0.3a2/solid_backend/slideshow/urls.py
+-rw-r--r--   0        0        0     2895 2022-12-08 14:27:17.761609 solid_backend-0.3a2/solid_backend/slideshow/views.py
+-rw-r--r--   0        0        0      666 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/urls.py
+-rw-r--r--   0        0        0        0 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/utils/__init__.py
+-rw-r--r--   0        0        0      966 2022-11-17 14:17:18.887941 solid_backend-0.3a2/solid_backend/utils/serializers.py
+-rw-r--r--   0        0        0     7849 1970-01-01 00:00:00.000000 solid_backend-0.3a2/setup.py
+-rw-r--r--   0        0        0     6494 1970-01-01 00:00:00.000000 solid_backend-0.3a2/PKG-INFO
```

### Comparing `solid_backend-0.3.5/LICENSE` & `solid_backend-0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/README.md` & `solid_backend-0.3a2/README.md`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/pyproject.toml` & `solid_backend-0.3a2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solid-backend"
-version = "0.3.5"
+version = "0.3.a2"
 
 description = "Clean Django app for e-learning application with..."
 authors = [
 	"Christian Grossmüller <chgad.games@gmail.com>",
 	"Timotheus Kozlowski <kozlowski@itp.uni-frankfurt.de>"
 ]
 license = "MIT"
@@ -12,15 +12,15 @@
 readme = "README.md"
 homepage = "https://github.com/zentrumnawi/solid-backend"
 repository = "https://github.com/zentrumnawi/solid-backend"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-django = "^3.0.7"
+django = "~3.0.7"
 djangorestframework = "3.11.0"
 django-mptt = "0.11.0"
 pillow = "7.1.2"
 django-cleanup = "4.0.0"
 psycopg2-binary = "^2.8.5"
 mutagen = "^1.44.0"
 django-stdimage = "^5.1.1"
@@ -44,13 +44,10 @@
 pytest-cov = "2.9.0"
 codecov = "2.1.4"
 black = "19.10b0"
 flake8 = "*"
 drf-yasg = "^1.20.0"
 
 
-[tool.poetry.group.extras.dependencies]
-drf-spectacular = "^0.25.1"
-
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `solid_backend-0.3.5/solid_backend/contact/tests/test_serializers.py` & `solid_backend-0.3a2/solid_backend/contact/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/contact/views.py` & `solid_backend-0.3a2/solid_backend/contact/views.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/content/fields.py` & `solid_backend-0.3a2/solid_backend/content/fields.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/content/migrations/0001_create_tree_node_model.py` & `solid_backend-0.3a2/solid_backend/content/migrations/0001_create_tree_node_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/content/migrations/0005_alter_treenode_name_attributes.py` & `solid_backend-0.3a2/solid_backend/content/migrations/0005_alter_treenode_name_attributes.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/content/models.py` & `solid_backend-0.3a2/solid_backend/content/models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/content/serializers.py` & `solid_backend-0.3a2/solid_backend/content/serializers.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,29 +3,36 @@
 from django.conf import settings
 from rest_framework import serializers
 
 from solid_backend.utils.serializers import RecursiveSerializer
 
 from .models import TreeNode
 
-SERIALIZERS = {}
+SERIALIZERS = []
 
 if hasattr(settings, "PROFILES_SERIALIZERS"):
     for field_name in settings.PROFILES_SERIALIZERS:
-        module, serializer = settings.PROFILES_SERIALIZERS[field_name]
-        SERIALIZERS[field_name] = getattr(import_module(module), serializer)
+        SERIALIZERS.append(
+            (
+                field_name,
+                getattr(
+                    import_module(settings.PROFILES_SERIALIZER_MODULE),
+                    settings.PROFILES_SERIALIZER_NAME,
+                )(many=True, required=False),
+            )
+        )
 
 
 class TreeNodeSerializer(serializers.ModelSerializer):
-    def build_nested_field(self, field_name, relation_info, nested_depth):
-        if SERIALIZERS.get(field_name) is not None:
-            return SERIALIZERS.get(field_name), {"many": True, "required": False}
-        return super(TreeNodeSerializer, self).build_nested_field(
-            field_name, relation_info, nested_depth
-        )
+    # To use a custom serializer for the profiles field, it must be specified in the
+    # settings with PROFILES_SERIALIZER_MODULE and PROFILES_SERIALIZER_NAME.
+    def __init__(self, *args, **kwargs):
+        super(TreeNodeSerializer, self).__init__(*args, **kwargs)
+        for field, serializer in SERIALIZERS:
+            setattr(self, field, serializer)
 
     children = RecursiveSerializer(many=True, required=False)
 
     class Meta:
         model = TreeNode
         fields = ("name", "info", "children") + tuple(
             settings.PROFILES_SERIALIZERS.keys()
```

### Comparing `solid_backend-0.3.5/solid_backend/content/tests/test_base_models.py` & `solid_backend-0.3a2/solid_backend/content/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/content/views.py` & `solid_backend-0.3a2/solid_backend/content/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django.conf import settings
 from django.db.models import Prefetch
 from rest_framework.viewsets import ReadOnlyModelViewSet
 
 from solid_backend.media_object.models import MediaObject
 
 from .models import TreeNode
 from .serializers import TreeNodeSerializer
```

### Comparing `solid_backend-0.3.5/solid_backend/glossary/forms.py` & `solid_backend-0.3a2/solid_backend/glossary/forms.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/glossary/migrations/0001_implement_glossary_entry_model.py` & `solid_backend-0.3a2/solid_backend/glossary/migrations/0001_implement_glossary_entry_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/glossary/migrations/0005_fields_optional.py` & `solid_backend-0.3a2/solid_backend/glossary/migrations/0005_fields_optional.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/glossary/tests/test_base_models.py` & `solid_backend-0.3a2/solid_backend/glossary/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/glossary/views.py` & `solid_backend-0.3a2/solid_backend/glossary/views.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/media_object/admin.py` & `solid_backend-0.3a2/solid_backend/media_object/admin.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/media_object/forms.py` & `solid_backend-0.3a2/solid_backend/media_object/forms.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/media_object/migrations/0001_initial.py` & `solid_backend-0.3a2/solid_backend/media_object/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/media_object/migrations/0002_audiovideomediaobject_imagemediaobject.py` & `solid_backend-0.3a2/solid_backend/media_object/migrations/0002_audiovideomediaobject_imagemediaobject.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/media_object/models.py` & `solid_backend-0.3a2/solid_backend/media_object/models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/media_object/serializers.py` & `solid_backend-0.3a2/solid_backend/media_object/serializers.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/media_object/static/media_object/js/hide_elements.js` & `solid_backend-0.3a2/solid_backend/media_object/static/media_object/js/hide_elements.js`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/media_object/tests/test_base_models.py` & `solid_backend-0.3a2/solid_backend/media_object/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/message/admin.py` & `solid_backend-0.3a2/solid_backend/message/admin.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/message/migrations/0001_implement_message_model.py` & `solid_backend-0.3a2/solid_backend/message/migrations/0001_implement_message_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/message/migrations/0004_assign_photograph_as_img_field.py` & `solid_backend-0.3a2/solid_backend/message/migrations/0004_assign_photograph_as_img_field.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/message/models.py` & `solid_backend-0.3a2/solid_backend/message/models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/message/tests/test_base_models.py` & `solid_backend-0.3a2/solid_backend/message/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/message/views.py` & `solid_backend-0.3a2/solid_backend/message/views.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/openzoom/deepzoom.py` & `solid_backend-0.3a2/solid_backend/openzoom/deepzoom.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/photograph/admin.py` & `solid_backend-0.3a2/solid_backend/photograph/admin.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/photograph/forms.py` & `solid_backend-0.3a2/solid_backend/photograph/forms.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/photograph/migrations/0001_implement_photograph_model.py` & `solid_backend-0.3a2/solid_backend/photograph/migrations/0001_implement_photograph_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/photograph/migrations/0002_add_audio_fields.py` & `solid_backend-0.3a2/solid_backend/photograph/migrations/0002_add_audio_fields.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/photograph/migrations/0003_create_generic_foreign_key.py` & `solid_backend-0.3a2/solid_backend/photograph/migrations/0003_create_generic_foreign_key.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/photograph/migrations/0004_add_verbose_names.py` & `solid_backend-0.3a2/solid_backend/photograph/migrations/0004_add_verbose_names.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/photograph/migrations/0005_implement_deep_zoom_fields.py` & `solid_backend-0.3a2/solid_backend/photograph/migrations/0005_implement_deep_zoom_fields.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/photograph/models.py` & `solid_backend-0.3a2/solid_backend/photograph/models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/photograph/serializers.py` & `solid_backend-0.3a2/solid_backend/photograph/serializers.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/photograph/tests/test_base_models.py` & `solid_backend-0.3a2/solid_backend/photograph/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/admin.py` & `solid_backend-0.3a2/solid_backend/quiz/admin.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/forms.py` & `solid_backend-0.3a2/solid_backend/quiz/forms.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/migrations/0001_implement_quiz_question_model.py` & `solid_backend-0.3a2/solid_backend/quiz/migrations/0001_implement_quiz_question_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/migrations/0002_implement_quiz_answer_model.py` & `solid_backend-0.3a2/solid_backend/quiz/migrations/0002_implement_quiz_answer_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/migrations/0003_add_verbose_name_to_text_fields.py` & `solid_backend-0.3a2/solid_backend/quiz/migrations/0003_add_verbose_name_to_text_fields.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/migrations/0004_assign_photograph_as_img_field.py` & `solid_backend-0.3a2/solid_backend/quiz/migrations/0004_assign_photograph_as_img_field.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/migrations/0005_auto_20220222_1829.py` & `solid_backend-0.3a2/solid_backend/quiz/migrations/0005_auto_20220222_1829.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/migrations/0006_auto_20220308_1744.py` & `solid_backend-0.3a2/solid_backend/quiz/migrations/0006_auto_20220308_1744.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/migrations/0008_quizquestion_new_tags.py` & `solid_backend-0.3a2/solid_backend/quiz/migrations/0008_quizquestion_new_tags.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/models.py` & `solid_backend-0.3a2/solid_backend/quiz/models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/serializers.py` & `solid_backend-0.3a2/solid_backend/quiz/serializers.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/static/quiz/js/hide_columns.js` & `solid_backend-0.3a2/solid_backend/quiz/static/quiz/js/hide_columns.js`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/tests/test_base_models.py` & `solid_backend-0.3a2/solid_backend/quiz/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/quiz/views.py` & `solid_backend-0.3a2/solid_backend/quiz/views.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/admin.py` & `solid_backend-0.3a2/solid_backend/slideshow/admin.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/forms.py` & `solid_backend-0.3a2/solid_backend/slideshow/forms.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/migrations/0001_implement_slideshow_model.py` & `solid_backend-0.3a2/solid_backend/slideshow/migrations/0001_implement_slideshow_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/migrations/0002_implement_slideshow_page_model.py` & `solid_backend-0.3a2/solid_backend/slideshow/migrations/0002_implement_slideshow_page_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/migrations/0003_implement_slideshow_image_model.py` & `solid_backend-0.3a2/solid_backend/slideshow/migrations/0003_implement_slideshow_image_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/migrations/0004_add_verbose_name_to_text_fields.py` & `solid_backend-0.3a2/solid_backend/slideshow/migrations/0004_add_verbose_name_to_text_fields.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/migrations/0005_add_img_fields_slideshow_model.py` & `solid_backend-0.3a2/solid_backend/slideshow/migrations/0005_add_img_fields_slideshow_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/migrations/0006_assign_photograph_as_img_field_slideshow_model.py` & `solid_backend-0.3a2/solid_backend/slideshow/migrations/0006_assign_photograph_as_img_field_slideshow_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/migrations/0007_assign_photograph_as_img_field_slideshow_image_model.py` & `solid_backend-0.3a2/solid_backend/slideshow/migrations/0007_assign_photograph_as_img_field_slideshow_image_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/migrations/0008_add_active_and_position_field_slideshow_model.py` & `solid_backend-0.3a2/solid_backend/slideshow/migrations/0008_add_active_and_position_field_slideshow_model.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/migrations/0009_remove_default_from_position_fields.py` & `solid_backend-0.3a2/solid_backend/slideshow/migrations/0009_remove_default_from_position_fields.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/migrations/0012_add_taggit_tags.py` & `solid_backend-0.3a2/solid_backend/slideshow/migrations/0012_add_taggit_tags.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/models.py` & `solid_backend-0.3a2/solid_backend/slideshow/models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/serializers.py` & `solid_backend-0.3a2/solid_backend/slideshow/serializers.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/tests/test_base_models.py` & `solid_backend-0.3a2/solid_backend/slideshow/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/slideshow/views.py` & `solid_backend-0.3a2/solid_backend/slideshow/views.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/solid_backend/urls.py` & `solid_backend-0.3a2/solid_backend/urls.py`

 * *Files identical despite different names*

### Comparing `solid_backend-0.3.5/setup.py` & `solid_backend-0.3a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,23 +46,23 @@
 
 install_requires = \
 ['django-cleanup==4.0.0',
  'django-filter>=21.1,<22.0',
  'django-mptt==0.11.0',
  'django-stdimage>=5.1.1,<6.0.0',
  'django-taggit>=1.5.1,<2.0.0',
- 'django>=3.0.7,<4.0.0',
+ 'django>=3.0.7,<3.1.0',
  'djangorestframework==3.11.0',
  'mutagen>=1.44.0,<2.0.0',
  'pillow==7.1.2',
  'psycopg2-binary>=2.8.5,<3.0.0']
 
 setup_kwargs = {
     'name': 'solid-backend',
-    'version': '0.3.5',
+    'version': '0.3a2',
     'description': 'Clean Django app for e-learning application with...',
     'long_description': '# S.O.L.I.D.-Backend\n\n<p align="center">\n<a href="https://codecov.io/gh/zentrumnawi/solid-backend">\n  <img src="https://codecov.io/gh/zentrumnawi/solid-backend/branch/master/graph/badge.svg" /> \n</a>\n<a href="https://travis-ci.com/zentrumnawi/solid-backend"> \n  <img src="https://travis-ci.com/zentrumnawi/solid-backend.svg?branch=master">\n</a>\n<a href="https://github.com/ambv/black">\n  <img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">\n</a>\n</p>\n\n## What is S.O.L.I.D.?\nThe project\'s name is an acronym for **S**ystematic **O**bject-**L**earning and **I**dentification, \nwhich is the purpose of this pluggable django app. It is here to provide a solid (hehe - :D) foundation for future eLearning apps.\nDuring the creation of two eLearning apps at Goethe University Frankfurt we figured out that a lot of disciplines require students to learn how to systematically analyse and classify certain objects. Those objects might be hand-samples of minerals, stones, stuffed animals, paintings or plants, mostly stored in archives with limited access - or none at all. To prevent us from repeating all steps in the creation of a back- and frontend, we focused on the question "Which components will all these apps have in common?" and this package is what we came up with.\nIn order to tackle the problem of limited access to hand-samples, we need to store and process high-definition images with the capability of a zoom feature to deliver HD images on any kind of device. Furthermore, we need a way to arrange the hand-samples in a structured way to provide the core feature. But that\'s not it. eLearning does not solely consist of content distribution. So we also thought of a glossary which the students have at hand without the need to refer to the lecture notes. Another module to display miscellaneous content is the slideshow feature which dombines text and image on separate pages.\nBeyond that, we implemented a quiz in order to give students the opportunity to evaluate their current level of understanding. To top it off, we figured it might be useful to display messages to communicate with our users. Messages can inform about updates, events in the context of a lecture, provide fun facts or make up an advent calender with daily tasks or puzzles. A contact form implementation provides a communication in the other direction.\n\nSo what does S.O.L.I.D provide in short:\n\n- A generic way to set up database models which can be structured in a hierarchical tree.\n- A simple way to store high-definition images which provides automatic creation of DZI-files for the usage of [OpenSeadragon](https://openseadragon.github.io/)\n- A Quiz-system with a variety of Question types.\n- A Glossary to provide subject-specific terminology.\n- A Message system which can be utilized in various ways.\n- A Slideshow system to provide content in a presentation style.\n- A Feedback form to facilitate bug reports and questions.\nSo if you are looking to build the backend of an eLearning app, you came to the right place.\nFor inspiration or just to see what it looks like to use `solid-backend` in the end have a look at [geomat-backend]()and/or [dive-backend]().\nIf you are also interested in the Frontend: We also have an Angular package which can be found [here]() and which is the foundation of the corresponding apps under geomat.uni-frankfurt.de and dive.uni-frankfurt.de\n\n\n## Get started\nRequirements for this package are:\n* Django >3.0.0\n* Djangorestframework 3.11.0\n* django-mptt 0.11.0\n* pillow 7.1.2\n* django-cleanup 4.0.0\n* psycopg2-binary 2.8.5\n* django-taggit 1.5.1\n\nPsycopg2 is important because we are using PostgreSQL specific databasefields. This means that\nyou are also required to use a PostgreSQL database.\n\n### Installation\n\nThe solid-backend package is distributed via PyPi so you can simply install it via\n\t\n\tpip install solid-backend\n\t\nAdd the apps to your `INSTALLED_APPS` for a bare minimum functionality\n\t\n\tsettings.py\n\t\n\tINSTALLED_APPS = [\n    ...,\n    "solid_backend.content",\n    "solid_backend.photograph",\n]\n\nor all apps\n\t\n\tsettings.py\n\t\n\tINSTALLED_APPS = [\n\t\t"solid_backend.contact",\n\t\t"solid_backend.content",\n\t\t"solid_backend.glossary",\n\t\t"solid_backend.message",\n\t\t"solid_backend.quiz",\n\t\t"solid_backend.slideshow",\n\t\t"solid_backend.photograph",\n\t]\n\nAfterwards, don\'t forget to add the url\'s to your url-config.\nHere, again, you can either decide which urls to include or include all of them:\n\nSpecific urls:\n\n\turls.py\n\t\n\turlpatterns = [\n\t\t...,\n\t\turl(r"", include("solid_backend.content.urls"), name="content"),\n\t\turl(r"", include("solid_backend.message.urls"), name="message"),\n\t\turl(r"", include("solid_backend.photograph.urls"), name="photograph"),\n\t\n\t]\n\nAll urls:\n\n\t\turls.py\n\t\n\turlpatterns = [\n\t\t...,\n\t\turl("", include("solid_backend.urls")),\n\t\t\n\t]\n\t\nAfter this you are ready to run the migrations and you are good to go.\n\n\n\n## Documentation\n\nDocumentation is available [here](https://app.gitbook.com/@zentrumnawi/s/dive/).\nThe Documentation is currently only available in german. If you are a non-german speaker\nand want to know more about something feel free to contact us directly via mail and we \nwill figure it out.\n\n## Coverage\n\nComing soon...\n\n## Try it out and local development\n\nFor a How-To guide see the README in the sample_project directory.\n\n',
     'author': 'Christian Grossmüller',
     'author_email': 'chgad.games@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/zentrumnawi/solid-backend',
```

#### html2text {}

```diff
@@ -17,18 +17,18 @@
 'solid_backend.quiz.tests.conftest_files', 'solid_backend.slideshow',
 'solid_backend.slideshow.migrations', 'solid_backend.slideshow.tests',
 'solid_backend.slideshow.tests.conftest_files', 'solid_backend.utils']
 package_data = \ {'': ['*'], 'solid_backend.media_object': ['static/
 media_object/css/*', 'static/media_object/js/*'], 'solid_backend.quiz':
 ['static/quiz/js/*']} install_requires = \ ['django-cleanup==4.0.0', 'django-
 filter>=21.1,<22.0', 'django-mptt==0.11.0', 'django-stdimage>=5.1.1,<6.0.0',
-'django-taggit>=1.5.1,<2.0.0', 'django>=3.0.7,<4.0.0',
+'django-taggit>=1.5.1,<2.0.0', 'django>=3.0.7,<3.1.0',
 'djangorestframework==3.11.0', 'mutagen>=1.44.0,<2.0.0', 'pillow==7.1.2',
 'psycopg2-binary>=2.8.5,<3.0.0'] setup_kwargs = { 'name': 'solid-backend',
-'version': '0.3.5', 'description': 'Clean Django app for e-learning application
+'version': '0.3a2', 'description': 'Clean Django app for e-learning application
 with...', 'long_description': '# S.O.L.I.D.-Backend\n\n
   \n\n_[https://codecov.io/gh/zentrumnawi/solid-backend/branch/master/graph/
           badge.svg]_\n\n\n_[https://travis-ci.com/zentrumnawi/solid-
            backend.svg?branch=master]\n\n\n_[Code_style:_black]\n\n
 \n\n## What is S.O.L.I.D.?\nThe project\'s name is an acronym for
 **S**ystematic **O**bject-**L**earning and **I**dentification, \nwhich is the
 purpose of this pluggable django app. It is here to provide a solid (hehe - :D)
```

### Comparing `solid_backend-0.3.5/PKG-INFO` & `solid_backend-0.3a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: solid-backend
-Version: 0.3.5
+Version: 0.3a2
 Summary: Clean Django app for e-learning application with...
 Home-page: https://github.com/zentrumnawi/solid-backend
 License: MIT
 Author: Christian Grossmüller
 Author-email: chgad.games@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django (>=3.0.7,<4.0.0)
+Requires-Dist: django (>=3.0.7,<3.1.0)
 Requires-Dist: django-cleanup (==4.0.0)
 Requires-Dist: django-filter (>=21.1,<22.0)
 Requires-Dist: django-mptt (==0.11.0)
 Requires-Dist: django-stdimage (>=5.1.1,<6.0.0)
 Requires-Dist: django-taggit (>=1.5.1,<2.0.0)
 Requires-Dist: djangorestframework (==3.11.0)
 Requires-Dist: mutagen (>=1.44.0,<2.0.0)
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: solid-backend Version: 0.3.5 Summary: Clean Django
+Metadata-Version: 2.1 Name: solid-backend Version: 0.3a2 Summary: Clean Django
 app for e-learning application with... Home-page: https://github.com/
 zentrumnawi/solid-backend License: MIT Author: Christian GrossmÃ¼ller Author-
 email: chgad.games@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: django (>=3.0.7,<4.0.0) Requires-
+Language :: Python :: 3.11 Requires-Dist: django (>=3.0.7,<3.1.0) Requires-
 Dist: django-cleanup (==4.0.0) Requires-Dist: django-filter (>=21.1,<22.0)
 Requires-Dist: django-mptt (==0.11.0) Requires-Dist: django-stdimage
 (>=5.1.1,<6.0.0) Requires-Dist: django-taggit (>=1.5.1,<2.0.0) Requires-Dist:
 djangorestframework (==3.11.0) Requires-Dist: mutagen (>=1.44.0,<2.0.0)
 Requires-Dist: pillow (==7.1.2) Requires-Dist: psycopg2-binary (>=2.8.5,<3.0.0)
 Project-URL: Repository, https://github.com/zentrumnawi/solid-backend
 Description-Content-Type: text/markdown # S.O.L.I.D.-Backend
```


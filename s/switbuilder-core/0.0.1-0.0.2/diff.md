# Comparing `tmp/switbuilder_core-0.0.1.tar.gz` & `tmp/switbuilder_core-0.0.2.tar.gz`

## Comparing `switbuilder_core-0.0.1.tar` & `switbuilder_core-0.0.2.tar`

### file list

```diff
@@ -1,62 +1,151 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/.DS_Store
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/.idea/core.iml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/__init__.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/collection_entry/Background.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/collection_entry/CollectionEntry.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/collection_entry/MetadataItem.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/collection_entry/StartSection.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/collection_entry/TextContent.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/collection_entry/TextSection.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/collection_entry/TextStyle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/collection_entry/__init__.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/collection_entry/tests.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/common/Button.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/common/Icon.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/common/StaticAction.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/common/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/divider/Divider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/divider/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/file/File.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/file/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/header/ContextMenuItem.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/header/Header.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/header/__init__.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/header/tests.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/html_frame/HtmlFrame.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/html_frame/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/image/Image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/image/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/input/Input.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/input/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/input/tests.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/select/Option.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/select/Select.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/select/Style.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/select/__init__.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/select/tests.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/signin/IntegratedService.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/signin/SignInPage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/signin/__init__.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/signin/tests.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/swit_response/AttachmentView.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/swit_response/Body.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/swit_response/Container.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/swit_response/Footer.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/swit_response/SwitResponse.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/swit_response/View.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/swit_response/__init__.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/swit_response/tests.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/text_paragraph/TextParagraph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/ui/text_paragraph/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/.gitignore
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/README.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 switbuilder_core-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.DS_Store
+-rwxr-xr-x   0        0        0       47 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/build.sh
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/database.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/core.iml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    21417 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/ActionId.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/__init__.py
+-rw-r--r--   0        0        0    18389 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/activity_handler.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/activity_handler_abc.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/constants.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/dependencies.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/exceptions.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/router.py
+-rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/schemas.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/tests.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/action/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/constants.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/dependencies.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/exception.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/models.py
+-rw-r--r--   0        0        0     5916 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/oauth2.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/repository.py
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/router.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/schemas.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/service.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/auth/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/channel/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/channel/schemas.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/channel/service.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/channel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/conversation/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/conversation/schemas.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/conversation/service.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/conversation/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/emails/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/emails/service.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/emails/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/constants.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/exception.py
+-rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/schemas.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/service.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/__init__.py
+-rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/tests.py
+-rw-r--r--   0        0        0   306291 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/cid_image_email.json
+-rw-r--r--   0        0        0  1499842 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/email_with_attachment.json
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/empty_receiver_email.json
+-rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/html_email.json
+-rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/invalid_swit_image.json
+-rw-r--r--   0        0        0   631221 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/large_cid_image_email.json
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/email/plain_text_email.json
+-rw-r--r--   0        0        0    34901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/html/example1.html
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/html/example2.html
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/html/example3.html
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/imap/tests/html/example4.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/membership/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/membership/schemas.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/membership/service.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/membership/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/project/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/project/schemas.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/project/service.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/project/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/task/__init__.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/task/schemas.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/task/service.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/task/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/__init__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/draw_manager_abc.py
+-rw-r--r--   0        0        0    25930 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/draw_managers.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/service.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/Background.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/CollectionEntry.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/MetadataItem.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/StartSection.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/TextContent.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/TextSection.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/TextStyle.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/__init__.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/collection_entry/tests.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/common/Button.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/common/Icon.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/common/StaticAction.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/common/__init__.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/container/Container.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/container/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/divider/Divider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/divider/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/file/File.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/file/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/header/ContextMenuItem.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/header/Header.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/header/__init__.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/header/tests.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/html_frame/HtmlFrame.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/html_frame/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/image/Image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/image/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/input/Input.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/input/__init__.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/input/tests.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/listitem/ListItem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/listitem/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/select/Option.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/select/Select.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/select/Style.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/select/__init__.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/select/tests.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/signin/IntegratedService.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/signin/SignInPage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/signin/__init__.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/signin/tests.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/AttachmentView.py
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/Body.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/Footer.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/SwitResponse.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/View.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/__init__.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/swit_response/tests.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/text_paragraph/TextParagraph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/text_paragraph/__init__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/textarea/Textarea.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/textarea/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/attach_to_task_modal/__init__.py
+-rw-r--r--   0        0        0     9100 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/attach_to_task_modal/draw_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/convert_to_task_modal/__init__.py
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/convert_to_task_modal/draw_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/need_authorization_modal/__init__.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/need_authorization_modal/draw_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/share_to_dm_modal/__init__.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/ui/view_draw_managers/share_to_dm_modal/draw_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/workspace/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/workspace/schemas.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/workspace/service.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/workspace/utils.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/.gitignore
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/README.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 switbuilder_core-0.0.2/PKG-INFO
```

### Comparing `switbuilder_core-0.0.1/.DS_Store` & `switbuilder_core-0.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `switbuilder_core-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.1/ui/collection_entry/CollectionEntry.py` & `switbuilder_core-0.0.2/ui/collection_entry/CollectionEntry.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.1/ui/collection_entry/tests.py` & `switbuilder_core-0.0.2/ui/collection_entry/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import unittest
 
 from ui.collection_entry.Background import Background
 from ui.collection_entry.CollectionEntry import CollectionEntry
 from ui.collection_entry.MetadataItem import MetadataItem
+from ui.collection_entry.StartSection import StartSection
 from ui.collection_entry.TextContent import TextContent
 from ui.collection_entry.TextSection import TextSection
 from ui.collection_entry.TextStyle import TextStyle
+from ui.common.Button import Button
+from ui.common.Icon import Icon
 from ui.common.StaticAction import StaticAction
+from ui.header.ContextMenuItem import ContextMenuItem
+from ui.header.Header import Header
 
 
 class Test(unittest.TestCase):
     def test_valid_collection_entry(self):
         given = {
             "type": "collection_entry",
             "text_sections": [
```

### Comparing `switbuilder_core-0.0.1/ui/file/File.py` & `switbuilder_core-0.0.2/ui/file/File.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.1/ui/header/tests.py` & `switbuilder_core-0.0.2/ui/header/tests.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.1/ui/select/tests.py` & `switbuilder_core-0.0.2/ui/select/tests.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.1/ui/signin/tests.py` & `switbuilder_core-0.0.2/ui/signin/tests.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.1/ui/swit_response/Body.py` & `switbuilder_core-0.0.2/ui/swit_response/Body.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from typing import Any
 
 from pydantic import BaseModel
 
 from ui.collection_entry.CollectionEntry import CollectionEntry
 from ui.common.Button import Button
+from ui.container.Container import Container
 from ui.divider.Divider import Divider
 from ui.file.File import File
 from ui.html_frame.HtmlFrame import HtmlFrame
 from ui.image.Image import Image
 from ui.input.Input import Input
 from ui.select.Select import Select
 from ui.signin.SignInPage import SignInPage
 from ui.text_paragraph.TextParagraph import TextParagraph
+from ui.textarea.Textarea import Textarea
 
-ElementType = CollectionEntry | Button | Divider | File | HtmlFrame | Input | Select | SignInPage | TextParagraph | Image
+ElementType = CollectionEntry | Button | Divider | File \
+              | HtmlFrame | Input | Select | SignInPage | TextParagraph | Image | Textarea | Container
 
 
 def contain_only_dict(elements_data: list[dict | ElementType]) -> bool:
     for element_data in elements_data:
         if isinstance(element_data, ElementType):
             return False
 
@@ -40,31 +43,35 @@
         return Input
     elif element_type_str == 'select':
         return Select
     elif element_type_str == 'sign_in_page':
         return SignInPage
     elif element_type_str == 'text':
         return TextParagraph
+    elif element_type_str == 'textarea':
+        return Textarea
     elif element_type_str == 'image':
         return Image
+    elif element_type_str == 'container':
+        return Container
     else:
         raise ValueError(f"Unknown element type: {element_type_str}")
 
 
 class Body(BaseModel):
     elements: list[ElementType]
 
     class Config:
         smart_union = True
 
     def __init__(self, **data: Any) -> None:
         elements_data = data.get('elements', [])
 
         if contain_only_dict(elements_data):
-            elements = []
+            _elements: list[ElementType] = []
             for element_data in elements_data:
                 element_type = get_element_type(element_data)
                 element = element_type(**element_data)
-                elements.append(element)
-            super().__init__(elements=elements)
+                _elements.append(element)
+            super().__init__(elements=_elements)
         else:
             super().__init__(**data)
```

### Comparing `switbuilder_core-0.0.1/ui/swit_response/SwitResponse.py` & `switbuilder_core-0.0.2/ui/swit_response/SwitResponse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from enum import Enum
 
 from pydantic import BaseModel
 
+from action.constants import ViewIdTypes
 from ui.swit_response.AttachmentView import AttachmentView
 from ui.swit_response.View import View
 
 
 class ViewCallbackType(str, Enum):
     update = "views.update"
     initialize = "views.initialize"
@@ -28,8 +29,8 @@
     attachments: AttachmentView
 
 
 class SwitResponse(BaseModel):
     callback_type: ViewCallbackType | AttachmentCallbackType
     new_view: View | None
     attachments: AttachmentView | None
-    reference_view_id: str | None
+    reference_view_id: ViewIdTypes | None
```

### Comparing `switbuilder_core-0.0.1/ui/swit_response/tests.py` & `switbuilder_core-0.0.2/ui/swit_response/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 
+from action.constants import ViewIdTypes
 from ui.divider.Divider import Divider
 from ui.header.ContextMenuItem import ContextMenuItem
 from ui.header.Header import Header
 from ui.input.Input import Input
 from ui.swit_response.Body import Body
 from ui.swit_response.SwitResponse import SwitResponse, ViewCallbackType
 from ui.swit_response.View import View
@@ -28,28 +29,28 @@
         )
 
         body = Body(
             elements=[input_]
         )
 
         new_view = View(
-            view_id="right_panel",
+            view_id=ViewIdTypes.right_panel,
             state='',
             header=header,
             body=body
         )
 
         swit_response = SwitResponse(
             callback_type=ViewCallbackType.update,
             new_view=new_view
         )
 
         given = {
             'callback_type': 'views.update',
-            'new_view': {'view_id': "right_panel",
+            'new_view': {'view_id': ViewIdTypes.right_panel,
                          'state': '',
                          'header': {
                              "title": "This is a view title",
                              "subtitle": "Add a subtitle if needed",
                              "context_menu": [
                                  {
                                      "label": "Menu item 1",
```

### Comparing `switbuilder_core-0.0.1/pyproject.toml` & `switbuilder_core-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [project]
 name = "switbuilder-core"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "ur-team", email = "el.lee@swit.io" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'pydantic >= 1.10.9',
+    'httpx >=0.24.1',
+    'fastapi >=0.83.0',
+    'SQLAlchemy >=1.4.41',
+    'PyMySQL >=1.1.0',
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
 [build-system]
```


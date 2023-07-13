# Comparing `tmp/chainfury_server-1.0.1.tar.gz` & `tmp/chainfury_server-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainfury_server-1.0.1.tar", max compression
+gzip compressed data, was "chainfury_server-1.0.2.tar", max compression
```

## Comparing `chainfury_server-1.0.1.tar` & `chainfury_server-1.0.2.tar`

### file list

```diff
@@ -1,148 +1,148 @@
--rw-r--r--   0        0        0      108 2023-07-13 08:11:27.224304 chainfury_server-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-13 10:46:03.554810 chainfury_server-1.0.1/chainfury_server/__init__.py
--rw-r--r--   0        0        0     2899 2023-07-13 08:16:00.850229 chainfury_server-1.0.1/chainfury_server/api/auth.py
--rw-r--r--   0        0        0     5170 2023-07-13 08:16:00.713410 chainfury_server-1.0.1/chainfury_server/api/chatbot.py
--rw-r--r--   0        0        0     2349 2023-07-13 08:16:12.521773 chainfury_server-1.0.1/chainfury_server/api/dashboard.py
--rw-r--r--   0        0        0     1008 2023-07-13 08:16:17.522491 chainfury_server-1.0.1/chainfury_server/api/feedback.py
--rw-r--r--   0        0        0    10713 2023-07-13 08:16:27.917881 chainfury_server-1.0.1/chainfury_server/api/fury.py
--rw-r--r--   0        0        0     1128 2023-07-13 08:16:00.721524 chainfury_server-1.0.1/chainfury_server/api/intermediate_steps.py
--rw-r--r--   0        0        0      385 2023-07-13 08:14:55.569340 chainfury_server-1.0.1/chainfury_server/api/langflow.py
--rw-r--r--   0        0        0     7746 2023-07-13 08:16:48.304010 chainfury_server-1.0.1/chainfury_server/api/metrics.py
--rw-r--r--   0        0        0     5852 2023-07-13 08:20:52.792463 chainfury_server-1.0.1/chainfury_server/api/prompts.py
--rw-r--r--   0        0        0     1948 2023-07-13 08:17:57.465712 chainfury_server-1.0.1/chainfury_server/api/template.py
--rw-r--r--   0        0        0     1376 2023-07-13 08:18:08.982573 chainfury_server-1.0.1/chainfury_server/api/user.py
--rw-r--r--   0        0        0     3415 2023-07-13 10:46:56.419360 chainfury_server-1.0.1/chainfury_server/app.py
--rw-r--r--   0        0        0        0 2023-06-12 14:13:15.390604 chainfury_server-1.0.1/chainfury_server/commons/__init__.py
--rw-r--r--   0        0        0     1413 2023-06-12 14:13:15.390926 chainfury_server-1.0.1/chainfury_server/commons/config.py
--rw-r--r--   0        0        0        0 2023-06-12 14:13:15.391011 chainfury_server-1.0.1/chainfury_server/commons/constants.py
--rw-r--r--   0        0        0     7563 2023-07-13 08:18:45.219487 chainfury_server-1.0.1/chainfury_server/commons/fury_utils.py
--rw-r--r--   0        0        0     2944 2023-07-13 08:18:50.515872 chainfury_server-1.0.1/chainfury_server/commons/gpt_rating.py
--rw-r--r--   0        0        0     5205 2023-07-13 08:19:02.364524 chainfury_server-1.0.1/chainfury_server/commons/langflow_utils.py
--rw-r--r--   0        0        0        0 2023-06-12 14:13:15.391843 chainfury_server-1.0.1/chainfury_server/commons/metrics_utils.py
--rw-r--r--   0        0        0      563 2023-07-13 08:19:08.628139 chainfury_server-1.0.1/chainfury_server/commons/types.py
--rw-r--r--   0        0        0     9937 2023-07-13 10:42:38.175235 chainfury_server-1.0.1/chainfury_server/commons/utils.py
--rw-r--r--   0        0        0     8224 2023-07-13 08:22:11.384119 chainfury_server-1.0.1/chainfury_server/database.py
--rw-r--r--   0        0        0      606 2023-06-12 14:13:15.394729 chainfury_server-1.0.1/chainfury_server/database_constants.py
--rw-r--r--   0        0        0        0 2023-06-12 14:13:15.394837 chainfury_server-1.0.1/chainfury_server/database_utils/__init__.py
--rw-r--r--   0        0        0      412 2023-07-13 08:15:47.541666 chainfury_server-1.0.1/chainfury_server/database_utils/chatbot.py
--rw-r--r--   0        0        0     1141 2023-07-13 08:19:55.464141 chainfury_server-1.0.1/chainfury_server/database_utils/dashboard.py
--rw-r--r--   0        0        0      458 2023-06-12 14:13:15.395389 chainfury_server-1.0.1/chainfury_server/database_utils/general_utils.py
--rw-r--r--   0        0        0     1212 2023-07-13 08:15:47.461948 chainfury_server-1.0.1/chainfury_server/database_utils/intermediate_step.py
--rw-r--r--   0        0        0      808 2023-07-13 08:15:47.436610 chainfury_server-1.0.1/chainfury_server/database_utils/prompt.py
--rw-r--r--   0        0        0    20833 2023-06-12 14:13:15.396257 chainfury_server-1.0.1/chainfury_server/examples/basic_template.json
--rw-r--r--   0        0        0    11731 2023-07-04 11:08:52.449936 chainfury_server-1.0.1/chainfury_server/examples/chuck_norris.json
--rw-r--r--   0        0        0      713 2023-07-04 11:15:32.708753 chainfury_server-1.0.1/chainfury_server/examples/index.json
--rw-r--r--   0        0        0     8830 2023-07-04 11:10:59.210504 chainfury_server-1.0.1/chainfury_server/examples/serper_summarizer.json
--rw-r--r--   0        0        0      485 2023-06-12 14:13:15.398098 chainfury_server-1.0.1/chainfury_server/plugins/README.md
--rw-r--r--   0        0        0      208 2023-07-13 08:20:52.728195 chainfury_server-1.0.1/chainfury_server/plugins/__init__.py
--rw-r--r--   0        0        0     1317 2023-07-13 08:21:05.999858 chainfury_server-1.0.1/chainfury_server/plugins/base.py
--rw-r--r--   0        0        0     1105 2023-07-13 08:20:28.446116 chainfury_server-1.0.1/chainfury_server/plugins/echo/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-13 08:22:39.591789 chainfury_server-1.0.1/chainfury_server/plugins/handler.py
--rw-r--r--   0        0        0     1352 2023-07-13 08:20:28.423757 chainfury_server-1.0.1/chainfury_server/plugins/loader.py
--rw-r--r--   0        0        0      370 2023-06-12 14:13:15.398994 chainfury_server-1.0.1/chainfury_server/plugins/nbx/README.md
--rw-r--r--   0        0        0     1212 2023-07-13 08:20:52.750165 chainfury_server-1.0.1/chainfury_server/plugins/nbx/__init__.py
--rw-r--r--   0        0        0     1871 2023-07-13 08:20:52.760557 chainfury_server-1.0.1/chainfury_server/plugins/nbx/lmao.py
--rw-r--r--   0        0        0       93 2023-07-13 08:14:55.626096 chainfury_server-1.0.1/chainfury_server/plugins/nbx/utils.py
--rw-r--r--   0        0        0        0 2023-06-12 14:13:15.399497 chainfury_server-1.0.1/chainfury_server/schemas/__init__.py
--rw-r--r--   0        0        0      156 2023-06-12 14:13:15.399643 chainfury_server-1.0.1/chainfury_server/schemas/prompt_schema.py
--rw-r--r--   0        0        0      456 2023-07-13 08:22:45.858540 chainfury_server-1.0.1/chainfury_server/server.py
--rw-r--r--   0        0        0     6952 2023-04-26 06:34:46.433694 chainfury_server-1.0.1/chainfury_server/static/assets/Button-3149f941.js
--rw-r--r--   0        0        0     6950 2023-06-20 13:47:53.255568 chainfury_server-1.0.1/chainfury_server/static/assets/Button-593e2495.js
--rw-r--r--   0        0        0     6950 2023-06-26 08:19:02.031165 chainfury_server-1.0.1/chainfury_server/static/assets/Button-59c8a701.js
--rw-r--r--   0        0        0     6950 2023-07-04 11:30:32.013065 chainfury_server-1.0.1/chainfury_server/static/assets/Button-5a4b534a.js
--rw-r--r--   0        0        0     6950 2023-07-04 09:13:31.914124 chainfury_server-1.0.1/chainfury_server/static/assets/Button-c4b2e4dc.js
--rw-r--r--   0        0        0     6950 2023-06-27 12:22:20.870023 chainfury_server-1.0.1/chainfury_server/static/assets/Button-ee88713e.js
--rw-r--r--   0        0        0     6950 2023-07-04 04:41:08.275824 chainfury_server-1.0.1/chainfury_server/static/assets/Button-f8e4aa7f.js
--rw-r--r--   0        0        0     5407 2023-06-27 12:22:20.870133 chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-038cacf7.js
--rw-r--r--   0        0        0     5407 2023-06-20 13:47:53.258435 chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-25bd7bfc.js
--rw-r--r--   0        0        0     2919 2023-04-26 06:34:46.440206 chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-2f5c1012.js
--rw-r--r--   0        0        0     5407 2023-07-04 04:41:08.277845 chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-8d7894f9.js
--rw-r--r--   0        0        0     5402 2023-07-04 11:30:32.014151 chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-c5140795.js
--rw-r--r--   0        0        0     5407 2023-06-26 08:19:02.033268 chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-e4d4f5c0.js
--rw-r--r--   0        0        0     5407 2023-07-04 09:13:31.913993 chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-f3bf7953.js
--rw-r--r--   0        0        0    18349 2023-06-20 13:47:53.255828 chainfury_server-1.0.1/chainfury_server/static/assets/Close-28cfcc9d.js
--rw-r--r--   0        0        0    19251 2023-06-26 08:19:02.031757 chainfury_server-1.0.1/chainfury_server/static/assets/Close-52ca7490.js
--rw-r--r--   0        0        0    19251 2023-07-04 11:30:32.012073 chainfury_server-1.0.1/chainfury_server/static/assets/Close-59b68972.js
--rw-r--r--   0        0        0    19251 2023-07-04 04:41:08.277104 chainfury_server-1.0.1/chainfury_server/static/assets/Close-bdf112d1.js
--rw-r--r--   0        0        0    18321 2023-04-26 06:34:46.437970 chainfury_server-1.0.1/chainfury_server/static/assets/Close-d0ff1fdc.js
--rw-r--r--   0        0        0    19251 2023-06-27 12:22:20.870447 chainfury_server-1.0.1/chainfury_server/static/assets/Close-f05ea766.js
--rw-r--r--   0        0        0    19251 2023-07-04 09:13:31.914267 chainfury_server-1.0.1/chainfury_server/static/assets/Close-fc534dca.js
--rw-r--r--   0        0        0    58829 2023-07-04 04:41:08.277257 chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-17acb7b6.js
--rw-r--r--   0        0        0    58829 2023-07-04 09:13:31.912632 chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-8b686744.js
--rw-r--r--   0        0        0    58731 2023-06-27 12:22:20.869602 chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-a27fa07d.js
--rw-r--r--   0        0        0    10668 2023-04-26 06:34:46.436365 chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-a4b113e7.js
--rw-r--r--   0        0        0    58731 2023-06-26 08:19:02.033392 chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-a5c783f7.js
--rw-r--r--   0        0        0    58772 2023-06-20 13:47:53.257644 chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-c9de222f.js
--rw-r--r--   0        0        0    58888 2023-07-04 11:30:32.013834 chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-e4a49fcb.js
--rw-r--r--   0        0        0      992 2023-06-20 13:47:53.258177 chainfury_server-1.0.1/chainfury_server/static/assets/dispatchHooks-562c67db.js
--rw-r--r--   0        0        0      993 2023-04-26 06:34:46.435878 chainfury_server-1.0.1/chainfury_server/static/assets/dispatchHooks-85107758.js
--rw-r--r--   0        0        0      444 2023-04-26 06:34:46.437506 chainfury_server-1.0.1/chainfury_server/static/assets/index-0223be06.js
--rw-r--r--   0        0        0     2255 2023-07-04 11:30:32.012657 chainfury_server-1.0.1/chainfury_server/static/assets/index-10efa1c9.js
--rw-r--r--   0        0        0   341822 2023-06-27 12:22:20.870295 chainfury_server-1.0.1/chainfury_server/static/assets/index-1c76e43d.js
--rw-r--r--   0        0        0     2037 2023-06-27 12:22:20.868410 chainfury_server-1.0.1/chainfury_server/static/assets/index-233b7bec.js
--rw-r--r--   0        0        0   339600 2023-04-26 06:34:46.434837 chainfury_server-1.0.1/chainfury_server/static/assets/index-35325410.js
--rw-r--r--   0        0        0     2091 2023-06-26 08:19:02.032455 chainfury_server-1.0.1/chainfury_server/static/assets/index-36d17591.js
--rw-r--r--   0        0        0    25908 2023-04-26 06:34:46.439241 chainfury_server-1.0.1/chainfury_server/static/assets/index-3f4aa8cc.css
--rw-r--r--   0        0        0  1119873 2023-07-04 11:30:32.014476 chainfury_server-1.0.1/chainfury_server/static/assets/index-4e19540d.js
--rw-r--r--   0        0        0     2200 2023-07-04 04:41:08.276228 chainfury_server-1.0.1/chainfury_server/static/assets/index-5176fb7e.js
--rw-r--r--   0        0        0  1119872 2023-06-27 12:22:20.869286 chainfury_server-1.0.1/chainfury_server/static/assets/index-529e483a.js
--rw-r--r--   0        0        0     2037 2023-06-26 08:19:02.032235 chainfury_server-1.0.1/chainfury_server/static/assets/index-547b311b.js
--rw-r--r--   0        0        0   341944 2023-07-04 09:13:31.913856 chainfury_server-1.0.1/chainfury_server/static/assets/index-5582c958.js
--rw-r--r--   0        0        0   342086 2023-07-04 11:30:32.013270 chainfury_server-1.0.1/chainfury_server/static/assets/index-55f22566.js
--rw-r--r--   0        0        0     6883 2023-07-04 11:30:32.012873 chainfury_server-1.0.1/chainfury_server/static/assets/index-57a158a9.css
--rw-r--r--   0        0        0   228645 2023-06-26 08:19:02.031954 chainfury_server-1.0.1/chainfury_server/static/assets/index-5b6bc100.js
--rw-r--r--   0        0        0     2112 2023-04-26 06:34:46.439610 chainfury_server-1.0.1/chainfury_server/static/assets/index-5cfeeef6.js
--rw-r--r--   0        0        0    27870 2023-07-04 11:30:32.013418 chainfury_server-1.0.1/chainfury_server/static/assets/index-628511b6.css
--rw-r--r--   0        0        0    27779 2023-07-04 04:41:08.276388 chainfury_server-1.0.1/chainfury_server/static/assets/index-68ec8b36.css
--rw-r--r--   0        0        0   341736 2023-06-26 08:19:02.033593 chainfury_server-1.0.1/chainfury_server/static/assets/index-6ac8ab06.js
--rw-r--r--   0        0        0   341944 2023-07-04 04:41:08.276043 chainfury_server-1.0.1/chainfury_server/static/assets/index-7221a78d.js
--rw-r--r--   0        0        0   234892 2023-07-04 11:30:32.014978 chainfury_server-1.0.1/chainfury_server/static/assets/index-75500326.js
--rw-r--r--   0        0        0   231540 2023-07-04 04:41:08.276672 chainfury_server-1.0.1/chainfury_server/static/assets/index-7d6e7c9a.js
--rw-r--r--   0        0        0     2091 2023-06-27 12:22:20.869897 chainfury_server-1.0.1/chainfury_server/static/assets/index-81f0ebfb.js
--rw-r--r--   0        0        0     2091 2023-06-20 13:47:53.254937 chainfury_server-1.0.1/chainfury_server/static/assets/index-9084c7e8.js
--rw-r--r--   0        0        0     2091 2023-07-04 04:41:08.276802 chainfury_server-1.0.1/chainfury_server/static/assets/index-9546d633.js
--rw-r--r--   0        0        0  1119359 2023-04-26 06:34:46.441000 chainfury_server-1.0.1/chainfury_server/static/assets/index-9b6b9c14.js
--rw-r--r--   0        0        0   220504 2023-04-26 06:34:46.434201 chainfury_server-1.0.1/chainfury_server/static/assets/index-9da9e357.js
--rw-r--r--   0        0        0  1119872 2023-07-04 04:41:08.277699 chainfury_server-1.0.1/chainfury_server/static/assets/index-9fd47f49.js
--rw-r--r--   0        0        0  1119872 2023-06-26 08:19:02.032799 chainfury_server-1.0.1/chainfury_server/static/assets/index-a077d00c.js
--rw-r--r--   0        0        0  1119872 2023-07-04 09:13:31.912994 chainfury_server-1.0.1/chainfury_server/static/assets/index-a6ad3f72.js
--rw-r--r--   0        0        0   230102 2023-06-27 12:22:20.869763 chainfury_server-1.0.1/chainfury_server/static/assets/index-a8a84317.js
--rw-r--r--   0        0        0     2037 2023-06-20 13:47:53.257911 chainfury_server-1.0.1/chainfury_server/static/assets/index-b4463069.js
--rw-r--r--   0        0        0   234897 2023-07-04 09:13:31.914655 chainfury_server-1.0.1/chainfury_server/static/assets/index-b5b9763d.js
--rw-r--r--   0        0        0  1119913 2023-06-20 13:47:53.257014 chainfury_server-1.0.1/chainfury_server/static/assets/index-b6e3039e.js
--rw-r--r--   0        0        0     2037 2023-07-04 04:41:08.276950 chainfury_server-1.0.1/chainfury_server/static/assets/index-b9992484.js
--rw-r--r--   0        0        0     2091 2023-07-04 11:30:32.014820 chainfury_server-1.0.1/chainfury_server/static/assets/index-c066588b.js
--rw-r--r--   0        0        0     2037 2023-07-04 09:13:31.913444 chainfury_server-1.0.1/chainfury_server/static/assets/index-c1411de8.js
--rw-r--r--   0        0        0   341798 2023-06-20 13:47:53.254640 chainfury_server-1.0.1/chainfury_server/static/assets/index-d4346eec.js
--rw-r--r--   0        0        0      947 2023-06-27 12:22:20.868643 chainfury_server-1.0.1/chainfury_server/static/assets/index-e156bd3d.js
--rw-r--r--   0        0        0     2171 2023-04-26 06:34:46.439914 chainfury_server-1.0.1/chainfury_server/static/assets/index-eb6972f0.js
--rw-r--r--   0        0        0   226087 2023-06-20 13:47:53.255267 chainfury_server-1.0.1/chainfury_server/static/assets/index-eed7f1d2.js
--rw-r--r--   0        0        0     2091 2023-07-04 09:13:31.914385 chainfury_server-1.0.1/chainfury_server/static/assets/index-f1d79a0e.js
--rw-r--r--   0        0        0     2037 2023-07-04 11:30:32.013973 chainfury_server-1.0.1/chainfury_server/static/assets/index-ff44d1cd.js
--rw-r--r--   0        0        0    27472 2023-06-20 13:47:53.256371 chainfury_server-1.0.1/chainfury_server/static/assets/index-ffbb8444.css
--rw-r--r--   0        0        0       73 2023-06-20 13:47:53.257367 chainfury_server-1.0.1/chainfury_server/static/assets/store-06cc0006.js
--rw-r--r--   0        0        0       73 2023-06-27 12:22:20.868532 chainfury_server-1.0.1/chainfury_server/static/assets/store-71291eee.js
--rw-r--r--   0        0        0       73 2023-06-26 08:19:02.031026 chainfury_server-1.0.1/chainfury_server/static/assets/store-b83ff62b.js
--rw-r--r--   0        0        0       73 2023-07-04 11:30:32.011921 chainfury_server-1.0.1/chainfury_server/static/assets/store-c9993eae.js
--rw-r--r--   0        0        0       73 2023-07-04 04:41:08.277395 chainfury_server-1.0.1/chainfury_server/static/assets/store-ce236640.js
--rw-r--r--   0        0        0       73 2023-04-26 06:34:46.436918 chainfury_server-1.0.1/chainfury_server/static/assets/store-d6cbae01.js
--rw-r--r--   0        0        0       73 2023-07-04 09:13:31.913674 chainfury_server-1.0.1/chainfury_server/static/assets/store-e09eb698.js
--rw-r--r--   0        0        0      227 2023-06-20 13:47:53.256092 chainfury_server-1.0.1/chainfury_server/static/assets/useControlled-00f12b58.js
--rw-r--r--   0        0        0      227 2023-06-27 12:22:20.868778 chainfury_server-1.0.1/chainfury_server/static/assets/useControlled-1019e2b5.js
--rw-r--r--   0        0        0      227 2023-06-26 08:19:02.033123 chainfury_server-1.0.1/chainfury_server/static/assets/useControlled-143349eb.js
--rw-r--r--   0        0        0      227 2023-07-04 04:41:08.276517 chainfury_server-1.0.1/chainfury_server/static/assets/useControlled-360d1c06.js
--rw-r--r--   0        0        0      227 2023-07-04 09:13:31.914502 chainfury_server-1.0.1/chainfury_server/static/assets/useControlled-63c4605a.js
--rw-r--r--   0        0        0      227 2023-07-04 11:30:32.013675 chainfury_server-1.0.1/chainfury_server/static/assets/useControlled-6a808db7.js
--rw-r--r--   0        0        0    77380 2023-07-04 11:30:32.011345 chainfury_server-1.0.1/chainfury_server/static/chainfury.png
--rw-r--r--   0        0        0      454 2023-07-04 11:30:32.010881 chainfury_server-1.0.1/chainfury_server/static/index.html
--rw-r--r--   0        0        0     2138 2023-07-04 11:30:32.011633 chainfury_server-1.0.1/chainfury_server/static/script/embedBot.js
--rw-r--r--   0        0        0     1497 2023-04-26 06:34:46.432782 chainfury_server-1.0.1/chainfury_server/static/vite.svg
--rw-r--r--   0        0        0        0 2023-06-12 14:13:15.400002 chainfury_server-1.0.1/chainfury_server/stories/__init__.py
--rw-r--r--   0        0        0    10578 2023-06-26 12:43:39.055327 chainfury_server-1.0.1/chainfury_server/stories/api.py
--rw-r--r--   0        0        0    15135 2023-06-12 14:13:15.400726 chainfury_server-1.0.1/chainfury_server/stories/dag.json
--rw-r--r--   0        0        0      101 2023-07-13 08:20:52.793186 chainfury_server-1.0.1/chainfury_server/stories/plugins.py
--rw-r--r--   0        0        0      454 2023-07-04 11:30:32.020977 chainfury_server-1.0.1/chainfury_server/templates/index.html
--rw-r--r--   0        0        0      135 2023-07-13 11:22:06.514553 chainfury_server-1.0.1/chainfury_server/version.py
--rw-r--r--   0        0        0      713 2023-07-13 11:22:06.509672 chainfury_server-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1493 1970-01-01 00:00:00.000000 chainfury_server-1.0.1/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 chainfury_server-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      108 2023-07-13 08:11:27.224304 chainfury_server-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 10:46:03.554810 chainfury_server-1.0.2/chainfury_server/__init__.py
+-rw-r--r--   0        0        0     2899 2023-07-13 08:16:00.850229 chainfury_server-1.0.2/chainfury_server/api/auth.py
+-rw-r--r--   0        0        0     5170 2023-07-13 08:16:00.713410 chainfury_server-1.0.2/chainfury_server/api/chatbot.py
+-rw-r--r--   0        0        0     2349 2023-07-13 08:16:12.521773 chainfury_server-1.0.2/chainfury_server/api/dashboard.py
+-rw-r--r--   0        0        0     1008 2023-07-13 08:16:17.522491 chainfury_server-1.0.2/chainfury_server/api/feedback.py
+-rw-r--r--   0        0        0    10713 2023-07-13 08:16:27.917881 chainfury_server-1.0.2/chainfury_server/api/fury.py
+-rw-r--r--   0        0        0     1128 2023-07-13 08:16:00.721524 chainfury_server-1.0.2/chainfury_server/api/intermediate_steps.py
+-rw-r--r--   0        0        0      385 2023-07-13 08:14:55.569340 chainfury_server-1.0.2/chainfury_server/api/langflow.py
+-rw-r--r--   0        0        0     7746 2023-07-13 08:16:48.304010 chainfury_server-1.0.2/chainfury_server/api/metrics.py
+-rw-r--r--   0        0        0     5852 2023-07-13 08:20:52.792463 chainfury_server-1.0.2/chainfury_server/api/prompts.py
+-rw-r--r--   0        0        0     1948 2023-07-13 08:17:57.465712 chainfury_server-1.0.2/chainfury_server/api/template.py
+-rw-r--r--   0        0        0     1376 2023-07-13 08:18:08.982573 chainfury_server-1.0.2/chainfury_server/api/user.py
+-rw-r--r--   0        0        0     3415 2023-07-13 16:22:23.600200 chainfury_server-1.0.2/chainfury_server/app.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:13:15.390604 chainfury_server-1.0.2/chainfury_server/commons/__init__.py
+-rw-r--r--   0        0        0     1413 2023-06-12 14:13:15.390926 chainfury_server-1.0.2/chainfury_server/commons/config.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:13:15.391011 chainfury_server-1.0.2/chainfury_server/commons/constants.py
+-rw-r--r--   0        0        0     7563 2023-07-13 08:18:45.219487 chainfury_server-1.0.2/chainfury_server/commons/fury_utils.py
+-rw-r--r--   0        0        0     2944 2023-07-13 08:18:50.515872 chainfury_server-1.0.2/chainfury_server/commons/gpt_rating.py
+-rw-r--r--   0        0        0     5205 2023-07-13 08:19:02.364524 chainfury_server-1.0.2/chainfury_server/commons/langflow_utils.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:13:15.391843 chainfury_server-1.0.2/chainfury_server/commons/metrics_utils.py
+-rw-r--r--   0        0        0      563 2023-07-13 08:19:08.628139 chainfury_server-1.0.2/chainfury_server/commons/types.py
+-rw-r--r--   0        0        0     9937 2023-07-13 10:42:38.175235 chainfury_server-1.0.2/chainfury_server/commons/utils.py
+-rw-r--r--   0        0        0     8224 2023-07-13 08:22:11.384119 chainfury_server-1.0.2/chainfury_server/database.py
+-rw-r--r--   0        0        0      606 2023-06-12 14:13:15.394729 chainfury_server-1.0.2/chainfury_server/database_constants.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:13:15.394837 chainfury_server-1.0.2/chainfury_server/database_utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-13 08:15:47.541666 chainfury_server-1.0.2/chainfury_server/database_utils/chatbot.py
+-rw-r--r--   0        0        0     1141 2023-07-13 08:19:55.464141 chainfury_server-1.0.2/chainfury_server/database_utils/dashboard.py
+-rw-r--r--   0        0        0      458 2023-06-12 14:13:15.395389 chainfury_server-1.0.2/chainfury_server/database_utils/general_utils.py
+-rw-r--r--   0        0        0     1212 2023-07-13 08:15:47.461948 chainfury_server-1.0.2/chainfury_server/database_utils/intermediate_step.py
+-rw-r--r--   0        0        0      808 2023-07-13 08:15:47.436610 chainfury_server-1.0.2/chainfury_server/database_utils/prompt.py
+-rw-r--r--   0        0        0    20833 2023-06-12 14:13:15.396257 chainfury_server-1.0.2/chainfury_server/examples/basic_template.json
+-rw-r--r--   0        0        0    11731 2023-07-04 11:08:52.449936 chainfury_server-1.0.2/chainfury_server/examples/chuck_norris.json
+-rw-r--r--   0        0        0      713 2023-07-04 11:15:32.708753 chainfury_server-1.0.2/chainfury_server/examples/index.json
+-rw-r--r--   0        0        0     8830 2023-07-04 11:10:59.210504 chainfury_server-1.0.2/chainfury_server/examples/serper_summarizer.json
+-rw-r--r--   0        0        0      485 2023-06-12 14:13:15.398098 chainfury_server-1.0.2/chainfury_server/plugins/README.md
+-rw-r--r--   0        0        0      208 2023-07-13 08:20:52.728195 chainfury_server-1.0.2/chainfury_server/plugins/__init__.py
+-rw-r--r--   0        0        0     1317 2023-07-13 08:21:05.999858 chainfury_server-1.0.2/chainfury_server/plugins/base.py
+-rw-r--r--   0        0        0     1105 2023-07-13 08:20:28.446116 chainfury_server-1.0.2/chainfury_server/plugins/echo/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-13 08:22:39.591789 chainfury_server-1.0.2/chainfury_server/plugins/handler.py
+-rw-r--r--   0        0        0     1352 2023-07-13 08:20:28.423757 chainfury_server-1.0.2/chainfury_server/plugins/loader.py
+-rw-r--r--   0        0        0      370 2023-06-12 14:13:15.398994 chainfury_server-1.0.2/chainfury_server/plugins/nbx/README.md
+-rw-r--r--   0        0        0     1212 2023-07-13 08:20:52.750165 chainfury_server-1.0.2/chainfury_server/plugins/nbx/__init__.py
+-rw-r--r--   0        0        0     1871 2023-07-13 08:20:52.760557 chainfury_server-1.0.2/chainfury_server/plugins/nbx/lmao.py
+-rw-r--r--   0        0        0       93 2023-07-13 08:14:55.626096 chainfury_server-1.0.2/chainfury_server/plugins/nbx/utils.py
+-rw-r--r--   0        0        0        0 2023-06-12 14:13:15.399497 chainfury_server-1.0.2/chainfury_server/schemas/__init__.py
+-rw-r--r--   0        0        0      156 2023-06-12 14:13:15.399643 chainfury_server-1.0.2/chainfury_server/schemas/prompt_schema.py
+-rw-r--r--   0        0        0      456 2023-07-13 08:22:45.858540 chainfury_server-1.0.2/chainfury_server/server.py
+-rw-r--r--   0        0        0     6952 2023-04-26 06:34:46.433694 chainfury_server-1.0.2/chainfury_server/static/assets/Button-3149f941.js
+-rw-r--r--   0        0        0     6950 2023-06-20 13:47:53.255568 chainfury_server-1.0.2/chainfury_server/static/assets/Button-593e2495.js
+-rw-r--r--   0        0        0     6950 2023-06-26 08:19:02.031165 chainfury_server-1.0.2/chainfury_server/static/assets/Button-59c8a701.js
+-rw-r--r--   0        0        0     6950 2023-07-04 11:30:32.013065 chainfury_server-1.0.2/chainfury_server/static/assets/Button-5a4b534a.js
+-rw-r--r--   0        0        0     6950 2023-07-04 09:13:31.914124 chainfury_server-1.0.2/chainfury_server/static/assets/Button-c4b2e4dc.js
+-rw-r--r--   0        0        0     6950 2023-06-27 12:22:20.870023 chainfury_server-1.0.2/chainfury_server/static/assets/Button-ee88713e.js
+-rw-r--r--   0        0        0     6950 2023-07-04 04:41:08.275824 chainfury_server-1.0.2/chainfury_server/static/assets/Button-f8e4aa7f.js
+-rw-r--r--   0        0        0     5407 2023-06-27 12:22:20.870133 chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-038cacf7.js
+-rw-r--r--   0        0        0     5407 2023-06-20 13:47:53.258435 chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-25bd7bfc.js
+-rw-r--r--   0        0        0     2919 2023-04-26 06:34:46.440206 chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-2f5c1012.js
+-rw-r--r--   0        0        0     5407 2023-07-04 04:41:08.277845 chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-8d7894f9.js
+-rw-r--r--   0        0        0     5402 2023-07-04 11:30:32.014151 chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-c5140795.js
+-rw-r--r--   0        0        0     5407 2023-06-26 08:19:02.033268 chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-e4d4f5c0.js
+-rw-r--r--   0        0        0     5407 2023-07-04 09:13:31.913993 chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-f3bf7953.js
+-rw-r--r--   0        0        0    18349 2023-06-20 13:47:53.255828 chainfury_server-1.0.2/chainfury_server/static/assets/Close-28cfcc9d.js
+-rw-r--r--   0        0        0    19251 2023-06-26 08:19:02.031757 chainfury_server-1.0.2/chainfury_server/static/assets/Close-52ca7490.js
+-rw-r--r--   0        0        0    19251 2023-07-04 11:30:32.012073 chainfury_server-1.0.2/chainfury_server/static/assets/Close-59b68972.js
+-rw-r--r--   0        0        0    19251 2023-07-04 04:41:08.277104 chainfury_server-1.0.2/chainfury_server/static/assets/Close-bdf112d1.js
+-rw-r--r--   0        0        0    18321 2023-04-26 06:34:46.437970 chainfury_server-1.0.2/chainfury_server/static/assets/Close-d0ff1fdc.js
+-rw-r--r--   0        0        0    19251 2023-06-27 12:22:20.870447 chainfury_server-1.0.2/chainfury_server/static/assets/Close-f05ea766.js
+-rw-r--r--   0        0        0    19251 2023-07-04 09:13:31.914267 chainfury_server-1.0.2/chainfury_server/static/assets/Close-fc534dca.js
+-rw-r--r--   0        0        0    58829 2023-07-04 04:41:08.277257 chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-17acb7b6.js
+-rw-r--r--   0        0        0    58829 2023-07-04 09:13:31.912632 chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-8b686744.js
+-rw-r--r--   0        0        0    58731 2023-06-27 12:22:20.869602 chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-a27fa07d.js
+-rw-r--r--   0        0        0    10668 2023-04-26 06:34:46.436365 chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-a4b113e7.js
+-rw-r--r--   0        0        0    58731 2023-06-26 08:19:02.033392 chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-a5c783f7.js
+-rw-r--r--   0        0        0    58772 2023-06-20 13:47:53.257644 chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-c9de222f.js
+-rw-r--r--   0        0        0    58888 2023-07-04 11:30:32.013834 chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-e4a49fcb.js
+-rw-r--r--   0        0        0      992 2023-06-20 13:47:53.258177 chainfury_server-1.0.2/chainfury_server/static/assets/dispatchHooks-562c67db.js
+-rw-r--r--   0        0        0      993 2023-04-26 06:34:46.435878 chainfury_server-1.0.2/chainfury_server/static/assets/dispatchHooks-85107758.js
+-rw-r--r--   0        0        0      444 2023-04-26 06:34:46.437506 chainfury_server-1.0.2/chainfury_server/static/assets/index-0223be06.js
+-rw-r--r--   0        0        0     2255 2023-07-04 11:30:32.012657 chainfury_server-1.0.2/chainfury_server/static/assets/index-10efa1c9.js
+-rw-r--r--   0        0        0   341822 2023-06-27 12:22:20.870295 chainfury_server-1.0.2/chainfury_server/static/assets/index-1c76e43d.js
+-rw-r--r--   0        0        0     2037 2023-06-27 12:22:20.868410 chainfury_server-1.0.2/chainfury_server/static/assets/index-233b7bec.js
+-rw-r--r--   0        0        0   339600 2023-04-26 06:34:46.434837 chainfury_server-1.0.2/chainfury_server/static/assets/index-35325410.js
+-rw-r--r--   0        0        0     2091 2023-06-26 08:19:02.032455 chainfury_server-1.0.2/chainfury_server/static/assets/index-36d17591.js
+-rw-r--r--   0        0        0    25908 2023-04-26 06:34:46.439241 chainfury_server-1.0.2/chainfury_server/static/assets/index-3f4aa8cc.css
+-rw-r--r--   0        0        0  1119873 2023-07-04 11:30:32.014476 chainfury_server-1.0.2/chainfury_server/static/assets/index-4e19540d.js
+-rw-r--r--   0        0        0     2200 2023-07-04 04:41:08.276228 chainfury_server-1.0.2/chainfury_server/static/assets/index-5176fb7e.js
+-rw-r--r--   0        0        0  1119872 2023-06-27 12:22:20.869286 chainfury_server-1.0.2/chainfury_server/static/assets/index-529e483a.js
+-rw-r--r--   0        0        0     2037 2023-06-26 08:19:02.032235 chainfury_server-1.0.2/chainfury_server/static/assets/index-547b311b.js
+-rw-r--r--   0        0        0   341944 2023-07-04 09:13:31.913856 chainfury_server-1.0.2/chainfury_server/static/assets/index-5582c958.js
+-rw-r--r--   0        0        0   342086 2023-07-04 11:30:32.013270 chainfury_server-1.0.2/chainfury_server/static/assets/index-55f22566.js
+-rw-r--r--   0        0        0     6883 2023-07-04 11:30:32.012873 chainfury_server-1.0.2/chainfury_server/static/assets/index-57a158a9.css
+-rw-r--r--   0        0        0   228645 2023-06-26 08:19:02.031954 chainfury_server-1.0.2/chainfury_server/static/assets/index-5b6bc100.js
+-rw-r--r--   0        0        0     2112 2023-04-26 06:34:46.439610 chainfury_server-1.0.2/chainfury_server/static/assets/index-5cfeeef6.js
+-rw-r--r--   0        0        0    27870 2023-07-04 11:30:32.013418 chainfury_server-1.0.2/chainfury_server/static/assets/index-628511b6.css
+-rw-r--r--   0        0        0    27779 2023-07-04 04:41:08.276388 chainfury_server-1.0.2/chainfury_server/static/assets/index-68ec8b36.css
+-rw-r--r--   0        0        0   341736 2023-06-26 08:19:02.033593 chainfury_server-1.0.2/chainfury_server/static/assets/index-6ac8ab06.js
+-rw-r--r--   0        0        0   341944 2023-07-04 04:41:08.276043 chainfury_server-1.0.2/chainfury_server/static/assets/index-7221a78d.js
+-rw-r--r--   0        0        0   234892 2023-07-04 11:30:32.014978 chainfury_server-1.0.2/chainfury_server/static/assets/index-75500326.js
+-rw-r--r--   0        0        0   231540 2023-07-04 04:41:08.276672 chainfury_server-1.0.2/chainfury_server/static/assets/index-7d6e7c9a.js
+-rw-r--r--   0        0        0     2091 2023-06-27 12:22:20.869897 chainfury_server-1.0.2/chainfury_server/static/assets/index-81f0ebfb.js
+-rw-r--r--   0        0        0     2091 2023-06-20 13:47:53.254937 chainfury_server-1.0.2/chainfury_server/static/assets/index-9084c7e8.js
+-rw-r--r--   0        0        0     2091 2023-07-04 04:41:08.276802 chainfury_server-1.0.2/chainfury_server/static/assets/index-9546d633.js
+-rw-r--r--   0        0        0  1119359 2023-04-26 06:34:46.441000 chainfury_server-1.0.2/chainfury_server/static/assets/index-9b6b9c14.js
+-rw-r--r--   0        0        0   220504 2023-04-26 06:34:46.434201 chainfury_server-1.0.2/chainfury_server/static/assets/index-9da9e357.js
+-rw-r--r--   0        0        0  1119872 2023-07-04 04:41:08.277699 chainfury_server-1.0.2/chainfury_server/static/assets/index-9fd47f49.js
+-rw-r--r--   0        0        0  1119872 2023-06-26 08:19:02.032799 chainfury_server-1.0.2/chainfury_server/static/assets/index-a077d00c.js
+-rw-r--r--   0        0        0  1119872 2023-07-04 09:13:31.912994 chainfury_server-1.0.2/chainfury_server/static/assets/index-a6ad3f72.js
+-rw-r--r--   0        0        0   230102 2023-06-27 12:22:20.869763 chainfury_server-1.0.2/chainfury_server/static/assets/index-a8a84317.js
+-rw-r--r--   0        0        0     2037 2023-06-20 13:47:53.257911 chainfury_server-1.0.2/chainfury_server/static/assets/index-b4463069.js
+-rw-r--r--   0        0        0   234897 2023-07-04 09:13:31.914655 chainfury_server-1.0.2/chainfury_server/static/assets/index-b5b9763d.js
+-rw-r--r--   0        0        0  1119913 2023-06-20 13:47:53.257014 chainfury_server-1.0.2/chainfury_server/static/assets/index-b6e3039e.js
+-rw-r--r--   0        0        0     2037 2023-07-04 04:41:08.276950 chainfury_server-1.0.2/chainfury_server/static/assets/index-b9992484.js
+-rw-r--r--   0        0        0     2091 2023-07-04 11:30:32.014820 chainfury_server-1.0.2/chainfury_server/static/assets/index-c066588b.js
+-rw-r--r--   0        0        0     2037 2023-07-04 09:13:31.913444 chainfury_server-1.0.2/chainfury_server/static/assets/index-c1411de8.js
+-rw-r--r--   0        0        0   341798 2023-06-20 13:47:53.254640 chainfury_server-1.0.2/chainfury_server/static/assets/index-d4346eec.js
+-rw-r--r--   0        0        0      947 2023-06-27 12:22:20.868643 chainfury_server-1.0.2/chainfury_server/static/assets/index-e156bd3d.js
+-rw-r--r--   0        0        0     2171 2023-04-26 06:34:46.439914 chainfury_server-1.0.2/chainfury_server/static/assets/index-eb6972f0.js
+-rw-r--r--   0        0        0   226087 2023-06-20 13:47:53.255267 chainfury_server-1.0.2/chainfury_server/static/assets/index-eed7f1d2.js
+-rw-r--r--   0        0        0     2091 2023-07-04 09:13:31.914385 chainfury_server-1.0.2/chainfury_server/static/assets/index-f1d79a0e.js
+-rw-r--r--   0        0        0     2037 2023-07-04 11:30:32.013973 chainfury_server-1.0.2/chainfury_server/static/assets/index-ff44d1cd.js
+-rw-r--r--   0        0        0    27472 2023-06-20 13:47:53.256371 chainfury_server-1.0.2/chainfury_server/static/assets/index-ffbb8444.css
+-rw-r--r--   0        0        0       73 2023-06-20 13:47:53.257367 chainfury_server-1.0.2/chainfury_server/static/assets/store-06cc0006.js
+-rw-r--r--   0        0        0       73 2023-06-27 12:22:20.868532 chainfury_server-1.0.2/chainfury_server/static/assets/store-71291eee.js
+-rw-r--r--   0        0        0       73 2023-06-26 08:19:02.031026 chainfury_server-1.0.2/chainfury_server/static/assets/store-b83ff62b.js
+-rw-r--r--   0        0        0       73 2023-07-04 11:30:32.011921 chainfury_server-1.0.2/chainfury_server/static/assets/store-c9993eae.js
+-rw-r--r--   0        0        0       73 2023-07-04 04:41:08.277395 chainfury_server-1.0.2/chainfury_server/static/assets/store-ce236640.js
+-rw-r--r--   0        0        0       73 2023-04-26 06:34:46.436918 chainfury_server-1.0.2/chainfury_server/static/assets/store-d6cbae01.js
+-rw-r--r--   0        0        0       73 2023-07-04 09:13:31.913674 chainfury_server-1.0.2/chainfury_server/static/assets/store-e09eb698.js
+-rw-r--r--   0        0        0      227 2023-06-20 13:47:53.256092 chainfury_server-1.0.2/chainfury_server/static/assets/useControlled-00f12b58.js
+-rw-r--r--   0        0        0      227 2023-06-27 12:22:20.868778 chainfury_server-1.0.2/chainfury_server/static/assets/useControlled-1019e2b5.js
+-rw-r--r--   0        0        0      227 2023-06-26 08:19:02.033123 chainfury_server-1.0.2/chainfury_server/static/assets/useControlled-143349eb.js
+-rw-r--r--   0        0        0      227 2023-07-04 04:41:08.276517 chainfury_server-1.0.2/chainfury_server/static/assets/useControlled-360d1c06.js
+-rw-r--r--   0        0        0      227 2023-07-04 09:13:31.914502 chainfury_server-1.0.2/chainfury_server/static/assets/useControlled-63c4605a.js
+-rw-r--r--   0        0        0      227 2023-07-04 11:30:32.013675 chainfury_server-1.0.2/chainfury_server/static/assets/useControlled-6a808db7.js
+-rw-r--r--   0        0        0    77380 2023-07-04 11:30:32.011345 chainfury_server-1.0.2/chainfury_server/static/chainfury.png
+-rw-r--r--   0        0        0      454 2023-07-04 11:30:32.010881 chainfury_server-1.0.2/chainfury_server/static/index.html
+-rw-r--r--   0        0        0     2138 2023-07-04 11:30:32.011633 chainfury_server-1.0.2/chainfury_server/static/script/embedBot.js
+-rw-r--r--   0        0        0     1497 2023-04-26 06:34:46.432782 chainfury_server-1.0.2/chainfury_server/static/vite.svg
+-rw-r--r--   0        0        0        0 2023-06-12 14:13:15.400002 chainfury_server-1.0.2/chainfury_server/stories/__init__.py
+-rw-r--r--   0        0        0    10578 2023-06-26 12:43:39.055327 chainfury_server-1.0.2/chainfury_server/stories/api.py
+-rw-r--r--   0        0        0    15135 2023-06-12 14:13:15.400726 chainfury_server-1.0.2/chainfury_server/stories/dag.json
+-rw-r--r--   0        0        0      101 2023-07-13 08:20:52.793186 chainfury_server-1.0.2/chainfury_server/stories/plugins.py
+-rw-r--r--   0        0        0      454 2023-07-04 11:30:32.020977 chainfury_server-1.0.2/chainfury_server/templates/index.html
+-rw-r--r--   0        0        0      135 2023-07-13 16:22:09.809019 chainfury_server-1.0.2/chainfury_server/version.py
+-rw-r--r--   0        0        0     1302 2023-07-13 16:21:51.347844 chainfury_server-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 chainfury_server-1.0.2/setup.py
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 chainfury_server-1.0.2/PKG-INFO
```

### Comparing `chainfury_server-1.0.1/chainfury_server/api/auth.py` & `chainfury_server-1.0.2/chainfury_server/api/auth.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/api/chatbot.py` & `chainfury_server-1.0.2/chainfury_server/api/chatbot.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/api/dashboard.py` & `chainfury_server-1.0.2/chainfury_server/api/dashboard.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/api/feedback.py` & `chainfury_server-1.0.2/chainfury_server/api/feedback.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/api/fury.py` & `chainfury_server-1.0.2/chainfury_server/api/fury.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/api/intermediate_steps.py` & `chainfury_server-1.0.2/chainfury_server/api/intermediate_steps.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/api/metrics.py` & `chainfury_server-1.0.2/chainfury_server/api/metrics.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/api/prompts.py` & `chainfury_server-1.0.2/chainfury_server/api/prompts.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/api/template.py` & `chainfury_server-1.0.2/chainfury_server/api/template.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/api/user.py` & `chainfury_server-1.0.2/chainfury_server/api/user.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/app.py` & `chainfury_server-1.0.2/chainfury_server/app.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/commons/config.py` & `chainfury_server-1.0.2/chainfury_server/commons/config.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/commons/fury_utils.py` & `chainfury_server-1.0.2/chainfury_server/commons/fury_utils.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/commons/gpt_rating.py` & `chainfury_server-1.0.2/chainfury_server/commons/gpt_rating.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/commons/langflow_utils.py` & `chainfury_server-1.0.2/chainfury_server/commons/langflow_utils.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/commons/types.py` & `chainfury_server-1.0.2/chainfury_server/commons/types.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/commons/utils.py` & `chainfury_server-1.0.2/chainfury_server/commons/utils.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/database.py` & `chainfury_server-1.0.2/chainfury_server/database.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/database_constants.py` & `chainfury_server-1.0.2/chainfury_server/database_constants.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/database_utils/dashboard.py` & `chainfury_server-1.0.2/chainfury_server/database_utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/database_utils/intermediate_step.py` & `chainfury_server-1.0.2/chainfury_server/database_utils/intermediate_step.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/database_utils/prompt.py` & `chainfury_server-1.0.2/chainfury_server/database_utils/prompt.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/examples/basic_template.json` & `chainfury_server-1.0.2/chainfury_server/examples/basic_template.json`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/examples/chuck_norris.json` & `chainfury_server-1.0.2/chainfury_server/examples/chuck_norris.json`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/examples/index.json` & `chainfury_server-1.0.2/chainfury_server/examples/index.json`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/examples/serper_summarizer.json` & `chainfury_server-1.0.2/chainfury_server/examples/serper_summarizer.json`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/plugins/base.py` & `chainfury_server-1.0.2/chainfury_server/plugins/base.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/plugins/echo/__init__.py` & `chainfury_server-1.0.2/chainfury_server/plugins/echo/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/plugins/handler.py` & `chainfury_server-1.0.2/chainfury_server/plugins/handler.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/plugins/loader.py` & `chainfury_server-1.0.2/chainfury_server/plugins/loader.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/plugins/nbx/__init__.py` & `chainfury_server-1.0.2/chainfury_server/plugins/nbx/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/plugins/nbx/lmao.py` & `chainfury_server-1.0.2/chainfury_server/plugins/nbx/lmao.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Button-3149f941.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Button-3149f941.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Button-593e2495.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Button-593e2495.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Button-59c8a701.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Button-59c8a701.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Button-5a4b534a.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Button-5a4b534a.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Button-c4b2e4dc.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Button-c4b2e4dc.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Button-ee88713e.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Button-ee88713e.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Button-f8e4aa7f.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Button-f8e4aa7f.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-038cacf7.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-038cacf7.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-25bd7bfc.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-25bd7bfc.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-2f5c1012.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-2f5c1012.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-8d7894f9.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-8d7894f9.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-c5140795.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-c5140795.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-e4d4f5c0.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-e4d4f5c0.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/ChatComp-f3bf7953.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/ChatComp-f3bf7953.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Close-28cfcc9d.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Close-28cfcc9d.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Close-52ca7490.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Close-52ca7490.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Close-59b68972.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Close-59b68972.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Close-bdf112d1.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Close-bdf112d1.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Close-d0ff1fdc.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Close-d0ff1fdc.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Close-f05ea766.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Close-f05ea766.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Close-fc534dca.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Close-fc534dca.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-17acb7b6.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-17acb7b6.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-8b686744.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-8b686744.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-a27fa07d.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-a27fa07d.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-a4b113e7.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-a4b113e7.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-a5c783f7.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-a5c783f7.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-c9de222f.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-c9de222f.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/Sidebar-e4a49fcb.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/Sidebar-e4a49fcb.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/dispatchHooks-562c67db.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/dispatchHooks-562c67db.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/dispatchHooks-85107758.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/dispatchHooks-85107758.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-10efa1c9.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-10efa1c9.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-1c76e43d.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-1c76e43d.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-233b7bec.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-233b7bec.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-35325410.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-35325410.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-36d17591.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-36d17591.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-3f4aa8cc.css` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-3f4aa8cc.css`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-4e19540d.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-4e19540d.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-5176fb7e.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-5176fb7e.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-529e483a.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-529e483a.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-547b311b.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-547b311b.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-5582c958.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-5582c958.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-55f22566.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-55f22566.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-57a158a9.css` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-57a158a9.css`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-5b6bc100.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-5b6bc100.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-5cfeeef6.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-5cfeeef6.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-628511b6.css` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-628511b6.css`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-68ec8b36.css` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-68ec8b36.css`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-6ac8ab06.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-6ac8ab06.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-7221a78d.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-7221a78d.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-75500326.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-75500326.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-7d6e7c9a.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-7d6e7c9a.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-81f0ebfb.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-81f0ebfb.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-9084c7e8.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-9084c7e8.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-9546d633.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-9546d633.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-9b6b9c14.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-9b6b9c14.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-9da9e357.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-9da9e357.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-9fd47f49.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-9fd47f49.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-a077d00c.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-a077d00c.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-a6ad3f72.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-a6ad3f72.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-a8a84317.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-a8a84317.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-b4463069.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-b4463069.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-b5b9763d.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-b5b9763d.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-b6e3039e.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-b6e3039e.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-b9992484.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-b9992484.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-c066588b.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-c066588b.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-c1411de8.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-c1411de8.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-d4346eec.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-d4346eec.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-e156bd3d.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-e156bd3d.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-eb6972f0.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-eb6972f0.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-eed7f1d2.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-eed7f1d2.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-f1d79a0e.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-f1d79a0e.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-ff44d1cd.js` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-ff44d1cd.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/assets/index-ffbb8444.css` & `chainfury_server-1.0.2/chainfury_server/static/assets/index-ffbb8444.css`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/chainfury.png` & `chainfury_server-1.0.2/chainfury_server/static/chainfury.png`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/script/embedBot.js` & `chainfury_server-1.0.2/chainfury_server/static/script/embedBot.js`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/static/vite.svg` & `chainfury_server-1.0.2/chainfury_server/static/vite.svg`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/stories/api.py` & `chainfury_server-1.0.2/chainfury_server/stories/api.py`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/chainfury_server/stories/dag.json` & `chainfury_server-1.0.2/chainfury_server/stories/dag.json`

 * *Files identical despite different names*

### Comparing `chainfury_server-1.0.1/setup.py` & `chainfury_server-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,23 +17,53 @@
  'chainfury_server': ['examples/*',
                       'static/*',
                       'static/assets/*',
                       'static/script/*',
                       'templates/*']}
 
 install_requires = \
-['Jinja2==3.1.2', 'fire==0.5.0', 'jinja2schema==0.1.4']
+['black==23.3.0',
+ 'chromadb==0.3.21',
+ 'dill==0.3.6',
+ 'docstring-parser==0.15',
+ 'fake-useragent==1.1.3',
+ 'fastapi==0.95.2',
+ 'fire==0.5.0',
+ 'google-api-python-client==2.86.0',
+ 'google-search-results==2.4.2',
+ 'huggingface-hub==0.13.4',
+ 'jinja2',
+ 'jinja2schema==0.1.4',
+ 'langchain==0.0.141',
+ 'langflow==0.0.54',
+ 'lxml==4.9.2',
+ 'networkx==3.1',
+ 'openai==0.27.4',
+ 'pandas==1.5.3',
+ 'passlib==1.7.4',
+ 'psycopg2-binary==2.9.6',
+ 'pyarrow==11.0.0',
+ 'pyjwt[crypto]',
+ 'pymysql',
+ 'pypdf==3.8.1',
+ 'pysrt==1.1.2',
+ 'rich==13.3.4',
+ 'sqlalchemy',
+ 'typer==0.7.0',
+ 'types-pyyaml',
+ 'unstructured==0.6.1',
+ 'uvicorn==0.20.0']
 
 entry_points = \
 {'console_scripts': ['cf_server = chainfury_server.server:main',
                      'chainfury_server = chainfury_server.server:main']}
 
 setup_kwargs = {
     'name': 'chainfury-server',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'ChainFury Server is the open source server for running ChainFury Engine!',
     'long_description': '# ChainFury Server\n\nThis is a package separate from `chainfury` which provides the python execution engine.\n',
     'author': 'NimbleBox Engineering',
     'author_email': 'engineering@nimblebox.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/NimbleBoxAI/ChainFury',
```


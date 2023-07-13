# Comparing `tmp/MeUtils-2023.7.6.9.18.40.tar.gz` & `tmp/MeUtils-2023.7.7.15.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeUtils-2023.7.6.9.18.40.tar", last modified: Thu Jul  6 01:18:41 2023, max compression
+gzip compressed data, was "MeUtils-2023.7.7.15.3.6.tar", last modified: Fri Jul  7 07:03:06 2023, max compression
```

## Comparing `MeUtils-2023.7.6.9.18.40.tar` & `MeUtils-2023.7.7.15.3.6.tar`

### file list

```diff
@@ -1,548 +1,553 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.450931 MeUtils-2023.7.6.9.18.40/
--rw-r--r--   0 betterme   (501) staff       (20)     1204 2023-05-22 06:35:12.000000 MeUtils-2023.7.6.9.18.40/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/MANIFEST.in
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.347566 MeUtils-2023.7.6.9.18.40/MeUtils.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1893 2023-07-06 01:18:41.000000 MeUtils-2023.7.6.9.18.40/MeUtils.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)    18529 2023-07-06 01:18:41.000000 MeUtils-2023.7.6.9.18.40/MeUtils.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-07-06 01:18:41.000000 MeUtils-2023.7.6.9.18.40/MeUtils.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)      193 2023-07-06 01:18:41.000000 MeUtils-2023.7.6.9.18.40/MeUtils.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1039 2023-07-06 01:18:41.000000 MeUtils-2023.7.6.9.18.40/MeUtils.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)       17 2023-07-06 01:18:41.000000 MeUtils-2023.7.6.9.18.40/MeUtils.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1893 2023-07-06 01:18:41.450760 MeUtils-2023.7.6.9.18.40/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2023.7.6.9.18.40/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      105 2023-06-12 01:19:08.000000 MeUtils-2023.7.6.9.18.40/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/clear_git_history.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      289 2023-05-26 11:03:24.000000 MeUtils-2023.7.6.9.18.40/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.352466 MeUtils-2023.7.6.9.18.40/meutils/
--rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.7.6.9.18.40/meutils/_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.352820 MeUtils-2023.7.6.9.18.40/meutils/ai_audio/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_audio/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      637 2023-05-17 05:56:24.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_audio/asr.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.353309 MeUtils-2023.7.6.9.18.40/meutils/ai_cv/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_cv/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:11:56.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_cv/ocr.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.355912 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/
--rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/SplitSentence.py
--rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/Untitled-1(1).py
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/_lda.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.356622 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/_textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/_textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/_textsplitter/text_split.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/lda.py
--rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-06-05 05:29:27.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/ner.py
--rw-r--r--   0 betterme   (501) staff       (20)      963 2023-07-04 08:24:23.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/sentence_transformers.py
--rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.359293 MeUtils-2023.7.6.9.18.40/meutils/ann/
--rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/README_gensim.md
--rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/ann.py
--rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/ann_faiss.py
--rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/ann_gensim.py
--rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/ann_inmemory.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/ann_qdrant.py
--rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/ann_service.py
--rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/ann_v1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.359591 MeUtils-2023.7.6.9.18.40/meutils/ann/examples/
--rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/examples/client.py
--rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/examples/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/milvus.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/ann/shake_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.359739 MeUtils-2023.7.6.9.18.40/meutils/asyncio_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/asyncio_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6054 2023-07-06 01:10:38.000000 MeUtils-2023.7.6.9.18.40/meutils/cache_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.361167 MeUtils-2023.7.6.9.18.40/meutils/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/clis/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/clis/cron.py
--rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/clis/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/clis/gunicorn.conf.py
--rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/clis/monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/clis/nesc.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.361903 MeUtils-2023.7.6.9.18.40/meutils/cmds/
--rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/cmds/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/cmds/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/cmds/cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/cmds/hdfs_cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/cmds/subprocess_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.362194 MeUtils-2023.7.6.9.18.40/meutils/coding/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/coding/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/coding/find132.py
--rw-r--r--   0 betterme   (501) staff       (20)    10315 2023-07-06 01:18:39.000000 MeUtils-2023.7.6.9.18.40/meutils/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.362533 MeUtils-2023.7.6.9.18.40/meutils/comp_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/comp_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/comp_utils/reverse_metric.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.370604 MeUtils-2023.7.6.9.18.40/meutils/data/
--rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.7.6.9.18.40/meutils/data/SimHei.ttf
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-07-06 01:18:40.000000 MeUtils-2023.7.6.9.18.40/meutils/data/VERSION
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/data/_FLAG
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/data/_SUCCESS
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/data/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/data/coordinate.py
--rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/date_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.375307 MeUtils-2023.7.6.9.18.40/meutils/db/
--rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/db/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     7396 2023-06-30 01:59:42.000000 MeUtils-2023.7.6.9.18.40/meutils/db/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/db/mongo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/db/neo4j.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.377481 MeUtils-2023.7.6.9.18.40/meutils/decorators/
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/decorators/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2023.7.6.9.18.40/meutils/decorators/__ai.py
--rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/decorators/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/decorators/catch.py
--rw-r--r--   0 betterme   (501) staff       (20)     7099 2023-07-03 09:51:08.000000 MeUtils-2023.7.6.9.18.40/meutils/decorators/common.py
--rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.7.6.9.18.40/meutils/decorators/decorator.py
--rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/decorators/decorator_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/decorators/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/decorators/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/decorators/retry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.7.6.9.18.40/meutils/decorators/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2023.7.6.9.18.40/meutils/dist_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.378854 MeUtils-2023.7.6.9.18.40/meutils/docarray_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.7.6.9.18.40/meutils/docarray_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/docarray_utils/demo_es.py
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.7.6.9.18.40/meutils/docarray_utils/demo_hnsw.py
--rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.7.6.9.18.40/meutils/docarray_utils/in_memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.7.6.9.18.40/meutils/docarray_utils/改造下hnsw.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.379332 MeUtils-2023.7.6.9.18.40/meutils/easy_search/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/easy_search/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2217 2023-05-25 08:27:44.000000 MeUtils-2023.7.6.9.18.40/meutils/easy_search/es.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.381662 MeUtils-2023.7.6.9.18.40/meutils/fileparser/
--rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2023.7.6.9.18.40/meutils/fileparser/PDF抽取.py
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-18 08:38:53.000000 MeUtils-2023.7.6.9.18.40/meutils/fileparser/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:32:11.000000 MeUtils-2023.7.6.9.18.40/meutils/fileparser/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-18 08:39:22.000000 MeUtils-2023.7.6.9.18.40/meutils/fileparser/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:39:36.000000 MeUtils-2023.7.6.9.18.40/meutils/fileparser/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.7.6.9.18.40/meutils/hash_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/import_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.382297 MeUtils-2023.7.6.9.18.40/meutils/init/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.7.6.9.18.40/meutils/init/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1303 2023-06-04 08:38:47.000000 MeUtils-2023.7.6.9.18.40/meutils/init/evn.py
--rw-r--r--   0 betterme   (501) staff       (20)    12884 2023-07-06 01:18:39.000000 MeUtils-2023.7.6.9.18.40/meutils/init/oo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.383475 MeUtils-2023.7.6.9.18.40/meutils/io/
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.7.6.9.18.40/meutils/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/io/file.py
--rw-r--r--   0 betterme   (501) staff       (20)     2319 2023-05-30 01:57:16.000000 MeUtils-2023.7.6.9.18.40/meutils/io/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2023.7.6.9.18.40/meutils/io/tf_io.py
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/io/x.yml
--rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/jinja_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.7.6.9.18.40/meutils/log_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.385828 MeUtils-2023.7.6.9.18.40/meutils/notice/
--rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/notice/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/notice/emails.py
--rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/notice/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/notice/file_post.py
--rw-r--r--   0 betterme   (501) staff       (20)     2511 2023-06-13 09:13:04.000000 MeUtils-2023.7.6.9.18.40/meutils/notice/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/notice/wechat_.py
--rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/notice/wecom.py
--rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/notice/weekmeet.py
--rw-r--r--   0 betterme   (501) staff       (20)     2962 2023-05-16 06:23:15.000000 MeUtils-2023.7.6.9.18.40/meutils/np_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.387483 MeUtils-2023.7.6.9.18.40/meutils/office_automation/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/office_automation/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.7.6.9.18.40/meutils/office_automation/doc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1538 2023-04-28 07:14:17.000000 MeUtils-2023.7.6.9.18.40/meutils/office_automation/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.7.6.9.18.40/meutils/office_automation/pdm.py
--rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.7.6.9.18.40/meutils/office_automation/pdm_run.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.388453 MeUtils-2023.7.6.9.18.40/meutils/office_automation/report/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/office_automation/report/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/office_automation/投资管理系统O3.2_交易组.pdm
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.389463 MeUtils-2023.7.6.9.18.40/meutils/other/
--rw-r--r--   0 betterme   (501) staff       (20)      996 2023-07-04 01:28:59.000000 MeUtils-2023.7.6.9.18.40/meutils/other/__demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/other/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.391221 MeUtils-2023.7.6.9.18.40/meutils/other/aiomultiprocess/
--rw-r--r--   0 betterme   (501) staff       (20)      416 2023-07-04 01:05:39.000000 MeUtils-2023.7.6.9.18.40/meutils/other/aiomultiprocess/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-07-04 01:01:15.000000 MeUtils-2023.7.6.9.18.40/meutils/other/aiomultiprocess/__version__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7835 2023-07-04 01:01:15.000000 MeUtils-2023.7.6.9.18.40/meutils/other/aiomultiprocess/core.py
--rw-r--r--   0 betterme   (501) staff       (20)    11688 2023-07-04 01:01:15.000000 MeUtils-2023.7.6.9.18.40/meutils/other/aiomultiprocess/pool.py
--rw-r--r--   0 betterme   (501) staff       (20)     2573 2023-07-04 01:01:15.000000 MeUtils-2023.7.6.9.18.40/meutils/other/aiomultiprocess/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1037 2023-07-04 01:01:15.000000 MeUtils-2023.7.6.9.18.40/meutils/other/aiomultiprocess/types.py
--rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/other/besttable.py
--rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.7.6.9.18.40/meutils/other/crontab.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.391908 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/
--rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.394835 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/
--rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/annlite.py
--rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/chunk.py
--rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/document.py
--rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/elastic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/match.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/milvus.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.398992 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/content.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.399417 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/dataloader/
--rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/dataloader/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/dataloader/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/delitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/embed.py
--rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/empty.py
--rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/getattr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/getitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/group.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.400922 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/binary.py
--rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/csv.py
--rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/dataframe.py
--rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/from_gen.py
--rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/json.py
--rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/pbar.py
--rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/pushpull.py
--rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/match.py
--rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/parallel.py
--rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/post.py
--rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/reduce.py
--rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/sample.py
--rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/setitem.py
--rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/traverse.py
--rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/opensearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/qdrant.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.401674 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/queryset/
--rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/queryset/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/queryset/lookup.py
--rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/queryset/parser.py
--rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/redis.py
--rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/sqlite.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.401938 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.402835 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.403638 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/base/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/base/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/base/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/base/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/base/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.404487 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/elastic/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/elastic/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/elastic/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/elastic/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/elastic/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/elastic/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.405325 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/memory/
--rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/memory/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/memory/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/memory/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/memory/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/memory/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.406176 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/milvus/
--rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/milvus/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/milvus/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/milvus/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/milvus/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/milvus/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.407048 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/opensearch/
--rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/opensearch/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/opensearch/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/opensearch/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/opensearch/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/opensearch/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.408059 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/
--rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.408782 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/redis/
--rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/redis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/redis/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/redis/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/redis/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/redis/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/registry.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.409501 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/sqlite/
--rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/sqlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/sqlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/sqlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/sqlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/sqlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.410430 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/weaviate/
--rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/weaviate/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/weaviate/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/weaviate/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/weaviate/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/weaviate/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/weaviate.py
--rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/base.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.411412 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/dataclasses/
--rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/dataclasses/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/dataclasses/enums.py
--rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/dataclasses/getter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/dataclasses/setter.py
--rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/dataclasses/types.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.412402 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/
--rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/data.py
--rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/generators.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.416394 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/_property.py
--rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/attribute.py
--rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/audio.py
--rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/blob.py
--rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/content.py
--rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/convert.py
--rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/dump.py
--rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/featurehash.py
--rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/mesh.py
--rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/multimodal.py
--rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/porting.py
--rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/protobuf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/rich_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/sugar.py
--rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/video.py
--rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/pydantic_model.py
--rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/strawberry_type.py
--rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/helper.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.417100 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.418046 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/distance/
--rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/distance/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/distance/numpy.py
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/distance/paddle.py
--rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/distance/tensorflow.py
--rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/distance/torch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.418311 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.418602 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/io/
--rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/io/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.418861 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/pb/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/pb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/pb/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.419109 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/pb2/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/pb2/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/pb2/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.419266 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/resources/
--rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/resources/ci-vendors.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.419424 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/resources/embedding-projector/
--rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/resources/embedding-projector/index.html.gz
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.420127 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/score/
--rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/score/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/score/data.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.420577 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/score/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/score/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/score/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/score/mixins/representer.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.420740 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/typing/
--rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.7.6.9.18.40/meutils/other/docarray/typing/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.421310 MeUtils-2023.7.6.9.18.40/meutils/pandas_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/pandas_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/pandas_utils/opt.py
--rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/pandas_utils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.7.6.9.18.40/meutils/path_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     8435 2023-07-04 01:07:58.000000 MeUtils-2023.7.6.9.18.40/meutils/pipe.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.423183 MeUtils-2023.7.6.9.18.40/meutils/plot_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/plot_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      265 2023-05-09 07:50:11.000000 MeUtils-2023.7.6.9.18.40/meutils/plot_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/plot_utils/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/plot_utils/echarts.py
--rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2023.7.6.9.18.40/meutils/plot_utils/embedding_plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.7.6.9.18.40/meutils/plot_utils/mecharts.py
--rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/plot_utils/metrics.py
--rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/plot_utils/plot_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.424305 MeUtils-2023.7.6.9.18.40/meutils/request_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     2461 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/request_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.7.6.9.18.40/meutils/request_utils/crawler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.7.6.9.18.40/meutils/request_utils/download.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/request_utils/results.py
--rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/request_utils/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/request_utils/公网ip.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.425021 MeUtils-2023.7.6.9.18.40/meutils/serving/
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/_fastapi.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.425623 MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.426069 MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/__demo/异步任务.py
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2119 2023-07-03 09:53:08.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.426627 MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/errors/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/errors/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-05-25 10:51:34.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/errors/http_error.py
--rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/errors/validation_error.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.427625 MeUtils-2023.7.6.9.18.40/meutils/serving/gui/
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/gui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/gui/bar.py
--rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/gui/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/gui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.427879 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.428972 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/__demo/client.py
--rw-r--r--   0 betterme   (501) staff       (20)    13659 2023-05-18 02:37:48.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/__demo/flow.svg
--rw-r--r--   0 betterme   (501) staff       (20)     2011 2023-05-18 02:37:46.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/__demo/server.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.429511 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/executors/
--rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/executors/SentenceEncoder.py
--rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/executors/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.430071 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/nlp_serving/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/nlp_serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/jina/nlp_serving/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.431477 MeUtils-2023.7.6.9.18.40/meutils/serving/st_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/st_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      826 2023-05-15 04:13:53.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/st_utils/_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     7163 2023-05-30 01:47:36.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/st_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-05-15 03:46:21.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/st_utils/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/st_utils/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.432837 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.433399 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/.streamlit/
--rw-r--r--   0 betterme   (501) staff       (20)     7586 2023-03-24 08:27:34.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/.streamlit/_config.toml
--rw-r--r--   0 betterme   (501) staff       (20)      511 2023-03-24 08:27:34.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/.streamlit/config.toml
--rw-r--r--   0 betterme   (501) staff       (20)     1756 2023-05-22 09:24:56.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/_2_词性标注与实体识别.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-05-22 10:05:43.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/_🏆_主页.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.434260 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/pages/
--rw-r--r--   0 betterme   (501) staff       (20)     1943 2023-05-22 10:51:26.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/pages/_1_分词.py
--rw-r--r--   0 betterme   (501) staff       (20)     1714 2023-05-22 10:56:06.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/pages/_2_词性标注与实体识别.py
--rw-r--r--   0 betterme   (501) staff       (20)     2424 2023-05-22 10:48:03.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/pages/_3_文本匹配.py
--rwxr--r--   0 betterme   (501) staff       (20)      252 2023-05-22 10:17:52.000000 MeUtils-2023.7.6.9.18.40/meutils/serving/webui/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/sftp.py
--rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/sk_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/smooth_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.434608 MeUtils-2023.7.6.9.18.40/meutils/spark/
--rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/spark/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.435505 MeUtils-2023.7.6.9.18.40/meutils/str_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/str_utils/Translator.py
--rw-r--r--   0 betterme   (501) staff       (20)     6655 2023-05-17 05:26:27.000000 MeUtils-2023.7.6.9.18.40/meutils/str_utils/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.436434 MeUtils-2023.7.6.9.18.40/meutils/str_utils/__translater/
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/str_utils/__translater/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/str_utils/__translater/tencent.py
--rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/str_utils/__translater/translater.py
--rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/str_utils/__translater/youdao.py
--rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2023.7.6.9.18.40/meutils/str_utils/json_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      926 2023-04-09 12:05:21.000000 MeUtils-2023.7.6.9.18.40/meutils/str_utils/regular_expression.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.439201 MeUtils-2023.7.6.9.18.40/meutils/templates/
--rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/demo.conf
--rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/demo.j2
--rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/demox.py
--rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/df_html.j2
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.440662 MeUtils-2023.7.6.9.18.40/meutils/templates/dockerfiles/
--rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/dockerfiles/Dockerfile
--rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/dockerfiles/Dockerfile_me
--rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/dockerfiles/Dockerfile_milvus
--rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/dockerfiles/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/dockerfiles/docker_build_push.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/dockerfiles/docker_push.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/hegui.py
--rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/markmap.html
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.440826 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/
--rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/cookiecutter.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.444326 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.444488 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
--rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.446780 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.447048 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
--rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
--rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.447433 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.447789 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.448404 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/tpl.docx
--rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/x.html
--rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/templates/合规日报模板.docx
--rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2023.7.6.9.18.40/meutils/todo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.449786 MeUtils-2023.7.6.9.18.40/meutils/tools/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/tools/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/tools/cprint.py
--rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/tools/machine_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/tools/monitor.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/tools/seize.py
--rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/tools/service_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/tools/sys_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      360 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/typings.py
--rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/meutils/zk_utils.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      526 2023-05-15 03:11:01.000000 MeUtils-2023.7.6.9.18.40/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)      351 2023-06-28 06:59:00.000000 MeUtils-2023.7.6.9.18.40/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/requirements_ai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/requirements_app.txt
--rw-r--r--   0 betterme   (501) staff       (20)       52 2023-06-02 06:00:11.000000 MeUtils-2023.7.6.9.18.40/requirements_db.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-18 08:43:00.000000 MeUtils-2023.7.6.9.18.40/requirements_fileparser.txt
--rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/requirements_office.txt
--rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/requirements_pd.txt
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/requirements_plot.txt
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/requirements_plus.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-06 01:18:41.450481 MeUtils-2023.7.6.9.18.40/scripts/
--rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/scripts/demo.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/scripts/killall.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/scripts/py_sh.sh
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/scripts/yum.sh
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-07-06 01:18:41.450978 MeUtils-2023.7.6.9.18.40/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.7.6.9.18.40/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.948479 MeUtils-2023.7.7.15.3.6/
+-rw-r--r--   0 betterme   (501) staff       (20)     1204 2023-05-22 06:35:12.000000 MeUtils-2023.7.7.15.3.6/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/MANIFEST.in
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.836333 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)    18628 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      193 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1039 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       17 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-07-07 07:03:06.948305 MeUtils-2023.7.7.15.3.6/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2023.7.7.15.3.6/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      105 2023-06-12 01:19:08.000000 MeUtils-2023.7.7.15.3.6/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/clear_git_history.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      289 2023-05-26 11:03:24.000000 MeUtils-2023.7.7.15.3.6/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.841564 MeUtils-2023.7.7.15.3.6/meutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.7.7.15.3.6/meutils/_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.841988 MeUtils-2023.7.7.15.3.6/meutils/ai_audio/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_audio/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      637 2023-05-17 05:56:24.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_audio/asr.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.842473 MeUtils-2023.7.7.15.3.6/meutils/ai_cv/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_cv/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:11:56.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_cv/ocr.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.845000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/
+-rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/SplitSentence.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/Untitled-1(1).py
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_lda.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.845689 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/text_split.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/lda.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-06-05 05:29:27.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/ner.py
+-rw-r--r--   0 betterme   (501) staff       (20)      963 2023-07-04 08:24:23.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/sentence_transformers.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.848251 MeUtils-2023.7.7.15.3.6/meutils/ann/
+-rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/README_gensim.md
+-rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_faiss.py
+-rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_gensim.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_inmemory.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_qdrant.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_service.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_v1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.848634 MeUtils-2023.7.7.15.3.6/meutils/ann/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/examples/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/examples/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/milvus.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/shake_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.848851 MeUtils-2023.7.7.15.3.6/meutils/asyncio_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/asyncio_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6839 2023-07-07 07:01:54.000000 MeUtils-2023.7.7.15.3.6/meutils/cache_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.849634 MeUtils-2023.7.7.15.3.6/meutils/cachedir/
+-rw-r--r--   0 betterme   (501) staff       (20)    32768 2023-07-06 12:37:19.000000 MeUtils-2023.7.7.15.3.6/meutils/cachedir/cache.db
+-rw-r--r--   0 betterme   (501) staff       (20)    32768 2023-07-06 12:37:19.000000 MeUtils-2023.7.7.15.3.6/meutils/cachedir/cache.db-shm
+-rw-r--r--   0 betterme   (501) staff       (20)    98912 2023-07-06 12:37:51.000000 MeUtils-2023.7.7.15.3.6/meutils/cachedir/cache.db-wal
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.851249 MeUtils-2023.7.7.15.3.6/meutils/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/cron.py
+-rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/gunicorn.conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/nesc.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.852109 MeUtils-2023.7.7.15.3.6/meutils/cmds/
+-rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/cmds/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/cmds/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/cmds/cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/cmds/hdfs_cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/cmds/subprocess_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.852414 MeUtils-2023.7.7.15.3.6/meutils/coding/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/coding/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/coding/find132.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10338 2023-07-06 09:14:28.000000 MeUtils-2023.7.7.15.3.6/meutils/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.852772 MeUtils-2023.7.7.15.3.6/meutils/comp_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/comp_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/comp_utils/reverse_metric.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.861386 MeUtils-2023.7.7.15.3.6/meutils/data/
+-rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.7.7.15.3.6/meutils/data/SimHei.ttf
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/meutils/data/VERSION
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/data/_FLAG
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/data/_SUCCESS
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/data/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/data/coordinate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/date_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.866395 MeUtils-2023.7.7.15.3.6/meutils/db/
+-rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/db/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     7396 2023-06-30 01:59:42.000000 MeUtils-2023.7.7.15.3.6/meutils/db/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/db/mongo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/db/neo4j.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.870025 MeUtils-2023.7.7.15.3.6/meutils/decorators/
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/__ai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/catch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7099 2023-07-03 09:51:08.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/decorator.py
+-rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/decorator_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/retry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2023.7.7.15.3.6/meutils/dist_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.871277 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/demo_es.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/demo_hnsw.py
+-rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/in_memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/改造下hnsw.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.871673 MeUtils-2023.7.7.15.3.6/meutils/easy_search/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/easy_search/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2217 2023-05-25 08:27:44.000000 MeUtils-2023.7.7.15.3.6/meutils/easy_search/es.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.872805 MeUtils-2023.7.7.15.3.6/meutils/fileparser/
+-rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2023.7.7.15.3.6/meutils/fileparser/PDF抽取.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-18 08:38:53.000000 MeUtils-2023.7.7.15.3.6/meutils/fileparser/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:32:11.000000 MeUtils-2023.7.7.15.3.6/meutils/fileparser/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-18 08:39:22.000000 MeUtils-2023.7.7.15.3.6/meutils/fileparser/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:39:36.000000 MeUtils-2023.7.7.15.3.6/meutils/fileparser/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.7.7.15.3.6/meutils/hash_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/import_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.873569 MeUtils-2023.7.7.15.3.6/meutils/init/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.7.7.15.3.6/meutils/init/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1303 2023-06-04 08:38:47.000000 MeUtils-2023.7.7.15.3.6/meutils/init/evn.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12884 2023-07-06 01:18:39.000000 MeUtils-2023.7.7.15.3.6/meutils/init/oo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.875181 MeUtils-2023.7.7.15.3.6/meutils/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.7.7.15.3.6/meutils/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/io/file.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2319 2023-05-30 01:57:16.000000 MeUtils-2023.7.7.15.3.6/meutils/io/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2023.7.7.15.3.6/meutils/io/tf_io.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/io/x.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/jinja_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.7.7.15.3.6/meutils/log_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.876625 MeUtils-2023.7.7.15.3.6/meutils/notice/
+-rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/emails.py
+-rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/file_post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2511 2023-06-13 09:13:04.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/wechat_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/wecom.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/weekmeet.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2962 2023-05-16 06:23:15.000000 MeUtils-2023.7.7.15.3.6/meutils/np_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.878597 MeUtils-2023.7.7.15.3.6/meutils/office_automation/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/doc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1538 2023-04-28 07:14:17.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdm.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdm_run.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.879554 MeUtils-2023.7.7.15.3.6/meutils/office_automation/report/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/report/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/投资管理系统O3.2_交易组.pdm
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.880861 MeUtils-2023.7.7.15.3.6/meutils/other/
+-rw-r--r--   0 betterme   (501) staff       (20)      996 2023-07-04 01:28:59.000000 MeUtils-2023.7.7.15.3.6/meutils/other/__demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/other/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.882639 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/
+-rw-r--r--   0 betterme   (501) staff       (20)      416 2023-07-04 01:05:39.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-07-04 01:01:15.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/__version__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7835 2023-07-04 01:01:15.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/core.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11688 2023-07-04 01:01:15.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/pool.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2573 2023-07-04 01:01:15.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1037 2023-07-04 01:01:15.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/types.py
+-rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/other/besttable.py
+-rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.7.7.15.3.6/meutils/other/crontab.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.883513 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/
+-rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.886675 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/
+-rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/annlite.py
+-rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/chunk.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/document.py
+-rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/elastic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/milvus.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.891498 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/content.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.891921 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/dataloader/
+-rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/dataloader/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/dataloader/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/delitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/embed.py
+-rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/empty.py
+-rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/getattr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/getitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/group.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.893500 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/binary.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/csv.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/dataframe.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/from_gen.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/json.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/pbar.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/pushpull.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/parallel.py
+-rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/reduce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/sample.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/setitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/traverse.py
+-rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/opensearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/qdrant.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.894237 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/
+-rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/lookup.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/parser.py
+-rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/redis.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/sqlite.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.894525 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.895446 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.896430 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.897354 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.898243 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/
+-rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.899108 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/
+-rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.900182 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/
+-rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.901466 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/
+-rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.902386 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/
+-rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/registry.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.903304 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.904334 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/
+-rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/weaviate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/base.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.905394 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/
+-rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/enums.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/getter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/setter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/types.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.906491 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/
+-rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/data.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/generators.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.910431 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/_property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/attribute.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/audio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/blob.py
+-rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/content.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/convert.py
+-rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/dump.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/featurehash.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/mesh.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/multimodal.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/porting.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/protobuf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/rich_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/sugar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/pydantic_model.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/strawberry_type.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/helper.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.911152 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.912094 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/
+-rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/numpy.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/paddle.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/tensorflow.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/torch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.912379 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.912713 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/io/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.913091 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.913419 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb2/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb2/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb2/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.913627 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/
+-rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/ci-vendors.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.913819 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/embedding-projector/
+-rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/embedding-projector/index.html.gz
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.914714 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/
+-rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/data.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.915181 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/mixins/representer.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.915335 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/typing/
+-rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/typing/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.917774 MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/opt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.7.7.15.3.6/meutils/path_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8435 2023-07-04 01:07:58.000000 MeUtils-2023.7.7.15.3.6/meutils/pipe.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.919552 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      265 2023-05-09 07:50:11.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/echarts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/embedding_plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/mecharts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/metrics.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/plot_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.920881 MeUtils-2023.7.7.15.3.6/meutils/request_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     2461 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/crawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/download.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/results.py
+-rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/公网ip.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.921558 MeUtils-2023.7.7.15.3.6/meutils/serving/
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/_fastapi.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.922145 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.922666 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/__demo/异步任务.py
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2119 2023-07-03 09:53:08.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.923251 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/errors/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/errors/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-05-25 10:51:34.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/errors/http_error.py
+-rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/errors/validation_error.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.924238 MeUtils-2023.7.7.15.3.6/meutils/serving/gui/
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/gui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/gui/bar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/gui/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/gui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.924495 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.925805 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13659 2023-05-18 02:37:48.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/flow.svg
+-rw-r--r--   0 betterme   (501) staff       (20)     2011 2023-05-18 02:37:46.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/server.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.926341 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/executors/
+-rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/executors/SentenceEncoder.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/executors/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.926898 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/nlp_serving/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/nlp_serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/nlp_serving/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.928337 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      826 2023-05-15 04:13:53.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7163 2023-05-30 01:47:36.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-05-15 03:46:21.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.929416 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.929916 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/.streamlit/
+-rw-r--r--   0 betterme   (501) staff       (20)     7586 2023-03-24 08:27:34.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/.streamlit/_config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)      511 2023-03-24 08:27:34.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/.streamlit/config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)     1756 2023-05-22 09:24:56.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-05-22 10:05:43.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/_🏆_主页.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.930615 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/
+-rw-r--r--   0 betterme   (501) staff       (20)     1943 2023-05-22 10:51:26.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_1_分词.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1714 2023-05-22 10:56:06.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2424 2023-05-22 10:48:03.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_3_文本匹配.py
+-rwxr--r--   0 betterme   (501) staff       (20)      252 2023-05-22 10:17:52.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/sftp.py
+-rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/sk_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/smooth_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.930918 MeUtils-2023.7.7.15.3.6/meutils/spark/
+-rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/spark/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.931887 MeUtils-2023.7.7.15.3.6/meutils/str_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/Translator.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6655 2023-05-17 05:26:27.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.932637 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/tencent.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/translater.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/youdao.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/json_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      926 2023-04-09 12:05:21.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/regular_expression.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.935181 MeUtils-2023.7.7.15.3.6/meutils/templates/
+-rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/demo.conf
+-rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/demo.j2
+-rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/demox.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/df_html.j2
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.937767 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/
+-rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/Dockerfile
+-rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/Dockerfile_me
+-rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/Dockerfile_milvus
+-rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/docker_build_push.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/docker_push.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/hegui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/markmap.html
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.937963 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/
+-rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/cookiecutter.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.942277 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.942441 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.945014 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.945168 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
+-rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.945528 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.945852 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.946369 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/tpl.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/x.html
+-rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/合规日报模板.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2023.7.7.15.3.6/meutils/todo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.947430 MeUtils-2023.7.7.15.3.6/meutils/tools/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/cprint.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/machine_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/monitor.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/seize.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/service_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/sys_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      360 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/typings.py
+-rw-r--r--   0 betterme   (501) staff       (20)      396 2023-07-06 12:39:08.000000 MeUtils-2023.7.7.15.3.6/meutils/x.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/zk_utils.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      526 2023-05-15 03:11:01.000000 MeUtils-2023.7.7.15.3.6/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      351 2023-06-28 06:59:00.000000 MeUtils-2023.7.7.15.3.6/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_ai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_app.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       52 2023-06-02 06:00:11.000000 MeUtils-2023.7.7.15.3.6/requirements_db.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-18 08:43:00.000000 MeUtils-2023.7.7.15.3.6/requirements_fileparser.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_office.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_pd.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_plot.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_plus.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.948033 MeUtils-2023.7.7.15.3.6/scripts/
+-rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/scripts/demo.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/scripts/killall.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/scripts/py_sh.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/scripts/yum.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-07-07 07:03:06.948536 MeUtils-2023.7.7.15.3.6/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/setup.py
```

### Comparing `MeUtils-2023.7.6.9.18.40/.gitignore` & `MeUtils-2023.7.7.15.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/LICENSE` & `MeUtils-2023.7.7.15.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/MeUtils.egg-info/PKG-INFO` & `MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.7.6.9.18.40
+Version: 2023.7.7.15.3.6
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `MeUtils-2023.7.6.9.18.40/MeUtils.egg-info/SOURCES.txt` & `MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 meutils/pd_utils.py
 meutils/pipe.py
 meutils/sftp.py
 meutils/sk_utils.py
 meutils/smooth_utils.py
 meutils/todo.py
 meutils/typings.py
+meutils/x.py
 meutils/zk_utils.py
 meutils/ai_audio/__init__.py
 meutils/ai_audio/asr.py
 meutils/ai_cv/__init__.py
 meutils/ai_cv/ocr.py
 meutils/ai_nlp/SplitSentence.py
 meutils/ai_nlp/Untitled-1(1).py
@@ -71,14 +72,17 @@
 meutils/ann/ann_v1.py
 meutils/ann/cli.py
 meutils/ann/milvus.py
 meutils/ann/shake_demo.py
 meutils/ann/examples/client.py
 meutils/ann/examples/demo.py
 meutils/asyncio_utils/__init__.py
+meutils/cachedir/cache.db
+meutils/cachedir/cache.db-shm
+meutils/cachedir/cache.db-wal
 meutils/clis/README.md
 meutils/clis/__init__.py
 meutils/clis/cli.py
 meutils/clis/conf.py
 meutils/clis/cron.py
 meutils/clis/demo.py
 meutils/clis/gunicorn.conf.py
```

### Comparing `MeUtils-2023.7.6.9.18.40/MeUtils.egg-info/requires.txt` & `MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -23,47 +23,47 @@
 schedule
 
 [ai]
 faiss-gpu
 gensim
 
 [all]
-simplejson
-asyncmy
-polars
-pandas-profiling[notebook]
-seaborn
-faiss-gpu
-faiss-cpu
-fastapi[all]
-geopy
-streamlit
-cachetools
-schedule
 missingno
-iteration_utilities
-pretty_errors
-thefuck
-pymysql
-dataframe_image
-filetype
+gensim
 pandas_summary
-jmespath
 pymupd
-redis-py-cluster
-uvicorn
-pymilvus
-jieba
+fastapi[all]
+pretty_errors
 reportlab
-sqlalchemy
+iteration_utilities
+streamlit
+jmespath
+seaborn
+thriftpy2
+jieba
+redis-py-cluster
+polars
+pandas-profiling[notebook]
+cachetools
+asyncmy
+faiss-cpu
 pyarrow
+thefuck
+dataframe_image
+pymysql
 jinja2
+uvicorn
 pymongo
-thriftpy2
-gensim
+faiss-gpu
+filetype
+schedule
+sqlalchemy
+simplejson
+geopy
+pymilvus
 
 [ann]
 pymilvus
 faiss-cpu
 
 [app]
 fastapi[all]
```

### Comparing `MeUtils-2023.7.6.9.18.40/PKG-INFO` & `MeUtils-2023.7.7.15.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.7.6.9.18.40
+Version: 2023.7.7.15.3.6
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `MeUtils-2023.7.6.9.18.40/README.md` & `MeUtils-2023.7.7.15.3.6/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/clear_git_history.sh` & `MeUtils-2023.7.7.15.3.6/clear_git_history.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ai_audio/asr.py` & `MeUtils-2023.7.7.15.3.6/meutils/ai_audio/asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/SplitSentence.py` & `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/SplitSentence.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/Untitled-1(1).py` & `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/Untitled-1(1).py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/_lda.py` & `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py` & `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/_textsplitter/text_split.py` & `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/text_split.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/lda.py` & `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/ner.py` & `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/ner.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/sentence_transformers.py` & `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/textsplitter.py` & `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/textsplitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ai_nlp/word_segmentation.py` & `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ann/README.md` & `MeUtils-2023.7.7.15.3.6/meutils/ann/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ann/README_gensim.md` & `MeUtils-2023.7.7.15.3.6/meutils/ann/README_gensim.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ann/ann.py` & `MeUtils-2023.7.7.15.3.6/meutils/ann/ann.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ann/ann_faiss.py` & `MeUtils-2023.7.7.15.3.6/meutils/ann/ann_faiss.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ann/ann_gensim.py` & `MeUtils-2023.7.7.15.3.6/meutils/ann/ann_gensim.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ann/ann_inmemory.py` & `MeUtils-2023.7.7.15.3.6/meutils/ann/ann_inmemory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ann/ann_service.py` & `MeUtils-2023.7.7.15.3.6/meutils/ann/ann_service.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ann/ann_v1.py` & `MeUtils-2023.7.7.15.3.6/meutils/ann/ann_v1.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ann/cli.py` & `MeUtils-2023.7.7.15.3.6/meutils/ann/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ann/examples/client.py` & `MeUtils-2023.7.7.15.3.6/meutils/ann/examples/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/ann/shake_demo.py` & `MeUtils-2023.7.7.15.3.6/meutils/ann/shake_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/cache_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/cache_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # @File         : cache_utils
 # @Time         : 2021/11/24 上午11:09
 # @Author       : yuanjie
 # @WeChat       : 313303303
 # @Software     : PyCharm
 # @Description  : https://cachetools.readthedocs.io/en/stable/
 """
+异步缓存 from aiocache import cached
+
 FIFO：First In、First Out，就是先进先出。
 
 LFU：Least Frequently Used，就是淘汰最不常用的。
 
 LRU：Least Recently Used，就是淘汰最久不用的。
 
 MRU：Most Recently Used，与 LRU 相反，淘汰最近用的。
@@ -23,20 +25,24 @@
 """
 import sys
 import math
 import pickle
 import hashlib
 import numpy as np
 import pandas as pd
+import inspect
 import joblib
 
 from typing import Iterable
 from functools import lru_cache
 from pathlib import Path
 from joblib import Memory
+from joblib.func_inspect import filter_args
+from joblib import hashing  # hashing.hash
+
 from loguru import logger
 from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
 
 from tqdm.auto import tqdm
 from cachetools import cached, cachedmethod, LRUCache, RRCache, TTLCache as _TTLCache, keys
 
 # ME
@@ -98,34 +104,53 @@
 
         df = func(*args, **kwargs)
         df.to_sql(k, conn, if_exists='replace', index=False)
         return df
 
 
 @decorator
-def diskcache(func, location='cachedir', ttl=None, verbose=True, *args, **kwargs):
+def diskcache(func, location='cachedir', ttl=None, ignore=None, verbose=1, func_tag=None, *args, **kwargs):
     """
     https://zhuanlan.zhihu.com/p/356447502
     https://grantjenks.com/docs/diskcache/
+
     """
-    from diskcache import Cache
+    from diskcache import Cache, FanoutCache
+
     cache = Cache(directory=location)
 
-    key = md5(f"cache_{func.__name__}_{args}_{kwargs}")
+    raw_key = dict(filter_args(func, [], list(args), kwargs))
+
+    ignore = (ignore or []) + ['self', 'cls', 'api_base', 'api_key', 'organization', 'request_timeout']  # self 本身就不好被计入
+    if ignore:
+        raw_key = {**raw_key.pop('**', {}), **raw_key, '__tag__':  func_tag or func.__name__}
+        for arg in ignore:
+            raw_key.pop(arg, None)
+
+    key = hashing.hash(raw_key)
+
     if key in cache:
         _ = cache.get(key)
     else:
+        _ = func(*args, **kwargs)
+        if inspect.isgenerator(_):
+            _ = list(_)
+            cache.set(f"{key}_isgenerator", True, expire=ttl)
+
+        cache.set(key, _, expire=ttl)  # 异步写入
+
         if verbose:
             from loguru import logger
             logger = logger.patch(lambda r: r.update(name=func.__name__))
+            if verbose != 1:
+                key = raw_key
+
             logger.info(f"{cache.directory}: `CacheKey: {key}`")
 
-        _ = func(*args, **kwargs)
-        cache.set(key, _, expire=ttl)
-    return _
+    return _ if not cache.get(f"{key}_isgenerator") else iter(_)
 
 
 @decorator
 def disk_cache(func, location='cachedir', maxsize=128, ttl=np.inf, verbose=True, *args, **kwargs):
     ttl_cache = TTLCache(maxsize, ttl)  # 单例
 
     k = md5(f"cache_{func.__name__}_{args}_{kwargs}")  # uuid
```

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/clis/cli.py` & `MeUtils-2023.7.7.15.3.6/meutils/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/clis/conf.py` & `MeUtils-2023.7.7.15.3.6/meutils/clis/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/clis/cron.py` & `MeUtils-2023.7.7.15.3.6/meutils/clis/cron.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/clis/demo.py` & `MeUtils-2023.7.7.15.3.6/meutils/clis/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/clis/gunicorn.conf.py` & `MeUtils-2023.7.7.15.3.6/meutils/clis/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/clis/monitor.py` & `MeUtils-2023.7.7.15.3.6/meutils/clis/monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/clis/nesc.py` & `MeUtils-2023.7.7.15.3.6/meutils/clis/nesc.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/cmds/README.md` & `MeUtils-2023.7.7.15.3.6/meutils/cmds/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/cmds/hdfs_cmd.py` & `MeUtils-2023.7.7.15.3.6/meutils/cmds/hdfs_cmd.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/cmds/subprocess_demo.py` & `MeUtils-2023.7.7.15.3.6/meutils/cmds/subprocess_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/coding/find132.py` & `MeUtils-2023.7.7.15.3.6/meutils/coding/find132.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/common.py` & `MeUtils-2023.7.7.15.3.6/meutils/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,17 @@
     if isinstance(l, type):
         l = [l]
     return l
 
 
 def show_code(func):
     sourcelines, _ = inspect.getsourcelines(func)
-    return textwrap.dedent("".join(sourcelines))
+    _ = textwrap.dedent("".join(sourcelines))
+    print(_)
+    return _
 
 
 def file_replace(file, old, new):
     p = Path(file)
     _ = (
         p.read_text()
         .replace(old, new)
```

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/comp_utils/reverse_metric.py` & `MeUtils-2023.7.7.15.3.6/meutils/comp_utils/reverse_metric.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/data/SimHei.ttf` & `MeUtils-2023.7.7.15.3.6/meutils/data/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/data/coordinate.py` & `MeUtils-2023.7.7.15.3.6/meutils/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/date_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/date_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/db/README.md` & `MeUtils-2023.7.7.15.3.6/meutils/db/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/db/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/db/mongo.py` & `MeUtils-2023.7.7.15.3.6/meutils/db/mongo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/db/neo4j.py` & `MeUtils-2023.7.7.15.3.6/meutils/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/decorators/__ai.py` & `MeUtils-2023.7.7.15.3.6/meutils/decorators/__ai.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/decorators/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/decorators/catch.py` & `MeUtils-2023.7.7.15.3.6/meutils/decorators/catch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/decorators/common.py` & `MeUtils-2023.7.7.15.3.6/meutils/decorators/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/decorators/decorator.py` & `MeUtils-2023.7.7.15.3.6/meutils/decorators/decorator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/decorators/decorator_demo.py` & `MeUtils-2023.7.7.15.3.6/meutils/decorators/decorator_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/decorators/demo.py` & `MeUtils-2023.7.7.15.3.6/meutils/decorators/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/decorators/feishu.py` & `MeUtils-2023.7.7.15.3.6/meutils/decorators/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/decorators/retry.py` & `MeUtils-2023.7.7.15.3.6/meutils/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/decorators/scheduler.py` & `MeUtils-2023.7.7.15.3.6/meutils/decorators/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/dist_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/docarray_utils/demo_es.py` & `MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/demo_es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/docarray_utils/demo_hnsw.py` & `MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/demo_hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/docarray_utils/in_memory.py` & `MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/in_memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/docarray_utils/改造下hnsw.py` & `MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/改造下hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/easy_search/es.py` & `MeUtils-2023.7.7.15.3.6/meutils/easy_search/es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/fileparser/PDF抽取.py` & `MeUtils-2023.7.7.15.3.6/meutils/fileparser/PDF抽取.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/hash_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/import_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/import_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/init/evn.py` & `MeUtils-2023.7.7.15.3.6/meutils/init/evn.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/init/oo.py` & `MeUtils-2023.7.7.15.3.6/meutils/init/oo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/io/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/io/image.py` & `MeUtils-2023.7.7.15.3.6/meutils/io/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/io/tf_io.py` & `MeUtils-2023.7.7.15.3.6/meutils/io/tf_io.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/jinja_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/log_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/notice/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/notice/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/notice/emails.py` & `MeUtils-2023.7.7.15.3.6/meutils/notice/emails.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/notice/feishu.py` & `MeUtils-2023.7.7.15.3.6/meutils/notice/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/notice/file_post.py` & `MeUtils-2023.7.7.15.3.6/meutils/notice/file_post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/notice/wechat.py` & `MeUtils-2023.7.7.15.3.6/meutils/notice/wechat.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/notice/wechat_.py` & `MeUtils-2023.7.7.15.3.6/meutils/notice/wechat_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/notice/wecom.py` & `MeUtils-2023.7.7.15.3.6/meutils/notice/wecom.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/notice/weekmeet.py` & `MeUtils-2023.7.7.15.3.6/meutils/notice/weekmeet.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/np_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/np_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/office_automation/pdf.py` & `MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/office_automation/pdm.py` & `MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdm.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/office_automation/pdm_run.py` & `MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdm_run.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/office_automation/投资管理系统O3.2_交易组.pdm` & `MeUtils-2023.7.7.15.3.6/meutils/office_automation/投资管理系统O3.2_交易组.pdm`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/__demo.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/__demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/aiomultiprocess/core.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/core.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/aiomultiprocess/pool.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/pool.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/aiomultiprocess/scheduler.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/aiomultiprocess/types.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/besttable.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/besttable.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/crontab.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/crontab.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/annlite.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/annlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/base.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/chunk.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/chunk.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/document.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/document.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/elastic.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/elastic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/match.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/memory.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/milvus.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/milvus.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/content.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/dataloader/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/dataloader/helper.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/dataloader/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/delitem.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/delitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/embed.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/embed.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/empty.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/empty.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/evaluation.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/find.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/getattr.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/getattr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/getitem.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/getitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/group.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/group.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/binary.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/binary.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/common.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/csv.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/csv.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/dataframe.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/dataframe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/from_gen.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/from_gen.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/json.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/json.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/pbar.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/pbar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/io/pushpull.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/pushpull.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/match.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/parallel.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/parallel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/plot.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/post.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/pydantic.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/reduce.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/reduce.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/sample.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/sample.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/setitem.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/setitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/strawberry.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/text.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/mixins/traverse.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/traverse.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/opensearch.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/opensearch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/qdrant.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/qdrant.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/queryset/lookup.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/lookup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/queryset/parser.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/parser.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/redis.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/redis.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/sqlite.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/sqlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/backend.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/find.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/getsetdel.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/helper.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/annlite/seqlike.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/base/backend.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/base/getsetdel.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/base/helper.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/base/seqlike.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/elastic/backend.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/elastic/find.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/elastic/getsetdel.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/elastic/seqlike.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/memory/backend.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/memory/find.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/memory/getsetdel.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/memory/seqlike.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/milvus/backend.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/milvus/find.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/milvus/getsetdel.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/milvus/seqlike.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/opensearch/backend.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/opensearch/find.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/opensearch/getsetdel.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/opensearch/seqlike.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/backend.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/find.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/getsetdel.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/qdrant/seqlike.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/redis/backend.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/redis/find.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/redis/getsetdel.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/redis/seqlike.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/sqlite/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/sqlite/backend.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/sqlite/getsetdel.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/sqlite/helper.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/sqlite/seqlike.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/weaviate/backend.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/weaviate/find.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/weaviate/getsetdel.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/storage/weaviate/seqlike.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/array/weaviate.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/weaviate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/base.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/dataclasses/enums.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/enums.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/dataclasses/getter.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/getter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/dataclasses/setter.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/setter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/dataclasses/types.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/data.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/generators.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/generators.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/_property.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/_property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/attribute.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/attribute.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/audio.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/audio.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/blob.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/blob.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/content.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/convert.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/dump.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/dump.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/featurehash.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/featurehash.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/helper.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/image.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/mesh.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/mesh.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/multimodal.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/multimodal.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/plot.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/porting.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/porting.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/property.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/protobuf.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/protobuf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/pydantic.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/rich_embedding.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/rich_embedding.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/strawberry.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/sugar.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/sugar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/text.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/mixins/video.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/pydantic_model.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/document/strawberry_type.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/strawberry_type.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/helper.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/distance/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/distance/numpy.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/numpy.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/distance/paddle.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/paddle.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/distance/tensorflow.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/tensorflow.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/distance/torch.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/torch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/evaluation.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/helper.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/math/ndarray.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/io/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/io/ndarray.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/io/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/pb/docarray_pb2.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/proto/pb2/docarray_pb2.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb2/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/resources/ci-vendors.json` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/ci-vendors.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/resources/embedding-projector/index.html.gz` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/embedding-projector/index.html.gz`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/score/data.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/score/mixins/property.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/other/docarray/typing/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/pandas_utils/opt.py` & `MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/opt.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/pandas_utils/pd_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/path_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/path_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/pd_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/pipe.py` & `MeUtils-2023.7.7.15.3.6/meutils/pipe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/plot_utils/demo.py` & `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/plot_utils/echarts.py` & `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/echarts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/plot_utils/embedding_plot.py` & `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/embedding_plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/plot_utils/mecharts.py` & `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/mecharts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/plot_utils/metrics.py` & `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/plot_utils/plot_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/request_utils/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/request_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/request_utils/crawler.py` & `MeUtils-2023.7.7.15.3.6/meutils/request_utils/crawler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/request_utils/download.py` & `MeUtils-2023.7.7.15.3.6/meutils/request_utils/download.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/request_utils/results.py` & `MeUtils-2023.7.7.15.3.6/meutils/request_utils/results.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/request_utils/公网ip.py` & `MeUtils-2023.7.7.15.3.6/meutils/request_utils/公网ip.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/_fastapi.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/_fastapi.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/__demo/异步任务.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/__demo/异步任务.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/common.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/fastapi/errors/validation_error.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/gui/bar.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/gui/bar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/gui/demo.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/gui/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/jina/__demo/client.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/jina/__demo/flow.svg` & `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/flow.svg`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/jina/__demo/server.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/server.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/jina/executors/SentenceEncoder.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/executors/SentenceEncoder.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/jina/executors/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/jina/nlp_serving/word_segmentation.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/nlp_serving/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/st_utils/_test.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/_test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/st_utils/common.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/webui/.streamlit/_config.toml` & `MeUtils-2023.7.7.15.3.6/meutils/serving/webui/.streamlit/_config.toml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/webui/_2_词性标注与实体识别.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/webui/_2_词性标注与实体识别.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/webui/pages/_1_分词.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_1_分词.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/webui/pages/_2_词性标注与实体识别.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_2_词性标注与实体识别.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/serving/webui/pages/_3_文本匹配.py` & `MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_3_文本匹配.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/sftp.py` & `MeUtils-2023.7.7.15.3.6/meutils/sftp.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/sk_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/sk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/smooth_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/smooth_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/spark/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/str_utils/Translator.py` & `MeUtils-2023.7.7.15.3.6/meutils/str_utils/Translator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/str_utils/__init__.py` & `MeUtils-2023.7.7.15.3.6/meutils/str_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/str_utils/__translater/tencent.py` & `MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/tencent.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/str_utils/__translater/translater.py` & `MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/translater.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/str_utils/__translater/youdao.py` & `MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/youdao.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/str_utils/json_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/str_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/str_utils/regular_expression.py` & `MeUtils-2023.7.7.15.3.6/meutils/str_utils/regular_expression.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/demo.j2` & `MeUtils-2023.7.7.15.3.6/meutils/templates/demo.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/demo.py` & `MeUtils-2023.7.7.15.3.6/meutils/templates/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/demox.py` & `MeUtils-2023.7.7.15.3.6/meutils/templates/demox.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/df_html.j2` & `MeUtils-2023.7.7.15.3.6/meutils/templates/df_html.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/dockerfiles/docker_build_push.py` & `MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/docker_build_push.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/hegui.py` & `MeUtils-2023.7.7.15.3.6/meutils/templates/hegui.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/markmap.html` & `MeUtils-2023.7.7.15.3.6/meutils/templates/markmap.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/cookiecutter.json` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py` & `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/tpl.docx` & `MeUtils-2023.7.7.15.3.6/meutils/templates/tpl.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/x.html` & `MeUtils-2023.7.7.15.3.6/meutils/templates/x.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/templates/合规日报模板.docx` & `MeUtils-2023.7.7.15.3.6/meutils/templates/合规日报模板.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/todo.py` & `MeUtils-2023.7.7.15.3.6/meutils/todo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/tools/cprint.py` & `MeUtils-2023.7.7.15.3.6/meutils/tools/cprint.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/tools/machine_monitor.py` & `MeUtils-2023.7.7.15.3.6/meutils/tools/machine_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/tools/monitor.yml` & `MeUtils-2023.7.7.15.3.6/meutils/tools/monitor.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/tools/seize.py` & `MeUtils-2023.7.7.15.3.6/meutils/tools/seize.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/tools/service_monitor.py` & `MeUtils-2023.7.7.15.3.6/meutils/tools/service_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/meutils/zk_utils.py` & `MeUtils-2023.7.7.15.3.6/meutils/zk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/pypi.sh` & `MeUtils-2023.7.7.15.3.6/pypi.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.6.9.18.40/setup.py` & `MeUtils-2023.7.7.15.3.6/setup.py`

 * *Files identical despite different names*


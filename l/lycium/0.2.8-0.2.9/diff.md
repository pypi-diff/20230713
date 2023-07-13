# Comparing `tmp/lycium-0.2.8.tar.gz` & `tmp/lycium-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lycium-0.2.8.tar", last modified: Fri Sep 23 03:51:05 2022, max compression
+gzip compressed data, was "dist/lycium-0.2.9.tar", last modified: Mon Sep 26 02:18:54 2022, max compression
```

## Comparing `lycium-0.2.8.tar` & `lycium-0.2.9.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:05.977028 lycium-0.2.8/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1073 2021-02-09 06:56:24.000000 lycium-0.2.8/LICENCE
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1356 2022-09-23 03:51:05.975022 lycium-0.2.8/PKG-INFO
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      909 2021-02-09 06:56:24.000000 lycium-0.2.8/README.md
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:04.125510 lycium-0.2.8/lycium/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)       46 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    11031 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/accesscontrol.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    48173 2022-08-04 13:47:40.000000 lycium-0.2.8/lycium/amqplib.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     7685 2021-10-06 08:50:29.000000 lycium-0.2.8/lycium/asynchttphandler.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    11619 2022-09-15 04:07:23.000000 lycium-0.2.8/lycium/asyncrequest.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1115 2021-06-04 14:17:50.000000 lycium-0.2.8/lycium/behaviors.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    12464 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/cacheproxy.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    70270 2022-09-23 03:44:00.000000 lycium-0.2.8/lycium/dbproxy.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     6816 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/elasticsearchsaver.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4782 2021-06-04 07:20:33.000000 lycium-0.2.8/lycium/exceptionreporter.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1437 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/guniapp.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:04.503922 lycium-0.2.8/lycium/kafka/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)       46 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/kafka/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      985 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/kafka/asyncWrapper.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1420 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/kafka/client.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     8824 2021-12-04 01:49:59.000000 lycium-0.2.8/lycium/kafka/consumerHelper.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      141 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/kafka/debugSet.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2485 2021-03-25 10:23:58.000000 lycium-0.2.8/lycium/kafka/helper.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    13547 2021-12-04 01:49:59.000000 lycium-0.2.8/lycium/kafka/kafkaWorker.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     5980 2021-12-04 01:49:59.000000 lycium-0.2.8/lycium/kafka/producerHelper.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:04.563788 lycium-0.2.8/lycium/kafka/protocol/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/kafka/protocol/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    12177 2021-04-13 08:00:06.000000 lycium-0.2.8/lycium/kafka/protocol/kafkapacket_pb2.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3748 2021-04-13 08:00:06.000000 lycium-0.2.8/lycium/kafka/publishesMessage.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      539 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/kafka/server.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3093 2021-05-07 08:29:45.000000 lycium-0.2.8/lycium/kafka/workerDelegate.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:04.704419 lycium-0.2.8/lycium/microsvc/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2021-04-12 09:36:20.000000 lycium-0.2.8/lycium/microsvc/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3075 2021-04-12 09:56:24.000000 lycium-0.2.8/lycium/microsvc/applicationServer.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2548 2021-05-07 08:29:45.000000 lycium-0.2.8/lycium/microsvc/context.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:04.834964 lycium-0.2.8/lycium/microsvc/middlewares/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2021-04-12 09:36:20.000000 lycium-0.2.8/lycium/microsvc/middlewares/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      639 2021-05-07 08:29:45.000000 lycium-0.2.8/lycium/microsvc/middlewares/exceptionMiddleware.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      328 2021-05-07 08:29:45.000000 lycium-0.2.8/lycium/microsvc/middlewares/logMiddleware.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      503 2021-05-07 08:29:45.000000 lycium-0.2.8/lycium/microsvc/middlewares/websocketPackageMiddleware.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:04.913073 lycium-0.2.8/lycium/microsvc/protocol/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2021-04-12 09:36:20.000000 lycium-0.2.8/lycium/microsvc/protocol/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    29303 2021-04-12 09:36:20.000000 lycium-0.2.8/lycium/microsvc/protocol/packagewrapper_pb2.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3209 2021-05-07 08:29:45.000000 lycium-0.2.8/lycium/microsvc/router.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2128 2021-05-07 08:29:45.000000 lycium-0.2.8/lycium/microsvc/utils.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3502 2021-10-02 17:00:32.000000 lycium-0.2.8/lycium/modelutils.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)       52 2022-09-19 09:29:55.000000 lycium-0.2.8/lycium/mq.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1226 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/registerroute.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      302 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/singleton.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:04.928731 lycium-0.2.8/lycium/sqlalchemy_dialects/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)       29 2021-09-26 18:59:38.000000 lycium-0.2.8/lycium/sqlalchemy_dialects/__init__.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:04.959950 lycium-0.2.8/lycium/sqlalchemy_dialects/asyncpg_migrate/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4519 2021-09-29 15:10:21.000000 lycium-0.2.8/lycium/sqlalchemy_dialects/asyncpg_migrate/__init__.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:05.100606 lycium-0.2.8/lycium/sqlalchemy_dialects/sync_threading/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)       86 2021-10-05 04:05:33.000000 lycium-0.2.8/lycium/sqlalchemy_dialects/sync_threading/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3392 2021-10-06 07:18:29.000000 lycium-0.2.8/lycium/sqlalchemy_dialects/sync_threading/asyncio.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    23405 2021-10-05 06:48:26.000000 lycium-0.2.8/lycium/sqlalchemy_dialects/sync_threading/base.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      800 2021-10-05 03:36:36.000000 lycium-0.2.8/lycium/sqlalchemy_dialects/sync_threading/exc.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      542 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/supports.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:05.147720 lycium-0.2.8/lycium/tornadoadapts/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)       47 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/tornadoadapts/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      147 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/tornadoadapts/stack_context.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:05.225824 lycium-0.2.8/lycium/tornadozeep/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)       65 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/tornadozeep/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      755 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/tornadozeep/bindings.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4601 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/tornadozeep/transport.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:05.631668 lycium-0.2.8/lycium/utilities/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3360 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1237 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/aescoder.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1126 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/descoder.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      288 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/fileutil.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4640 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/htmldocutils.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1000 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/img_utils.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      638 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/iplist.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4020 2021-08-10 16:05:46.000000 lycium-0.2.8/lycium/utilities/notifydata_utils.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      400 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/orderutil.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1236 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/restful_api.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      610 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/rsacoder.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4429 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/signatureutils.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      638 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/timeutil.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2721 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/work.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2845 2021-02-09 06:56:24.000000 lycium-0.2.8/lycium/utilities/xmlutil.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      434 2021-06-02 06:52:16.000000 lycium-0.2.8/lycium/webapplication.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:04.203656 lycium-0.2.8/lycium.egg-info/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1356 2022-09-23 03:51:02.000000 lycium-0.2.8/lycium.egg-info/PKG-INFO
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2604 2022-09-23 03:51:03.000000 lycium-0.2.8/lycium.egg-info/SOURCES.txt
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)        1 2022-09-23 03:51:02.000000 lycium-0.2.8/lycium.egg-info/dependency_links.txt
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      241 2022-09-23 03:51:02.000000 lycium-0.2.8/lycium.egg-info/requires.txt
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)        7 2022-09-23 03:51:02.000000 lycium-0.2.8/lycium.egg-info/top_level.txt
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)       38 2022-09-23 03:51:05.978029 lycium-0.2.8/setup.cfg
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1260 2022-09-15 04:08:41.000000 lycium-0.2.8/setup.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-23 03:51:05.958022 lycium-0.2.8/tests/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2021-02-09 06:56:24.000000 lycium-0.2.8/tests/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1774 2021-10-06 07:58:40.000000 lycium-0.2.8/tests/builtin_dbconfig.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    19243 2021-10-06 08:00:33.000000 lycium-0.2.8/tests/dbunittest.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2417 2022-01-20 18:56:26.000000 lycium-0.2.8/tests/local_dbconfig.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2165 2021-10-06 08:04:39.000000 lycium-0.2.8/tests/local_dbtest.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     9400 2021-10-06 08:43:23.000000 lycium-0.2.8/tests/local_mongotest.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1225 2021-10-06 08:03:18.000000 lycium-0.2.8/tests/local_test_consume_queue.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      893 2021-04-12 10:36:14.000000 lycium-0.2.8/tests/microsvcdemo.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1514 2021-09-23 13:42:59.000000 lycium-0.2.8/tests/soapdemo.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1908 2022-08-04 13:35:57.000000 lycium-0.2.8/tests/testamqpfanout.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2448 2021-09-03 10:23:38.000000 lycium-0.2.8/tests/testamqprpc.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      837 2022-09-22 09:07:16.000000 lycium-0.2.8/tests/testentry.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1877 2022-01-19 02:46:01.000000 lycium-0.2.8/tests/testhttpclient.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      696 2021-02-09 06:56:24.000000 lycium-0.2.8/tests/testreporter.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      943 2021-10-06 08:56:56.000000 lycium-0.2.8/tests/testrestconcurrency.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:53.059345 lycium-0.2.9/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1073 2021-02-09 06:56:24.000000 lycium-0.2.9/LICENCE
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1356 2022-09-26 02:18:53.043718 lycium-0.2.9/PKG-INFO
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      909 2021-02-09 06:56:24.000000 lycium-0.2.9/README.md
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:51.493899 lycium-0.2.9/lycium/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)       46 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    11031 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/accesscontrol.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    48173 2022-08-04 13:47:40.000000 lycium-0.2.9/lycium/amqplib.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     7685 2021-10-06 08:50:29.000000 lycium-0.2.9/lycium/asynchttphandler.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    11619 2022-09-15 04:07:23.000000 lycium-0.2.9/lycium/asyncrequest.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1115 2021-06-04 14:17:50.000000 lycium-0.2.9/lycium/behaviors.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    12464 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/cacheproxy.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    70374 2022-09-26 02:13:31.000000 lycium-0.2.9/lycium/dbproxy.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     6816 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/elasticsearchsaver.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4782 2021-06-04 07:20:33.000000 lycium-0.2.9/lycium/exceptionreporter.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1437 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/guniapp.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:51.807898 lycium-0.2.9/lycium/kafka/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)       46 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/kafka/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      985 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/kafka/asyncWrapper.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1420 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/kafka/client.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     8824 2021-12-04 01:49:59.000000 lycium-0.2.9/lycium/kafka/consumerHelper.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      141 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/kafka/debugSet.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2485 2021-03-25 10:23:58.000000 lycium-0.2.9/lycium/kafka/helper.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    13547 2021-12-04 01:49:59.000000 lycium-0.2.9/lycium/kafka/kafkaWorker.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     5980 2021-12-04 01:49:59.000000 lycium-0.2.9/lycium/kafka/producerHelper.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:51.853586 lycium-0.2.9/lycium/kafka/protocol/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/kafka/protocol/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    12177 2021-04-13 08:00:06.000000 lycium-0.2.9/lycium/kafka/protocol/kafkapacket_pb2.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3748 2021-04-13 08:00:06.000000 lycium-0.2.9/lycium/kafka/publishesMessage.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      539 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/kafka/server.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3093 2021-05-07 08:29:45.000000 lycium-0.2.9/lycium/kafka/workerDelegate.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:51.978594 lycium-0.2.9/lycium/microsvc/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2021-04-12 09:36:20.000000 lycium-0.2.9/lycium/microsvc/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3075 2021-04-12 09:56:24.000000 lycium-0.2.9/lycium/microsvc/applicationServer.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2548 2021-05-07 08:29:45.000000 lycium-0.2.9/lycium/microsvc/context.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:52.087966 lycium-0.2.9/lycium/microsvc/middlewares/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2021-04-12 09:36:20.000000 lycium-0.2.9/lycium/microsvc/middlewares/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      639 2021-05-07 08:29:45.000000 lycium-0.2.9/lycium/microsvc/middlewares/exceptionMiddleware.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      328 2021-05-07 08:29:45.000000 lycium-0.2.9/lycium/microsvc/middlewares/logMiddleware.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      503 2021-05-07 08:29:45.000000 lycium-0.2.9/lycium/microsvc/middlewares/websocketPackageMiddleware.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:52.134836 lycium-0.2.9/lycium/microsvc/protocol/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2021-04-12 09:36:20.000000 lycium-0.2.9/lycium/microsvc/protocol/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    29303 2021-04-12 09:36:20.000000 lycium-0.2.9/lycium/microsvc/protocol/packagewrapper_pb2.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3209 2021-05-07 08:29:45.000000 lycium-0.2.9/lycium/microsvc/router.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2128 2021-05-07 08:29:45.000000 lycium-0.2.9/lycium/microsvc/utils.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3502 2021-10-02 17:00:32.000000 lycium-0.2.9/lycium/modelutils.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)       52 2022-09-19 09:29:55.000000 lycium-0.2.9/lycium/mq.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1226 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/registerroute.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      302 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/singleton.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:52.166085 lycium-0.2.9/lycium/sqlalchemy_dialects/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)       29 2021-09-26 18:59:38.000000 lycium-0.2.9/lycium/sqlalchemy_dialects/__init__.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:52.197334 lycium-0.2.9/lycium/sqlalchemy_dialects/asyncpg_migrate/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4519 2021-09-29 15:10:21.000000 lycium-0.2.9/lycium/sqlalchemy_dialects/asyncpg_migrate/__init__.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:52.306710 lycium-0.2.9/lycium/sqlalchemy_dialects/sync_threading/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)       86 2021-10-05 04:05:33.000000 lycium-0.2.9/lycium/sqlalchemy_dialects/sync_threading/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3392 2021-10-06 07:18:29.000000 lycium-0.2.9/lycium/sqlalchemy_dialects/sync_threading/asyncio.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    23405 2021-10-05 06:48:26.000000 lycium-0.2.9/lycium/sqlalchemy_dialects/sync_threading/base.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      800 2021-10-05 03:36:36.000000 lycium-0.2.9/lycium/sqlalchemy_dialects/sync_threading/exc.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      542 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/supports.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:52.353585 lycium-0.2.9/lycium/tornadoadapts/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)       47 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/tornadoadapts/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      147 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/tornadoadapts/stack_context.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:52.431715 lycium-0.2.9/lycium/tornadozeep/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)       65 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/tornadozeep/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      755 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/tornadozeep/bindings.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4601 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/tornadozeep/transport.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:52.791346 lycium-0.2.9/lycium/utilities/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3360 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1237 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/aescoder.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1126 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/descoder.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      288 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/fileutil.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4640 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/htmldocutils.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1000 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/img_utils.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      638 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/iplist.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4020 2021-08-10 16:05:46.000000 lycium-0.2.9/lycium/utilities/notifydata_utils.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      400 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/orderutil.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1236 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/restful_api.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      610 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/rsacoder.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     4429 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/signatureutils.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      638 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/timeutil.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2721 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/work.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2845 2021-02-09 06:56:24.000000 lycium-0.2.9/lycium/utilities/xmlutil.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      434 2021-06-02 06:52:16.000000 lycium-0.2.9/lycium/webapplication.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:51.578920 lycium-0.2.9/lycium.egg-info/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1356 2022-09-26 02:18:50.000000 lycium-0.2.9/lycium.egg-info/PKG-INFO
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2604 2022-09-26 02:18:50.000000 lycium-0.2.9/lycium.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)        1 2022-09-26 02:18:50.000000 lycium-0.2.9/lycium.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      241 2022-09-26 02:18:50.000000 lycium-0.2.9/lycium.egg-info/requires.txt
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)        7 2022-09-26 02:18:50.000000 lycium-0.2.9/lycium.egg-info/top_level.txt
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)       38 2022-09-26 02:18:53.059345 lycium-0.2.9/setup.cfg
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1260 2022-09-26 02:17:39.000000 lycium-0.2.9/setup.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-09-26 02:18:53.028096 lycium-0.2.9/tests/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2021-02-09 06:56:24.000000 lycium-0.2.9/tests/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1774 2021-10-06 07:58:40.000000 lycium-0.2.9/tests/builtin_dbconfig.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    19243 2021-10-06 08:00:33.000000 lycium-0.2.9/tests/dbunittest.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2417 2022-01-20 18:56:26.000000 lycium-0.2.9/tests/local_dbconfig.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2165 2021-10-06 08:04:39.000000 lycium-0.2.9/tests/local_dbtest.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     9400 2021-10-06 08:43:23.000000 lycium-0.2.9/tests/local_mongotest.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1225 2021-10-06 08:03:18.000000 lycium-0.2.9/tests/local_test_consume_queue.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      893 2021-04-12 10:36:14.000000 lycium-0.2.9/tests/microsvcdemo.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1514 2021-09-23 13:42:59.000000 lycium-0.2.9/tests/soapdemo.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1908 2022-08-04 13:35:57.000000 lycium-0.2.9/tests/testamqpfanout.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2448 2021-09-03 10:23:38.000000 lycium-0.2.9/tests/testamqprpc.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      837 2022-09-22 09:07:16.000000 lycium-0.2.9/tests/testentry.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1877 2022-01-19 02:46:01.000000 lycium-0.2.9/tests/testhttpclient.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      696 2021-02-09 06:56:24.000000 lycium-0.2.9/tests/testreporter.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      943 2021-10-06 08:56:56.000000 lycium-0.2.9/tests/testrestconcurrency.py
```

### Comparing `lycium-0.2.8/LICENCE` & `lycium-0.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/PKG-INFO` & `lycium-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lycium
-Version: 0.2.8
+Version: 0.2.9
 Summary: Common python package
 Home-page: https://gitee.com/starview/lycium
 Author: kevinyjn
 Author-email: kevinyjn@foxmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lycium-0.2.8/README.md` & `lycium-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/accesscontrol.py` & `lycium-0.2.9/lycium/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/amqplib.py` & `lycium-0.2.9/lycium/amqplib.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/asynchttphandler.py` & `lycium-0.2.9/lycium/asynchttphandler.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/asyncrequest.py` & `lycium-0.2.9/lycium/asyncrequest.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/behaviors.py` & `lycium-0.2.9/lycium/behaviors.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/cacheproxy.py` & `lycium-0.2.9/lycium/cacheproxy.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/dbproxy.py` & `lycium-0.2.9/lycium/dbproxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,19 +267,20 @@
                 # 'timeout': 15
             }
         }
         if 'sqlite' == engine:
             del create_engine_params['pool_timeout']
             del create_engine_params['pool_size']
         if 'connect_args' in dbconf:
-            connect_args = dbconf['connect_args'] 
-            if 'pool_size' in connect_args:
-                create_engine_params['pool_size'] = int(connect_args['pool_size'])
-                del connect_args['pool_size']
-                dbconf['connect_args'] = connect_args
+            connect_args = dbconf['connect_args']
+            for custom_key in ['pool_size', 'pool_timeout', 'pool_recycle', 'max_overflow']:
+                if custom_key in connect_args:
+                    create_engine_params[custom_key] = int(connect_args[custom_key])
+                    del connect_args[custom_key]
+                    dbconf['connect_args'] = connect_args
             if not isinstance(connect_args, dict):
                 s1 = str(connect_args).split('&')
                 connect_args = {}
                 for s2 in s1:
                     s3 = s2.split('=')
                     if len(s3) > 1:
                         connect_args[s3[0].strip()] = s3[1].strip()
```

### Comparing `lycium-0.2.8/lycium/elasticsearchsaver.py` & `lycium-0.2.9/lycium/elasticsearchsaver.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/exceptionreporter.py` & `lycium-0.2.9/lycium/exceptionreporter.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/guniapp.py` & `lycium-0.2.9/lycium/guniapp.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/kafka/asyncWrapper.py` & `lycium-0.2.9/lycium/kafka/asyncWrapper.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/kafka/client.py` & `lycium-0.2.9/lycium/kafka/client.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/kafka/consumerHelper.py` & `lycium-0.2.9/lycium/kafka/consumerHelper.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/kafka/helper.py` & `lycium-0.2.9/lycium/kafka/helper.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/kafka/kafkaWorker.py` & `lycium-0.2.9/lycium/kafka/kafkaWorker.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/kafka/producerHelper.py` & `lycium-0.2.9/lycium/kafka/producerHelper.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/kafka/protocol/kafkapacket_pb2.py` & `lycium-0.2.9/lycium/kafka/protocol/kafkapacket_pb2.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/kafka/publishesMessage.py` & `lycium-0.2.9/lycium/kafka/publishesMessage.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/kafka/server.py` & `lycium-0.2.9/lycium/kafka/server.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/kafka/workerDelegate.py` & `lycium-0.2.9/lycium/kafka/workerDelegate.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/microsvc/applicationServer.py` & `lycium-0.2.9/lycium/microsvc/applicationServer.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/microsvc/context.py` & `lycium-0.2.9/lycium/microsvc/context.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/microsvc/middlewares/exceptionMiddleware.py` & `lycium-0.2.9/lycium/microsvc/middlewares/exceptionMiddleware.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/microsvc/protocol/packagewrapper_pb2.py` & `lycium-0.2.9/lycium/microsvc/protocol/packagewrapper_pb2.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/microsvc/router.py` & `lycium-0.2.9/lycium/microsvc/router.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/microsvc/utils.py` & `lycium-0.2.9/lycium/microsvc/utils.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/modelutils.py` & `lycium-0.2.9/lycium/modelutils.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/registerroute.py` & `lycium-0.2.9/lycium/registerroute.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/sqlalchemy_dialects/asyncpg_migrate/__init__.py` & `lycium-0.2.9/lycium/sqlalchemy_dialects/asyncpg_migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/sqlalchemy_dialects/sync_threading/asyncio.py` & `lycium-0.2.9/lycium/sqlalchemy_dialects/sync_threading/asyncio.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/sqlalchemy_dialects/sync_threading/base.py` & `lycium-0.2.9/lycium/sqlalchemy_dialects/sync_threading/base.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/sqlalchemy_dialects/sync_threading/exc.py` & `lycium-0.2.9/lycium/sqlalchemy_dialects/sync_threading/exc.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/supports.py` & `lycium-0.2.9/lycium/supports.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/tornadozeep/bindings.py` & `lycium-0.2.9/lycium/tornadozeep/bindings.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/tornadozeep/transport.py` & `lycium-0.2.9/lycium/tornadozeep/transport.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/__init__.py` & `lycium-0.2.9/lycium/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/aescoder.py` & `lycium-0.2.9/lycium/utilities/aescoder.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/descoder.py` & `lycium-0.2.9/lycium/utilities/descoder.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/htmldocutils.py` & `lycium-0.2.9/lycium/utilities/htmldocutils.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/img_utils.py` & `lycium-0.2.9/lycium/utilities/img_utils.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/iplist.py` & `lycium-0.2.9/lycium/utilities/iplist.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/notifydata_utils.py` & `lycium-0.2.9/lycium/utilities/notifydata_utils.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/restful_api.py` & `lycium-0.2.9/lycium/utilities/restful_api.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/rsacoder.py` & `lycium-0.2.9/lycium/utilities/rsacoder.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/signatureutils.py` & `lycium-0.2.9/lycium/utilities/signatureutils.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/timeutil.py` & `lycium-0.2.9/lycium/utilities/timeutil.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/work.py` & `lycium-0.2.9/lycium/utilities/work.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium/utilities/xmlutil.py` & `lycium-0.2.9/lycium/utilities/xmlutil.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/lycium.egg-info/PKG-INFO` & `lycium-0.2.9/lycium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lycium
-Version: 0.2.8
+Version: 0.2.9
 Summary: Common python package
 Home-page: https://gitee.com/starview/lycium
 Author: kevinyjn
 Author-email: kevinyjn@foxmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lycium-0.2.8/lycium.egg-info/SOURCES.txt` & `lycium-0.2.9/lycium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/setup.py` & `lycium-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lycium",
-    version="0.2.8",
+    version="0.2.9",
     author="kevinyjn",
     author_email="kevinyjn@foxmail.com",
     description="Common python package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/starview/lycium",
     packages=setuptools.find_packages(exclude=[".tests", ".tests.", "tests.*", "tests"]),
```

### Comparing `lycium-0.2.8/tests/builtin_dbconfig.py` & `lycium-0.2.9/tests/builtin_dbconfig.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/dbunittest.py` & `lycium-0.2.9/tests/dbunittest.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/local_dbconfig.py` & `lycium-0.2.9/tests/local_dbconfig.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/local_dbtest.py` & `lycium-0.2.9/tests/local_dbtest.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/local_mongotest.py` & `lycium-0.2.9/tests/local_mongotest.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/local_test_consume_queue.py` & `lycium-0.2.9/tests/local_test_consume_queue.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/microsvcdemo.py` & `lycium-0.2.9/tests/microsvcdemo.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/soapdemo.py` & `lycium-0.2.9/tests/soapdemo.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/testamqpfanout.py` & `lycium-0.2.9/tests/testamqpfanout.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/testamqprpc.py` & `lycium-0.2.9/tests/testamqprpc.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/testentry.py` & `lycium-0.2.9/tests/testentry.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/testhttpclient.py` & `lycium-0.2.9/tests/testhttpclient.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/testreporter.py` & `lycium-0.2.9/tests/testreporter.py`

 * *Files identical despite different names*

### Comparing `lycium-0.2.8/tests/testrestconcurrency.py` & `lycium-0.2.9/tests/testrestconcurrency.py`

 * *Files identical despite different names*


# Comparing `tmp/propan-0.1.5.7.tar.gz` & `tmp/propan-0.1.5.8.tar.gz`

## Comparing `propan-0.1.5.7.tar` & `propan-0.1.5.8.tar`

### file list

```diff
@@ -1,191 +1,192 @@
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 propan-0.1.5.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.5.7/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.5.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.5.7/.github/dependantbot.yml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.5.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.5.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 propan-0.1.5.7/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.5.7/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.5.7/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 propan-0.1.5.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/redis/pattern.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/scheduling/rocketry.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/serialization/gen_py_code.sh
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/serialization/message.proto
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/serialization/protobuf.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/serialization/requirements.txt
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.5.7/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/__about__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/__main__.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/_compat.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/py.typed
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/security.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/constants.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/exceptions.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/middlewares.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    21080 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/_model/routing.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    14111 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     9016 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/kafka/routing.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/kafka/routing.pyi
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/nats/consts.py
--rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0    11462 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0     8331 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/nats/nats_js_broker.pyi
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/nats/routing.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/nats/routing.pyi
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/rabbit/logging.py
--rw-r--r--   0        0        0    13761 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    11287 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/rabbit/routing.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/rabbit/routing.pyi
--rw-r--r--   0        0        0     7479 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/rabbit/utils.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     8135 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/redis/routing.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/redis/routing.pyi
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/sqs/routing.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/sqs/routing.pyi
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/__init__.py
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/app.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/test/kafka.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/test/nats.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/test/rabbit.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/test/redis.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/test/sqs.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/utils/classes.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/utils/context/main.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.5.7/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.7/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.5.7/scripts/publish.sh
--rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 propan-0.1.5.7/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.7/scripts/test.sh
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 propan-0.1.5.7/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.5.7/LICENSE
--rw-r--r--   0        0        0    15187 2020-02-02 00:00:00.000000 propan-0.1.5.7/README.md
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 propan-0.1.5.7/pyproject.toml
--rw-r--r--   0        0        0    19622 2020-02-02 00:00:00.000000 propan-0.1.5.7/PKG-INFO
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 propan-0.1.5.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.5.8/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.5.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.5.8/.github/dependantbot.yml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.5.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.5.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 propan-0.1.5.8/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.5.8/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.5.8/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 propan-0.1.5.8/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/rabbit/header.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/rabbit/streams.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/redis/pattern.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/scheduling/rocketry.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/serialization/gen_py_code.sh
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/serialization/message.proto
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/serialization/protobuf.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/serialization/requirements.txt
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.5.8/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/__about__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/__main__.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/_compat.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/py.typed
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/constants.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/middlewares.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    21080 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/_model/routing.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    14111 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     9016 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/kafka/routing.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/kafka/routing.pyi
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/nats/consts.py
+-rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0    11462 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0     8331 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/nats/nats_js_broker.pyi
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/nats/routing.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/nats/routing.pyi
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/rabbit/logging.py
+-rw-r--r--   0        0        0    13904 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/rabbit/routing.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/rabbit/routing.pyi
+-rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/rabbit/utils.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     8135 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/redis/routing.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/redis/routing.pyi
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/sqs/routing.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/sqs/routing.pyi
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/__init__.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/app.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/test/kafka.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/test/nats.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/test/redis.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/test/sqs.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/utils/classes.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/utils/context/main.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.5.8/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.8/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.5.8/scripts/publish.sh
+-rwxr-xr-x   0        0        0      407 2020-02-02 00:00:00.000000 propan-0.1.5.8/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.5.8/scripts/test.sh
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 propan-0.1.5.8/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.5.8/LICENSE
+-rw-r--r--   0        0        0    15187 2020-02-02 00:00:00.000000 propan-0.1.5.8/README.md
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 propan-0.1.5.8/pyproject.toml
+-rw-r--r--   0        0        0    19622 2020-02-02 00:00:00.000000 propan-0.1.5.8/PKG-INFO
```

### Comparing `propan-0.1.5.7/CONTRIBUTING.md` & `propan-0.1.5.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/SECURITY.md` & `propan-0.1.5.8/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.5.8/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.5.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.5.8/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/.github/workflows/documentation.yml` & `propan-0.1.5.8/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/.github/workflows/publish_coverage.yml` & `propan-0.1.5.8/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/.github/workflows/publish_pypi.yml` & `propan-0.1.5.8/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/.github/workflows/tests.yml` & `propan-0.1.5.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/3_lifespan_events.py` & `propan-0.1.5.8/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/4_cli_attributes_promotion.py` & `propan-0.1.5.8/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/5_publishing.py` & `propan-0.1.5.8/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/6_arguments_casting.py` & `propan-0.1.5.8/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/7_handler_errors_processing.py` & `propan-0.1.5.8/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/dependencies/1_dependency_injection.py` & `propan-0.1.5.8/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.5.8/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.5.8/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.5.8/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.5.8/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/dependencies/7_annotated.py` & `propan-0.1.5.8/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.5.8/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.5.8/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.5.8/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.5.8/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/http_frameworks_integrations/quart.py` & `propan-0.1.5.8/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.5.8/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.5.8/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/rabbit/direct.py` & `propan-0.1.5.8/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/rabbit/fanout.py` & `propan-0.1.5.8/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/rabbit/header.py` & `propan-0.1.5.8/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/rabbit/topic.py` & `propan-0.1.5.8/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/redis/direct.py` & `propan-0.1.5.8/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/redis/pattern.py` & `propan-0.1.5.8/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/examples/serialization/protobuf.py` & `propan-0.1.5.8/examples/serialization/protobuf.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/__about__.py` & `propan-0.1.5.8/propan/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.5.7"
+__version__ = "0.1.5.8"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.5.7/propan/__init__.py` & `propan-0.1.5.8/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/_compat.py` & `propan-0.1.5.8/propan/_compat.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/annotations.py` & `propan-0.1.5.8/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/types.py` & `propan-0.1.5.8/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/asyncapi/__init__.py` & `propan-0.1.5.8/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/asyncapi/channels.py` & `propan-0.1.5.8/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/asyncapi/info.py` & `propan-0.1.5.8/propan/asyncapi/info.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/asyncapi/main.py` & `propan-0.1.5.8/propan/asyncapi/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/asyncapi/message.py` & `propan-0.1.5.8/propan/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/asyncapi/security.py` & `propan-0.1.5.8/propan/asyncapi/security.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/asyncapi/subscription.py` & `propan-0.1.5.8/propan/asyncapi/subscription.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/asyncapi/bindings/amqp.py` & `propan-0.1.5.8/propan/asyncapi/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/asyncapi/bindings/kafka.py` & `propan-0.1.5.8/propan/asyncapi/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/asyncapi/bindings/main.py` & `propan-0.1.5.8/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/asyncapi/bindings/redis.py` & `propan-0.1.5.8/propan/asyncapi/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/middlewares.py` & `propan-0.1.5.8/propan/brokers/middlewares.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/push_back_watcher.py` & `propan-0.1.5.8/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/_model/broker_usecase.py` & `propan-0.1.5.8/propan/brokers/_model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/_model/routing.py` & `propan-0.1.5.8/propan/brokers/_model/routing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from abc import abstractmethod
 from typing import Any, Callable, Generic, List
 
 from typing_extensions import ParamSpec, TypeVar
 
 from propan.types import AnyDict, SendableMessage
 
-
 P_RouteCall = ParamSpec("P_RouteCall")
 T_RouteReturn = TypeVar("T_RouteReturn", bound=SendableMessage)
 MsgType = TypeVar("MsgType")
 
 
 class BrokerRoute(Generic[MsgType, T_RouteReturn]):
     call: Callable[P_RouteCall, T_RouteReturn]
```

### Comparing `propan-0.1.5.7/propan/brokers/_model/schemas.py` & `propan-0.1.5.8/propan/brokers/_model/schemas.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,14 @@
 
 
 Msg = TypeVar("Msg")
 
 
 @pydantic_dataclass
 class PropanMessage(Generic[Msg]):
-    body: Union[bytes, Any]
     raw_message: Msg
+    body: Union[bytes, Any]
     content_type: Optional[str] = None
     reply_to: str = ""
     headers: AnyDict = Field(default_factory=dict)
     message_id: str = Field(default_factory=lambda: str(uuid4()))
     decoded_body: Optional[DecodedMessage] = None
```

### Comparing `propan-0.1.5.7/propan/brokers/_model/utils.py` & `propan-0.1.5.8/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.5.8/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.5.8/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/kafka/routing.py` & `propan-0.1.5.8/propan/brokers/kafka/routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from typing import Callable, Awaitable
+from typing import Awaitable, Callable
 
 from aiokafka.structs import ConsumerRecord
 
+from propan.brokers._model.broker_usecase import HandlerCallable, T_HandlerReturn
 from propan.brokers._model.routing import BrokerRouter
-from propan.brokers._model.broker_usecase import (
-    HandlerCallable,
-    T_HandlerReturn,
-)
 from propan.types import AnyDict
 
 
 class KafkaRouter(BrokerRouter[ConsumerRecord]):
     def handle(  # type: ignore[override]
         self,
         *topics: str,
```

### Comparing `propan-0.1.5.7/propan/brokers/kafka/routing.pyi` & `propan-0.1.5.8/propan/brokers/kafka/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/kafka/schemas.py` & `propan-0.1.5.8/propan/brokers/kafka/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/nats/nats_broker.py` & `propan-0.1.5.8/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.5.8/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.5.8/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/nats/nats_js_broker.pyi` & `propan-0.1.5.8/propan/brokers/nats/nats_js_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/nats/routing.py` & `propan-0.1.5.8/propan/brokers/nats/routing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import Any, Awaitable, Callable
+
 from nats.aio.msg import Msg
 
+from propan.brokers._model.broker_usecase import HandlerCallable, T_HandlerReturn
 from propan.brokers._model.routing import BrokerRouter
-from propan.brokers._model.broker_usecase import (
-    HandlerCallable,
-    T_HandlerReturn,
-)
 from propan.types import AnyDict
 
 
 class NatsRouter(BrokerRouter[Msg]):
     def handle(
         self,
         subject: str,
```

### Comparing `propan-0.1.5.7/propan/brokers/nats/routing.pyi` & `propan-0.1.5.8/propan/brokers/nats/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/nats/schemas.py` & `propan-0.1.5.8/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/rabbit/logging.py` & `propan-0.1.5.8/propan/brokers/rabbit/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.5.8/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         return connection
 
     def handle(
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         *,
+        consume_arguments: Optional[AnyDict] = None,
         dependencies: Sequence[Depends] = (),
         description: str = "",
         **original_kwargs: AnyDict,
     ) -> Callable[
         [HandlerCallable[T_HandlerReturn]],
         Callable[[aio_pika.message.IncomingMessage, bool], Awaitable[T_HandlerReturn]],
     ]:
@@ -153,14 +154,15 @@
                 **original_kwargs,
             )
             handler = Handler(
                 callback=func,
                 queue=queue,
                 exchange=exchange,
                 _description=description,
+                consume_arguments=consume_arguments,
                 dependant=dependant,
             )
             self.handlers.append(handler)
 
             return func
 
         return wrapper
@@ -177,15 +179,15 @@
             queue = await self._init_handler(handler)
 
             func = handler.callback
 
             c = self._get_log_context(None, handler.queue, handler.exchange)
             self._log(f"`{func.__name__}` waiting for messages", extra=c)
 
-            await queue.consume(func)
+            await queue.consume(func, arguments=handler.consume_arguments)
 
     async def publish(
         self,
         message: PikaSendableMessage = "",
         queue: Union[RabbitQueue, str] = "",
         exchange: Union[RabbitExchange, str, None] = None,
         *,
```

### Comparing `propan-0.1.5.7/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.5.8/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from propan.brokers._model import BrokerAsyncUsecase
 from propan.brokers._model.broker_usecase import AsyncDecoder, AsyncParser
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.middlewares import BaseMiddleware
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.log import access_logger
-from propan.types import DecodedMessage, SendableMessage
+from propan.types import AnyDict, DecodedMessage, SendableMessage
 
 PikaSendableMessage: TypeAlias = Union[aio_pika.message.Message, SendableMessage]
 T_HandlerReturn = TypeVar("T_HandlerReturn", bound=PikaSendableMessage)
 HandlerCallable: TypeAlias = Callable[
     ..., Union[T_HandlerReturn, Awaitable[T_HandlerReturn]]
 ]
 
@@ -211,14 +211,15 @@
         _publisher confirms: https://www.rabbitmq.com/confirms.html
         """
     def handle(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         *,
+        consume_arguments: Optional[AnyDict] = None,
         retry: Union[bool, int] = False,
         dependencies: Sequence[Depends] = (),
         decode_message: AsyncDecoder[IncomingMessage] = None,
         parse_message: AsyncParser[IncomingMessage] = None,
         # AsyncAPI
         description: str = "",
     ) -> Callable[
```

### Comparing `propan-0.1.5.7/propan/brokers/rabbit/routing.py` & `propan-0.1.5.8/propan/brokers/rabbit/routing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-from typing import Any, Callable, Union, Awaitable
+from typing import Any, Awaitable, Callable, Union
+
 from aio_pika.message import IncomingMessage
 
+from propan.brokers._model.broker_usecase import HandlerCallable, T_HandlerReturn
 from propan.brokers._model.routing import BrokerRouter
-from propan.brokers._model.broker_usecase import (
-    HandlerCallable,
-    T_HandlerReturn,
-)
 from propan.brokers.rabbit.schemas import RabbitQueue
 from propan.brokers.rabbit.utils import validate_queue
-
 from propan.types import AnyDict
 
 
 class RabbitRouter(BrokerRouter[IncomingMessage]):
     def handle(
         self,
         queue: Union[str, RabbitQueue],
```

### Comparing `propan-0.1.5.7/propan/brokers/rabbit/routing.pyi` & `propan-0.1.5.8/propan/brokers/rabbit/routing.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Awaitable, Callable, Sequence, Union
+from typing import Awaitable, Callable, Optional, Sequence, Union
 
 import aio_pika
 from aio_pika.message import IncomingMessage
 from fast_depends.dependencies import Depends
 from typing_extensions import TypeAlias
 
 from propan.brokers._model.broker_usecase import (
@@ -10,25 +10,26 @@
     AsyncParser,
     HandlerCallable,
     T_HandlerReturn,
 )
 from propan.brokers._model.routing import BrokerRouter
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.rabbit.schemas import RabbitExchange, RabbitQueue
-from propan.types import SendableMessage
+from propan.types import AnyDict, SendableMessage
 
 PikaSendableMessage: TypeAlias = Union[aio_pika.message.Message, SendableMessage]
 RabbitMessage: TypeAlias = PropanMessage[IncomingMessage]
 
 class RabbitRouter(BrokerRouter[IncomingMessage]):
     def handle(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         *,
+        consume_arguments: Optional[AnyDict] = None,
         retry: Union[bool, int] = False,
         dependencies: Sequence[Depends] = (),
         decode_message: AsyncDecoder[IncomingMessage] = None,
         parse_message: AsyncParser[IncomingMessage] = None,
         # AsyncAPI
         description: str = "",
     ) -> Callable[
```

### Comparing `propan-0.1.5.7/propan/brokers/rabbit/schemas.py` & `propan-0.1.5.8/propan/brokers/rabbit/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     AsyncAPIOperationBinding,
     amqp,
 )
 from propan.asyncapi.channels import AsyncAPIChannel
 from propan.asyncapi.message import AsyncAPICorrelationId, AsyncAPIMessage
 from propan.asyncapi.subscription import AsyncAPISubscription
 from propan.brokers._model.schemas import BaseHandler, NameRequired, Queue
-from propan.types import DecoratedCallable
+from propan.types import AnyDict, DecoratedCallable
 
 
 @unique
 class ExchangeType(str, Enum):
     FANOUT = "fanout"
     DIRECT = "direct"
     TOPIC = "topic"
@@ -141,28 +141,31 @@
         )
 
 
 @dataclass
 class Handler(BaseHandler):
     queue: RabbitQueue
     exchange: Optional[RabbitExchange] = field(default=None)
+    consume_arguments: AnyDict = field(default_factory=dict)
 
     def __init__(
         self,
         callback: DecoratedCallable,
         dependant: CallModel,
         queue: RabbitQueue,
         exchange: Optional[RabbitExchange] = None,
+        consume_arguments: Optional[AnyDict] = None,
         _description: str = "",
     ):
         self.callback = callback
         self.dependant = dependant
         self.queue = queue
         self.exchange = exchange
         self._description = _description
+        self.consume_arguments = consume_arguments or {}
 
     def get_schema(self) -> Dict[str, AsyncAPIChannel]:
         message_title, body, reply_to = self.get_message_object()
 
         return {
             self.title: AsyncAPIChannel(
                 subscribe=AsyncAPISubscription(
```

### Comparing `propan-0.1.5.7/propan/brokers/rabbit/utils.py` & `propan-0.1.5.8/propan/brokers/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/redis/redis_broker.py` & `propan-0.1.5.8/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.5.8/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/redis/routing.py` & `propan-0.1.5.8/propan/brokers/redis/routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from typing import Awaitable, Callable
 
-from propan.brokers._model.broker_usecase import (
-    HandlerCallable,
-    T_HandlerReturn,
-)
+from propan.brokers._model.broker_usecase import HandlerCallable, T_HandlerReturn
 from propan.brokers._model.routing import BrokerRouter
 from propan.types import AnyDict
 
 
 class RedisRouter(BrokerRouter[AnyDict]):
     def handle(  # type: ignore[override]
         self,
```

### Comparing `propan-0.1.5.7/propan/brokers/redis/routing.pyi` & `propan-0.1.5.8/propan/brokers/redis/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/redis/schemas.py` & `propan-0.1.5.8/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/sqs/routing.py` & `propan-0.1.5.8/propan/brokers/sqs/routing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from typing import Awaitable, Callable, Union
 
-from propan.brokers._model.broker_usecase import (
-    HandlerCallable,
-    T_HandlerReturn,
-)
+from propan.brokers._model.broker_usecase import HandlerCallable, T_HandlerReturn
 from propan.brokers._model.routing import BrokerRouter
 from propan.brokers.sqs.schema import SQSQueue
 from propan.types import AnyDict
 
 
 class SQSRouter(BrokerRouter[AnyDict]):
     def handle(  # type: ignore[override]
```

### Comparing `propan-0.1.5.7/propan/brokers/sqs/routing.pyi` & `propan-0.1.5.8/propan/brokers/sqs/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/sqs/schema.py` & `propan-0.1.5.8/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.5.8/propan/brokers/sqs/sqs_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.5.8/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/app.py` & `propan-0.1.5.8/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/main.py` & `propan-0.1.5.8/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/docs/app.py` & `propan-0.1.5.8/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/docs/gen.py` & `propan-0.1.5.8/propan/cli/docs/gen.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/docs/serving.py` & `propan-0.1.5.8/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/startproject/core.py` & `propan-0.1.5.8/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/startproject/async_app/app.py` & `propan-0.1.5.8/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/startproject/async_app/core.py` & `propan-0.1.5.8/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.5.8/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/startproject/async_app/nats.py` & `propan-0.1.5.8/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.5.8/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/startproject/async_app/redis.py` & `propan-0.1.5.8/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.5.8/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/supervisors/basereload.py` & `propan-0.1.5.8/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/supervisors/multiprocess.py` & `propan-0.1.5.8/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/supervisors/utils.py` & `propan-0.1.5.8/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/supervisors/watchfiles.py` & `propan-0.1.5.8/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/utils/imports.py` & `propan-0.1.5.8/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/utils/logs.py` & `propan-0.1.5.8/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/cli/utils/parser.py` & `propan-0.1.5.8/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/fastapi/__init__.py` & `propan-0.1.5.8/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/fastapi/core/route.py` & `propan-0.1.5.8/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/fastapi/core/router.py` & `propan-0.1.5.8/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/fastapi/kafka/router.pyi` & `propan-0.1.5.8/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/fastapi/nats/router.pyi` & `propan-0.1.5.8/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/fastapi/rabbit/router.pyi` & `propan-0.1.5.8/propan/fastapi/rabbit/router.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     AsyncParser,
     HandlerCallable,
     T_HandlerReturn,
 )
 from propan.brokers.rabbit import RabbitExchange, RabbitQueue
 from propan.fastapi.core import PropanRouter
 from propan.log import access_logger
+from propan.types import AnyDict
 
 class RabbitRouter(PropanRouter[RabbitBroker]):
     def __init__(
         self,
         host: str = "localhost",
         port: int = 5672,
         login: str = "guest",
@@ -84,14 +85,15 @@
     ) -> Callable[[IncomingMessage, bool], Awaitable[T_HandlerReturn]]:
         pass
     def event(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         *,
         exchange: Union[str, RabbitExchange, None] = None,
+        consume_arguments: Optional[AnyDict] = None,
         retry: Union[bool, int] = False,
         decode_message: AsyncDecoder[IncomingMessage] = None,
         parse_message: AsyncParser[IncomingMessage] = None,
         description: str = "",
         dependencies: Optional[Sequence[params.Depends]] = None,
     ) -> Callable[
         [HandlerCallable[T_HandlerReturn]],
```

### Comparing `propan-0.1.5.7/propan/fastapi/redis/router.pyi` & `propan-0.1.5.8/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/fastapi/sqs/router.pyi` & `propan-0.1.5.8/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/log/formatter.py` & `propan-0.1.5.8/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/log/logging.py` & `propan-0.1.5.8/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/test/__init__.py` & `propan-0.1.5.8/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/test/kafka.py` & `propan-0.1.5.8/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/test/nats.py` & `propan-0.1.5.8/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/test/rabbit.py` & `propan-0.1.5.8/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/test/redis.py` & `propan-0.1.5.8/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/test/sqs.py` & `propan-0.1.5.8/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/test/utils.py` & `propan-0.1.5.8/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/utils/functions.py` & `propan-0.1.5.8/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/utils/context/main.py` & `propan-0.1.5.8/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/propan/utils/context/types.py` & `propan-0.1.5.8/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/LICENSE` & `propan-0.1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/README.md` & `propan-0.1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/pyproject.toml` & `propan-0.1.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.5.7/PKG-INFO` & `propan-0.1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.5.7
+Version: 0.1.5.8
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```


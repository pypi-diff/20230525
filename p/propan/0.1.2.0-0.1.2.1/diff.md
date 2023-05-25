# Comparing `tmp/propan-0.1.2.0.tar.gz` & `tmp/propan-0.1.2.1.tar.gz`

## Comparing `propan-0.1.2.0.tar` & `propan-0.1.2.1.tar`

### file list

```diff
@@ -1,126 +1,127 @@
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.0/SECURITY.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.2.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.0/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 propan-0.1.2.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.0/examples/redis/pattern.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/__about__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/__main__.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/py.typed
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/model/utils.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/app.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/log/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/log/logging.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/test/kafka.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/test/redis.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.0/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.0/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.0/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.0/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.0/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.2.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.0/LICENSE
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 propan-0.1.2.0/README.md
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 propan-0.1.2.0/pyproject.toml
--rw-r--r--   0        0        0    15874 2020-02-02 00:00:00.000000 propan-0.1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.1/SECURITY.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.2.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.1/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 propan-0.1.2.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/redis/pattern.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/__about__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/__main__.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/py.typed
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/model/utils.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/app.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/log/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/log/logging.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/test/kafka.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/test/redis.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.1/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.1/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.1/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.1/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.2.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.1/LICENSE
+-rw-r--r--   0        0        0    12237 2020-02-02 00:00:00.000000 propan-0.1.2.1/README.md
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 propan-0.1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    15819 2020-02-02 00:00:00.000000 propan-0.1.2.1/PKG-INFO
```

### Comparing `propan-0.1.2.0/CONTRIBUTING.md` & `propan-0.1.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/SECURITY.md` & `propan-0.1.2.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/.github/workflows/documentation.yml` & `propan-0.1.2.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/.github/workflows/publish_coverage.yml` & `propan-0.1.2.1/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/.github/workflows/publish_pypi.yml` & `propan-0.1.2.1/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/.github/workflows/tests.yml` & `propan-0.1.2.1/.github/workflows/tests.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,24 +16,14 @@
       fail-fast: false
 
     services:
       rabbitmq:
         image: rabbitmq
         ports:
           - 5672:5672
-
-      redis:
-        image: redis
-        ports:
-          - 6379:6379
-
-      nats:
-        image: nats
-        ports:
-          - 4222:4222
       
       kafka:
         image: bitnami/kafka
         ports:
           - 9092:9092
         env:
           KAFKA_ENABLE_KRAFT: "true"
@@ -43,14 +33,24 @@
           KAFKA_CFG_LISTENERS: "PLAINTEXT://:9092,CONTROLLER://:9093"
           KAFKA_CFG_LISTENER_SECURITY_PROTOCOL_MAP: "CONTROLLER:PLAINTEXT,PLAINTEXT:PLAINTEXT"
           KAFKA_CFG_ADVERTISED_LISTENERS: "PLAINTEXT://127.0.0.1:9092"
           KAFKA_BROKER_ID: "1"
           KAFKA_CFG_CONTROLLER_QUORUM_VOTERS: "1@kafka:9093"
           ALLOW_PLAINTEXT_LISTENER: "true"
 
+      nats:
+        image: nats
+        ports:
+          - 4222:4222
+
+      redis:
+        image: redis
+        ports:
+          - 6379:6379
+
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
```

### Comparing `propan-0.1.2.0/examples/3_lifespan_events.py` & `propan-0.1.2.1/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/4_cli_attributes_promotion.py` & `propan-0.1.2.1/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/5_publishing.py` & `propan-0.1.2.1/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/6_arguments_casting.py` & `propan-0.1.2.1/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/7_handler_errors_processing.py` & `propan-0.1.2.1/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/dependencies/1_dependency_injection.py` & `propan-0.1.2.1/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.2.1/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.2.1/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.2.1/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.2.1/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/dependencies/7_annotated.py` & `propan-0.1.2.1/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.2.1/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.2.1/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.2.1/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.2.1/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/http_frameworks_integrations/quart.py` & `propan-0.1.2.1/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.2.1/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.2.1/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/rabbit/direct.py` & `propan-0.1.2.1/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/rabbit/fanout.py` & `propan-0.1.2.1/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/rabbit/header.py` & `propan-0.1.2.1/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/rabbit/topic.py` & `propan-0.1.2.1/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/redis/direct.py` & `propan-0.1.2.1/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/examples/redis/pattern.py` & `propan-0.1.2.1/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/__init__.py` & `propan-0.1.2.1/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/annotations.py` & `propan-0.1.2.1/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/types.py` & `propan-0.1.2.1/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/push_back_watcher.py` & `propan-0.1.2.1/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.2.1/propan/brokers/kafka/kafka_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,19 @@
         }
         return partial(AIOKafkaConsumer, **consumer_kwargs)
 
     async def close(self) -> None:
         for handler in self.handlers:
             if handler.task is not None:
                 handler.task.cancel()
+                handler.task = None
 
             if handler.consumer is not None:
                 await handler.consumer.stop()
+                handler.consumer = None
 
         if self._publisher is not None:
             await self._publisher.stop()
             self._publisher = None
 
     def handle(
         self,
```

### Comparing `propan-0.1.2.0/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.2.1/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/model/broker_usecase.py` & `propan-0.1.2.1/propan/brokers/model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/model/schemas.py` & `propan-0.1.2.1/propan/brokers/model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/model/utils.py` & `propan-0.1.2.1/propan/brokers/model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/nats/nats_broker.py` & `propan-0.1.2.1/propan/brokers/nats/nats_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,17 +103,19 @@
                 "content-type": content_type,
             },
             **publish_args,
         )
 
     async def close(self) -> None:
         for h in self.handlers:
-            await h.subscription.unsubscribe()
+            if h.subscription is not None:
+                await h.subscription.unsubscribe()
+                h.subscription = None
 
-        if self._connection:
+        if self._connection is not None:
             await self._connection.drain()
             self._connection = None
 
     def _get_log_context(
         self,
         message: Optional[PropanMessage],
         subject: str,
```

### Comparing `propan-0.1.2.0/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.2.1/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.2.1/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/nats/schemas.py` & `propan-0.1.2.1/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.2.1/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.2.1/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/rabbit/schemas.py` & `propan-0.1.2.1/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/redis/redis_broker.py` & `propan-0.1.2.1/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.2.1/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/brokers/redis/schemas.py` & `propan-0.1.2.1/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/app.py` & `propan-0.1.2.1/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/main.py` & `propan-0.1.2.1/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/startproject/core.py` & `propan-0.1.2.1/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/startproject/async_app/app.py` & `propan-0.1.2.1/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/startproject/async_app/core.py` & `propan-0.1.2.1/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.2.1/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/startproject/async_app/nats.py` & `propan-0.1.2.1/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.2.1/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/startproject/async_app/redis.py` & `propan-0.1.2.1/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/supervisors/basereload.py` & `propan-0.1.2.1/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/supervisors/multiprocess.py` & `propan-0.1.2.1/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/supervisors/utils.py` & `propan-0.1.2.1/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/supervisors/watchfiles.py` & `propan-0.1.2.1/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/utils/imports.py` & `propan-0.1.2.1/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/utils/logs.py` & `propan-0.1.2.1/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/cli/utils/parser.py` & `propan-0.1.2.1/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/fastapi/__init__.py` & `propan-0.1.2.1/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/fastapi/core/route.py` & `propan-0.1.2.1/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/fastapi/core/router.py` & `propan-0.1.2.1/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/fastapi/kafka/router.pyi` & `propan-0.1.2.1/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/fastapi/rabbit/router.pyi` & `propan-0.1.2.1/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/fastapi/redis/router.pyi` & `propan-0.1.2.1/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/log/formatter.py` & `propan-0.1.2.1/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/log/logging.py` & `propan-0.1.2.1/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/test/__init__.py` & `propan-0.1.2.1/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/test/kafka.py` & `propan-0.1.2.1/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/test/rabbit.py` & `propan-0.1.2.1/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/test/redis.py` & `propan-0.1.2.1/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/test/utils.py` & `propan-0.1.2.1/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/utils/functions.py` & `propan-0.1.2.1/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/utils/context/main.py` & `propan-0.1.2.1/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/propan/utils/context/types.py` & `propan-0.1.2.1/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/LICENSE` & `propan-0.1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/README.md` & `propan-0.1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **SQS**           | :mag: planning :mag:                                    | :mag: planning :mag: |
 
 ### Community
 
 If you are interested in this project, please give me feedback by star or/and watch repository.
 
-If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions) or public [telegram group](https://t.me/propan_python).
+If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions).
 
 ---
 
 ## Declarative?
 
 With declarative tools you can define **what you need to get**. With traditional imperative tools you must write **what you need to do**.
```

#### html2text {}

```diff
@@ -31,89 +31,88 @@
 mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :hammer_and_wrench: |
 :mag: planning :mag: | | **MQTT** | :mag: planning :mag: | :mag: planning :mag:
 | | **Redis Streams** | :mag: planning :mag: | :mag: planning :mag: | |
 **Pulsar** | :mag: planning :mag: | :mag: planning :mag: | | **SQS** | :mag:
 planning :mag: | :mag: planning :mag: | ### Community If you are interested in
 this project, please give me feedback by star or/and watch repository. If you
 have any questions or ideas about features to implement, welcome to
-[discussions](https://github.com/Lancetnik/Propan/discussions) or public
-[telegram group](https://t.me/propan_python). --- ## Declarative? With
-declarative tools you can define **what you need to get**. With traditional
-imperative tools you must write **what you need to do**. Take a look at classic
-imperative tools, such as aio-pika, pika, redis-py, nats-py, etc. This is the
-**Quickstart** with the *aio-pika*: ```python import asyncio import aio_pika
-async def main(): connection = await aio_pika.connect_robust( "amqp://guest:
-guest@127.0.0.1/" ) queue_name = "test_queue" async with connection: channel =
-await connection.channel() queue = await channel.declare_queue(queue_name)
-async with queue.iterator() as queue_iter: async for message in queue_iter:
-async with message.process(): print(message.body) asyncio.run(main()) ```
-**aio-pika** is a great tool with a really easy learning curve. But it's still
-imperative. You need to *connect*, declare *channel*, *queues*, *exchanges* by
-yourself. Also, you need to manage *connection*, *message*, *queue* context to
-avoid any troubles. It is not a bad way, but it can be much easier. ```python
-from propan import PropanApp, RabbitBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(broker) @broker.handle("test_queue")
-async def base_handler(body): print(body) ``` This is the **Propan**
-declarative way to write the same code. That is so much easier, isn't it? --
-- ## Quickstart Install using `pip`: ```shell pip install "propan[async-
-rabbit]" # or pip install "propan[async-nats]" # or pip install "propan[async-
-redis]" # or pip install "propan[async-kafka]" ``` ### Basic usage Create an
-application with the following code at `serve.py`: ```python from propan import
-PropanApp from propan import RabbitBroker # from propan import RedisBroker #
-from propan import NatsBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222") # broker
-= RedisBroker("redis://localhost:6379") app = PropanApp(broker) @broker.handle
-("test") async def base_handler(body): '''Handle all default exchange messages
-with `test` routing key''' print(body) ``` And just run it: ```shell propan run
-serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
-function arguments to types according to their annotation. ```python from
-pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
-broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
-(broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
-def second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` -
--- ## Dependencies **Propan** a has dependencies management policy close to
-`pytest fixtures`. You can specify in functions arguments which dependencies
-you would to use. Framework passes them from the global Context object. Already
-existed context fields are: *app*, *broker*, *context* (itself), *logger* and
-*message*. If you call not existing field, raises *pydantic.ValidationError*
-value. But you can specify your own dependencies, call dependencies functions
-(like `Fastapi Depends`) and [more](https://github.com/Lancetnik/Propan/tree/
-main/examples/dependencies). ```python import aio_pika from propan import
-PropanApp, RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://
-guest:guest@localhost:5672/") app = PropanApp(rabbit_broker) async def
-dependency(body: dict) -> bool: return True @rabbit_broker.handle("test") async
-def base_handler(body: dict, dep: bool = Depends(dependency), broker:
-RabbitBroker = Context()): assert dep is True assert broker is rabbit_broker
-``` --- ## CLI power **Propan** has its own CLI tool that provided the
-following features: * project generation * multiprocessing workers * project
-hot reloading * custom command line arguments passing ### Context passing For
-example: pass your current *.env* project setting to context ```bash propan run
-serve:app --env=.env.dev ``` ```python from propan import PropanApp,
-RabbitBroker from propan.annotations import ContextRepo from pydantic import
-BaseSettings broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
-PropanApp(broker) class Settings(BaseSettings): ... @app.on_startup async def
-setup(env: str, context: ContextRepo): settings = Settings(_env_file=env)
-context.set_global("settings", settings) ``` ### Project template Also,
-**Propan CLI** is able to generate a production-ready application template:
-```bash propan create async rabbit [projectname] ``` *Notice: project template
-require* `pydantic[dotenv]` *installation.* Run the created project: ```bash #
-Run rabbimq first docker compose --file [projectname]/docker-compose.yaml up -
-d # Run project propan run [projectname].app.serve:app --env=.env --reload ```
-Now you can enjoy a new development experience! --- ## HTTP Frameworks
-integrations ### Any Framework You can use **Propan** `MQBrokers` without
-`PropanApp`. Just *start* and *stop* them according to your application
-lifespan. ```python from propan import NatsBroker from sanic import Sanic app =
-Sanic("MyHelloWorldApp") broker = NatsBroker("nats://localhost:4222")
-@broker.handle("test") async def base_handler(body): print(body)
-@app.after_server_start async def start_broker(app, loop): await broker.start()
-@app.after_server_stop async def stop_broker(app, loop): await broker.close()
-``` ### FastAPI Plugin Also, **Propan** can be used as part of **FastAPI**.
-Just import a **PropanRouter** you need and declare the message handler using
-the `@event` decorator. This decorator is similar to the decorator `@handle`
-for the corresponding brokers. ```python from fastapi import Depends, FastAPI
-from pydantic import BaseModel from propan.fastapi import RabbitRouter app =
-FastAPI() router = RabbitRouter("amqp://guest:guest@localhost:5672") class
-Incoming(BaseModel): m: dict def call(): return True @router.event("test")
-async def hello(m: Incoming, d = Depends(call)) -> dict: return { "response":
-"Hello, Propan!" } app.include_router(router) ``` ## Examples To see more
-framework usages go to [**examples/**](https://github.com/Lancetnik/Propan/
-tree/main/examples)
+[discussions](https://github.com/Lancetnik/Propan/discussions). --- ##
+Declarative? With declarative tools you can define **what you need to get**.
+With traditional imperative tools you must write **what you need to do**. Take
+a look at classic imperative tools, such as aio-pika, pika, redis-py, nats-py,
+etc. This is the **Quickstart** with the *aio-pika*: ```python import asyncio
+import aio_pika async def main(): connection = await aio_pika.connect_robust
+( "amqp://guest:guest@127.0.0.1/" ) queue_name = "test_queue" async with
+connection: channel = await connection.channel() queue = await
+channel.declare_queue(queue_name) async with queue.iterator() as queue_iter:
+async for message in queue_iter: async with message.process(): print
+(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
+really easy learning curve. But it's still imperative. You need to *connect*,
+declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
+*connection*, *message*, *queue* context to avoid any troubles. It is not a bad
+way, but it can be much easier. ```python from propan import PropanApp,
+RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
+print(body) ``` This is the **Propan** declarative way to write the same code.
+That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
+```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
+nats]" # or pip install "propan[async-redis]" # or pip install "propan[async-
+kafka]" ``` ### Basic usage Create an application with the following code at
+`serve.py`: ```python from propan import PropanApp from propan import
+RabbitBroker # from propan import RedisBroker # from propan import NatsBroker
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/") # broker =
+NatsBroker("nats://localhost:4222") # broker = RedisBroker("redis://localhost:
+6379") app = PropanApp(broker) @broker.handle("test") async def base_handler
+(body): '''Handle all default exchange messages with `test` routing key'''
+print(body) ``` And just run it: ```shell propan run serve:app ``` --- ## Type
+casting Propan uses `pydantic` to cast incoming function arguments to types
+according to their annotation. ```python from pydantic import BaseModel from
+propan import PropanApp, Context, RabbitBroker broker = RabbitBroker("amqp://
+guest:guest@localhost:5672/") app = PropanApp(broker) class SimpleMessage
+(BaseModel): key: int @broker.handle("test2") async def second_handler(body:
+SimpleMessage): assert isinstance(body.key, int) ``` --- ## Dependencies
+**Propan** a has dependencies management policy close to `pytest fixtures`. You
+can specify in functions arguments which dependencies you would to use.
+Framework passes them from the global Context object. Already existed context
+fields are: *app*, *broker*, *context* (itself), *logger* and *message*. If you
+call not existing field, raises *pydantic.ValidationError* value. But you can
+specify your own dependencies, call dependencies functions (like `Fastapi
+Depends`) and [more](https://github.com/Lancetnik/Propan/tree/main/examples/
+dependencies). ```python import aio_pika from propan import PropanApp,
+RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") app = PropanApp(rabbit_broker) async def dependency
+(body: dict) -> bool: return True @rabbit_broker.handle("test") async def
+base_handler(body: dict, dep: bool = Depends(dependency), broker: RabbitBroker
+= Context()): assert dep is True assert broker is rabbit_broker ``` --- ## CLI
+power **Propan** has its own CLI tool that provided the following features: *
+project generation * multiprocessing workers * project hot reloading * custom
+command line arguments passing ### Context passing For example: pass your
+current *.env* project setting to context ```bash propan run serve:app --
+env=.env.dev ``` ```python from propan import PropanApp, RabbitBroker from
+propan.annotations import ContextRepo from pydantic import BaseSettings broker
+= RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp(broker)
+class Settings(BaseSettings): ... @app.on_startup async def setup(env: str,
+context: ContextRepo): settings = Settings(_env_file=env) context.set_global
+("settings", settings) ``` ### Project template Also, **Propan CLI** is able to
+generate a production-ready application template: ```bash propan create async
+rabbit [projectname] ``` *Notice: project template require* `pydantic[dotenv]`
+*installation.* Run the created project: ```bash # Run rabbimq first docker
+compose --file [projectname]/docker-compose.yaml up -d # Run project propan run
+[projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
+development experience! --- ## HTTP Frameworks integrations ### Any Framework
+You can use **Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop*
+them according to your application lifespan. ```python from propan import
+NatsBroker from sanic import Sanic app = Sanic("MyHelloWorldApp") broker =
+NatsBroker("nats://localhost:4222") @broker.handle("test") async def
+base_handler(body): print(body) @app.after_server_start async def start_broker
+(app, loop): await broker.start() @app.after_server_stop async def stop_broker
+(app, loop): await broker.close() ``` ### FastAPI Plugin Also, **Propan** can
+be used as part of **FastAPI**. Just import a **PropanRouter** you need and
+declare the message handler using the `@event` decorator. This decorator is
+similar to the decorator `@handle` for the corresponding brokers. ```python
+from fastapi import Depends, FastAPI from pydantic import BaseModel from
+propan.fastapi import RabbitRouter app = FastAPI() router = RabbitRouter("amqp:
+//guest:guest@localhost:5672") class Incoming(BaseModel): m: dict def call():
+return True @router.event("test") async def hello(m: Incoming, d = Depends
+(call)) -> dict: return { "response": "Hello, Propan!" } app.include_router
+(router) ``` ## Examples To see more framework usages go to [**examples/**]
+(https://github.com/Lancetnik/Propan/tree/main/examples)
```

### Comparing `propan-0.1.2.0/pyproject.toml` & `propan-0.1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.0/PKG-INFO` & `propan-0.1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.2.0
+Version: 0.1.2.1
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-Expression: MIT
@@ -150,15 +150,15 @@
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **SQS**           | :mag: planning :mag:                                    | :mag: planning :mag: |
 
 ### Community
 
 If you are interested in this project, please give me feedback by star or/and watch repository.
 
-If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions) or public [telegram group](https://t.me/propan_python).
+If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions).
 
 ---
 
 ## Declarative?
 
 With declarative tools you can define **what you need to get**. With traditional imperative tools you must write **what you need to do**.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.2.0 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.2.1 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-Expression: MIT License-File: LICENSE Keywords:
 framework,message brokers,rabbitmq Classifier: Development Status :: 5 -
@@ -79,89 +79,88 @@
 mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :hammer_and_wrench: |
 :mag: planning :mag: | | **MQTT** | :mag: planning :mag: | :mag: planning :mag:
 | | **Redis Streams** | :mag: planning :mag: | :mag: planning :mag: | |
 **Pulsar** | :mag: planning :mag: | :mag: planning :mag: | | **SQS** | :mag:
 planning :mag: | :mag: planning :mag: | ### Community If you are interested in
 this project, please give me feedback by star or/and watch repository. If you
 have any questions or ideas about features to implement, welcome to
-[discussions](https://github.com/Lancetnik/Propan/discussions) or public
-[telegram group](https://t.me/propan_python). --- ## Declarative? With
-declarative tools you can define **what you need to get**. With traditional
-imperative tools you must write **what you need to do**. Take a look at classic
-imperative tools, such as aio-pika, pika, redis-py, nats-py, etc. This is the
-**Quickstart** with the *aio-pika*: ```python import asyncio import aio_pika
-async def main(): connection = await aio_pika.connect_robust( "amqp://guest:
-guest@127.0.0.1/" ) queue_name = "test_queue" async with connection: channel =
-await connection.channel() queue = await channel.declare_queue(queue_name)
-async with queue.iterator() as queue_iter: async for message in queue_iter:
-async with message.process(): print(message.body) asyncio.run(main()) ```
-**aio-pika** is a great tool with a really easy learning curve. But it's still
-imperative. You need to *connect*, declare *channel*, *queues*, *exchanges* by
-yourself. Also, you need to manage *connection*, *message*, *queue* context to
-avoid any troubles. It is not a bad way, but it can be much easier. ```python
-from propan import PropanApp, RabbitBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(broker) @broker.handle("test_queue")
-async def base_handler(body): print(body) ``` This is the **Propan**
-declarative way to write the same code. That is so much easier, isn't it? --
-- ## Quickstart Install using `pip`: ```shell pip install "propan[async-
-rabbit]" # or pip install "propan[async-nats]" # or pip install "propan[async-
-redis]" # or pip install "propan[async-kafka]" ``` ### Basic usage Create an
-application with the following code at `serve.py`: ```python from propan import
-PropanApp from propan import RabbitBroker # from propan import RedisBroker #
-from propan import NatsBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222") # broker
-= RedisBroker("redis://localhost:6379") app = PropanApp(broker) @broker.handle
-("test") async def base_handler(body): '''Handle all default exchange messages
-with `test` routing key''' print(body) ``` And just run it: ```shell propan run
-serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
-function arguments to types according to their annotation. ```python from
-pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
-broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
-(broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
-def second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` -
--- ## Dependencies **Propan** a has dependencies management policy close to
-`pytest fixtures`. You can specify in functions arguments which dependencies
-you would to use. Framework passes them from the global Context object. Already
-existed context fields are: *app*, *broker*, *context* (itself), *logger* and
-*message*. If you call not existing field, raises *pydantic.ValidationError*
-value. But you can specify your own dependencies, call dependencies functions
-(like `Fastapi Depends`) and [more](https://github.com/Lancetnik/Propan/tree/
-main/examples/dependencies). ```python import aio_pika from propan import
-PropanApp, RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://
-guest:guest@localhost:5672/") app = PropanApp(rabbit_broker) async def
-dependency(body: dict) -> bool: return True @rabbit_broker.handle("test") async
-def base_handler(body: dict, dep: bool = Depends(dependency), broker:
-RabbitBroker = Context()): assert dep is True assert broker is rabbit_broker
-``` --- ## CLI power **Propan** has its own CLI tool that provided the
-following features: * project generation * multiprocessing workers * project
-hot reloading * custom command line arguments passing ### Context passing For
-example: pass your current *.env* project setting to context ```bash propan run
-serve:app --env=.env.dev ``` ```python from propan import PropanApp,
-RabbitBroker from propan.annotations import ContextRepo from pydantic import
-BaseSettings broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
-PropanApp(broker) class Settings(BaseSettings): ... @app.on_startup async def
-setup(env: str, context: ContextRepo): settings = Settings(_env_file=env)
-context.set_global("settings", settings) ``` ### Project template Also,
-**Propan CLI** is able to generate a production-ready application template:
-```bash propan create async rabbit [projectname] ``` *Notice: project template
-require* `pydantic[dotenv]` *installation.* Run the created project: ```bash #
-Run rabbimq first docker compose --file [projectname]/docker-compose.yaml up -
-d # Run project propan run [projectname].app.serve:app --env=.env --reload ```
-Now you can enjoy a new development experience! --- ## HTTP Frameworks
-integrations ### Any Framework You can use **Propan** `MQBrokers` without
-`PropanApp`. Just *start* and *stop* them according to your application
-lifespan. ```python from propan import NatsBroker from sanic import Sanic app =
-Sanic("MyHelloWorldApp") broker = NatsBroker("nats://localhost:4222")
-@broker.handle("test") async def base_handler(body): print(body)
-@app.after_server_start async def start_broker(app, loop): await broker.start()
-@app.after_server_stop async def stop_broker(app, loop): await broker.close()
-``` ### FastAPI Plugin Also, **Propan** can be used as part of **FastAPI**.
-Just import a **PropanRouter** you need and declare the message handler using
-the `@event` decorator. This decorator is similar to the decorator `@handle`
-for the corresponding brokers. ```python from fastapi import Depends, FastAPI
-from pydantic import BaseModel from propan.fastapi import RabbitRouter app =
-FastAPI() router = RabbitRouter("amqp://guest:guest@localhost:5672") class
-Incoming(BaseModel): m: dict def call(): return True @router.event("test")
-async def hello(m: Incoming, d = Depends(call)) -> dict: return { "response":
-"Hello, Propan!" } app.include_router(router) ``` ## Examples To see more
-framework usages go to [**examples/**](https://github.com/Lancetnik/Propan/
-tree/main/examples)
+[discussions](https://github.com/Lancetnik/Propan/discussions). --- ##
+Declarative? With declarative tools you can define **what you need to get**.
+With traditional imperative tools you must write **what you need to do**. Take
+a look at classic imperative tools, such as aio-pika, pika, redis-py, nats-py,
+etc. This is the **Quickstart** with the *aio-pika*: ```python import asyncio
+import aio_pika async def main(): connection = await aio_pika.connect_robust
+( "amqp://guest:guest@127.0.0.1/" ) queue_name = "test_queue" async with
+connection: channel = await connection.channel() queue = await
+channel.declare_queue(queue_name) async with queue.iterator() as queue_iter:
+async for message in queue_iter: async with message.process(): print
+(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
+really easy learning curve. But it's still imperative. You need to *connect*,
+declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
+*connection*, *message*, *queue* context to avoid any troubles. It is not a bad
+way, but it can be much easier. ```python from propan import PropanApp,
+RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
+print(body) ``` This is the **Propan** declarative way to write the same code.
+That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
+```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
+nats]" # or pip install "propan[async-redis]" # or pip install "propan[async-
+kafka]" ``` ### Basic usage Create an application with the following code at
+`serve.py`: ```python from propan import PropanApp from propan import
+RabbitBroker # from propan import RedisBroker # from propan import NatsBroker
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/") # broker =
+NatsBroker("nats://localhost:4222") # broker = RedisBroker("redis://localhost:
+6379") app = PropanApp(broker) @broker.handle("test") async def base_handler
+(body): '''Handle all default exchange messages with `test` routing key'''
+print(body) ``` And just run it: ```shell propan run serve:app ``` --- ## Type
+casting Propan uses `pydantic` to cast incoming function arguments to types
+according to their annotation. ```python from pydantic import BaseModel from
+propan import PropanApp, Context, RabbitBroker broker = RabbitBroker("amqp://
+guest:guest@localhost:5672/") app = PropanApp(broker) class SimpleMessage
+(BaseModel): key: int @broker.handle("test2") async def second_handler(body:
+SimpleMessage): assert isinstance(body.key, int) ``` --- ## Dependencies
+**Propan** a has dependencies management policy close to `pytest fixtures`. You
+can specify in functions arguments which dependencies you would to use.
+Framework passes them from the global Context object. Already existed context
+fields are: *app*, *broker*, *context* (itself), *logger* and *message*. If you
+call not existing field, raises *pydantic.ValidationError* value. But you can
+specify your own dependencies, call dependencies functions (like `Fastapi
+Depends`) and [more](https://github.com/Lancetnik/Propan/tree/main/examples/
+dependencies). ```python import aio_pika from propan import PropanApp,
+RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") app = PropanApp(rabbit_broker) async def dependency
+(body: dict) -> bool: return True @rabbit_broker.handle("test") async def
+base_handler(body: dict, dep: bool = Depends(dependency), broker: RabbitBroker
+= Context()): assert dep is True assert broker is rabbit_broker ``` --- ## CLI
+power **Propan** has its own CLI tool that provided the following features: *
+project generation * multiprocessing workers * project hot reloading * custom
+command line arguments passing ### Context passing For example: pass your
+current *.env* project setting to context ```bash propan run serve:app --
+env=.env.dev ``` ```python from propan import PropanApp, RabbitBroker from
+propan.annotations import ContextRepo from pydantic import BaseSettings broker
+= RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp(broker)
+class Settings(BaseSettings): ... @app.on_startup async def setup(env: str,
+context: ContextRepo): settings = Settings(_env_file=env) context.set_global
+("settings", settings) ``` ### Project template Also, **Propan CLI** is able to
+generate a production-ready application template: ```bash propan create async
+rabbit [projectname] ``` *Notice: project template require* `pydantic[dotenv]`
+*installation.* Run the created project: ```bash # Run rabbimq first docker
+compose --file [projectname]/docker-compose.yaml up -d # Run project propan run
+[projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
+development experience! --- ## HTTP Frameworks integrations ### Any Framework
+You can use **Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop*
+them according to your application lifespan. ```python from propan import
+NatsBroker from sanic import Sanic app = Sanic("MyHelloWorldApp") broker =
+NatsBroker("nats://localhost:4222") @broker.handle("test") async def
+base_handler(body): print(body) @app.after_server_start async def start_broker
+(app, loop): await broker.start() @app.after_server_stop async def stop_broker
+(app, loop): await broker.close() ``` ### FastAPI Plugin Also, **Propan** can
+be used as part of **FastAPI**. Just import a **PropanRouter** you need and
+declare the message handler using the `@event` decorator. This decorator is
+similar to the decorator `@handle` for the corresponding brokers. ```python
+from fastapi import Depends, FastAPI from pydantic import BaseModel from
+propan.fastapi import RabbitRouter app = FastAPI() router = RabbitRouter("amqp:
+//guest:guest@localhost:5672") class Incoming(BaseModel): m: dict def call():
+return True @router.event("test") async def hello(m: Incoming, d = Depends
+(call)) -> dict: return { "response": "Hello, Propan!" } app.include_router
+(router) ``` ## Examples To see more framework usages go to [**examples/**]
+(https://github.com/Lancetnik/Propan/tree/main/examples)
```


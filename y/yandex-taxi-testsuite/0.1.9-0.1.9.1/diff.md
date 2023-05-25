# Comparing `tmp/yandex-taxi-testsuite-0.1.9.tar.gz` & `tmp/yandex-taxi-testsuite-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandex-taxi-testsuite-0.1.9.tar", last modified: Mon Mar 27 14:37:15 2023, max compression
+gzip compressed data, was "yandex-taxi-testsuite-0.1.9.1.tar", last modified: Tue Mar 28 15:48:36 2023, max compression
```

## Comparing `yandex-taxi-testsuite-0.1.9.tar` & `yandex-taxi-testsuite-0.1.9.1.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.395980 yandex-taxi-testsuite-0.1.9/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)     1097 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/AUTHORS
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1082 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9/LICENSE
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3822 2023-03-27 14:37:15.395980 yandex-taxi-testsuite-0.1.9/PKG-INFO
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3142 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/README.rst
--rw-r--r--   0 vitja     (1000) vitja     (1000)       89 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/pyproject.toml
--rw-r--r--   0 vitja     (1000) vitja     (1000)      565 2023-03-27 14:37:15.395980 yandex-taxi-testsuite-0.1.9/setup.cfg
--rw-r--r--   0 vitja     (1000) vitja     (1000)     2031 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/setup.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.385980 yandex-taxi-testsuite-0.1.9/tests/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)     2916 2020-03-11 14:08:30.000000 yandex-taxi-testsuite-0.1.9/tests/test_ensure_db_indexes.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     2219 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/tests/test_http.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     4288 2023-03-27 14:36:21.000000 yandex-taxi-testsuite-0.1.9/tests/test_json_util.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      858 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/tests/test_loaders.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3663 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/tests/test_ordered_object.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1299 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/tests/test_service_client.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.385980 yandex-taxi-testsuite-0.1.9/testsuite/
--rw-r--r--   0 vitja     (1000) vitja     (1000)      139 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9/testsuite/__init__.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.385980 yandex-taxi-testsuite-0.1.9/testsuite/_internal/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9/testsuite/_internal/__init__.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     2498 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/_internal/fixture_class.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      635 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9/testsuite/_internal/fixture_types.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      450 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9/testsuite/annotations.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.385980 yandex-taxi-testsuite-0.1.9/testsuite/daemons/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/daemons/__init__.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)    14817 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/daemons/pytest_plugin.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     8750 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/daemons/service_client.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     7019 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/daemons/service_daemon.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     5854 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/daemons/spawn.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.385980 yandex-taxi-testsuite-0.1.9/testsuite/databases/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/__init__.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.385980 yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2022-03-18 08:22:00.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/__init__.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      571 2022-03-18 08:22:00.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/classes.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     4019 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/control.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1012 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/discover.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     4831 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/pytest_plugin.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.385980 yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/scripts/
--rw-r--r--   0 vitja     (1000) vitja     (1000)      599 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/scripts/find-clickhouse.sh
--rwxr-xr-x   0 vitja     (1000) vitja     (1000)     1412 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/scripts/service-clickhouse
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1784 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/service.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      235 2022-03-18 08:22:00.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/utils.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/__init__.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1946 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/connection.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3366 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/ensure_db_indexes.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     2948 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/mongo_schema.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)    12123 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/pytest_plugin.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/scripts/
--rwxr-xr-x   0 vitja     (1000) vitja     (1000)     3630 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/scripts/service-mongo
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1877 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/service.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/__init__.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)     1119 2021-10-18 08:34:13.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/classes.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     7691 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/control.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1962 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/discover.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)       77 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/exceptions.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     4674 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/pytest_plugin.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/scripts/
--rwxr-xr-x   0 vitja     (1000) vitja     (1000)      237 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/scripts/mysql-helper
--rwxr-xr-x   0 vitja     (1000) vitja     (1000)     2272 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/scripts/service-mysql
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1584 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/service.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      378 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/utils.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/__init__.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/configs/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      281 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/configs/pg_hba.conf
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/configs/pg_ident.conf
--rw-rw-r--   0 vitja     (1000) vitja     (1000)     1135 2021-11-01 14:48:23.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/configs/postgresql.conf
--rw-rw-r--   0 vitja     (1000) vitja     (1000)     2228 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/connection.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)    11951 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/control.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     7378 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/discover.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)      132 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/exceptions.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)    11034 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/pytest_plugin.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/scripts/
--rw-r--r--   0 vitja     (1000) vitja     (1000)      446 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/scripts/find-pg.sh
--rwxr-xr-x   0 vitja     (1000) vitja     (1000)      203 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/scripts/pgmigrate-helper
--rwxr-xr-x   0 vitja     (1000) vitja     (1000)      244 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/scripts/psql-helper
--rwxr-xr-x   0 vitja     (1000) vitja     (1000)     1741 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/scripts/service-postgresql
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1364 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/service.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     2720 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/testsuite_db.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1393 2022-09-01 14:52:15.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/utils.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/
--rw-r--r--   0 vitja     (1000) vitja     (1000)        0 2022-11-21 16:33:17.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/__init__.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3695 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/classes.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1619 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/pytest_plugin.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/scripts/
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1084 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/scripts/find-rabbitmq.sh
--rwxr-xr-x   0 vitja     (1000) vitja     (1000)     1507 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/scripts/service-rabbitmq
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1826 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/service.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/__init__.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/configs/
--rw-r--r--   0 vitja     (1000) vitja     (1000)      140 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/configs/redis_master.conf.tpl
--rw-r--r--   0 vitja     (1000) vitja     (1000)      284 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/configs/redis_sentinel.conf.tpl
--rw-r--r--   0 vitja     (1000) vitja     (1000)      172 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/configs/redis_slave.conf.tpl
--rw-r--r--   0 vitja     (1000) vitja     (1000)     6397 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/genredis.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3393 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/pytest_plugin.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.389313 yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/scripts/
--rwxr-xr-x   0 vitja     (1000) vitja     (1000)     2041 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/scripts/service-redis
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3558 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/service.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.392646 yandex-taxi-testsuite-0.1.9/testsuite/environment/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/environment/__init__.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)       84 2022-02-24 13:39:17.000000 yandex-taxi-testsuite-0.1.9/testsuite/environment/__main__.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     4403 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/environment/control.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     5349 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/environment/main.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3560 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/environment/pytest_plugin.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.392646 yandex-taxi-testsuite-0.1.9/testsuite/environment/scripts/
--rwxr-xr-x   0 vitja     (1000) vitja     (1000)     2174 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/environment/scripts/utils.sh
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3665 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/environment/service.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     2119 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/environment/shell.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     2588 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/environment/utils.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.392646 yandex-taxi-testsuite-0.1.9/testsuite/logging/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/logging/__init__.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     4161 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/logging/logger.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     2953 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/logging/pytest_plugin.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.392646 yandex-taxi-testsuite-0.1.9/testsuite/mockserver/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9/testsuite/mockserver/__init__.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1393 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/mockserver/classes.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      184 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9/testsuite/mockserver/exceptions.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3602 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/mockserver/magicargs.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     8494 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/mockserver/pytest_plugin.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1549 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/mockserver/reporter_plugin.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)    20961 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/mockserver/server.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.392646 yandex-taxi-testsuite-0.1.9/testsuite/plugins/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/__init__.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)    12195 2023-03-27 14:36:21.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/assertrepr_compare.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)    12040 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/common.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     2017 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/envinfo.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)      368 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/loop.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1692 2023-03-27 14:36:21.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/matching.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3123 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/mocked_time.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      953 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/network.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1419 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/object_hook.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3661 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/servicetest.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3806 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/tcp_mockserver.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3281 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/testpoint.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)      715 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/plugins/verify_file_paths.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)      613 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9/testsuite/pytest_plugin.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.392646 yandex-taxi-testsuite-0.1.9/testsuite/utils/
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      314 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/__init__.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      764 2021-10-18 08:34:13.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/approx.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)      231 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/cached_property.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     4749 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/callinfo.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)      533 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/colors.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)      508 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/compat.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     9977 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/http.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     2036 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/json_util.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     6816 2023-03-27 14:36:21.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/matching.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1057 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/net.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      904 2022-02-22 17:19:51.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/object_hook.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1550 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/ordered_object.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)      424 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/subprocess_helper.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)     1509 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/tskv.py
--rw-rw-r--   0 vitja     (1000) vitja     (1000)      462 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/url_util.py
--rw-r--r--   0 vitja     (1000) vitja     (1000)      795 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9/testsuite/utils/yaml_util.py
-drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-27 14:37:15.395980 yandex-taxi-testsuite-0.1.9/yandex_taxi_testsuite.egg-info/
--rw-r--r--   0 vitja     (1000) vitja     (1000)     3822 2023-03-27 14:37:15.000000 yandex-taxi-testsuite-0.1.9/yandex_taxi_testsuite.egg-info/PKG-INFO
--rw-r--r--   0 vitja     (1000) vitja     (1000)     4820 2023-03-27 14:37:15.000000 yandex-taxi-testsuite-0.1.9/yandex_taxi_testsuite.egg-info/SOURCES.txt
--rw-r--r--   0 vitja     (1000) vitja     (1000)        1 2023-03-27 14:37:15.000000 yandex-taxi-testsuite-0.1.9/yandex_taxi_testsuite.egg-info/dependency_links.txt
--rw-r--r--   0 vitja     (1000) vitja     (1000)        1 2023-03-27 14:36:50.000000 yandex-taxi-testsuite-0.1.9/yandex_taxi_testsuite.egg-info/not-zip-safe
--rw-r--r--   0 vitja     (1000) vitja     (1000)      554 2023-03-27 14:37:15.000000 yandex-taxi-testsuite-0.1.9/yandex_taxi_testsuite.egg-info/requires.txt
--rw-r--r--   0 vitja     (1000) vitja     (1000)       10 2023-03-27 14:37:15.000000 yandex-taxi-testsuite-0.1.9/yandex_taxi_testsuite.egg-info/top_level.txt
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.204344 yandex-taxi-testsuite-0.1.9.1/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)     1097 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/AUTHORS
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1082 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9.1/LICENSE
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3824 2023-03-28 15:48:36.204344 yandex-taxi-testsuite-0.1.9.1/PKG-INFO
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3142 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/README.rst
+-rw-r--r--   0 vitja     (1000) vitja     (1000)       89 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/pyproject.toml
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      567 2023-03-28 15:48:36.204344 yandex-taxi-testsuite-0.1.9.1/setup.cfg
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     2031 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9.1/setup.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.187677 yandex-taxi-testsuite-0.1.9.1/tests/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)     2916 2020-03-11 14:08:30.000000 yandex-taxi-testsuite-0.1.9.1/tests/test_ensure_db_indexes.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     2219 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/tests/test_http.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     4288 2023-03-27 14:36:21.000000 yandex-taxi-testsuite-0.1.9.1/tests/test_json_util.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      858 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/tests/test_loaders.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3663 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/tests/test_ordered_object.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1299 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/tests/test_service_client.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.187677 yandex-taxi-testsuite-0.1.9.1/testsuite/
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      139 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/__init__.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.187677 yandex-taxi-testsuite-0.1.9.1/testsuite/_internal/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/_internal/__init__.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     2498 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/_internal/fixture_class.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      635 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/_internal/fixture_types.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      450 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/annotations.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.191011 yandex-taxi-testsuite-0.1.9.1/testsuite/daemons/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/daemons/__init__.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)    14817 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/daemons/pytest_plugin.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     8750 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/daemons/service_client.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     7019 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/daemons/service_daemon.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     5854 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/daemons/spawn.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.191011 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/__init__.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.191011 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2022-03-18 08:22:00.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/__init__.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      571 2022-03-18 08:22:00.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/classes.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     4019 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/control.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1012 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/discover.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     4831 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/pytest_plugin.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.191011 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/scripts/
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      586 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/scripts/find-clickhouse.sh
+-rwxr-xr-x   0 vitja     (1000) vitja     (1000)     1402 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/scripts/service-clickhouse
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1784 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/service.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      235 2022-03-18 08:22:00.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/utils.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.191011 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/__init__.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1946 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/connection.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3366 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/ensure_db_indexes.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     2948 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/mongo_schema.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)    12123 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/pytest_plugin.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.191011 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/scripts/
+-rwxr-xr-x   0 vitja     (1000) vitja     (1000)     3620 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/scripts/service-mongo
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1877 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/service.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.191011 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/__init__.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)     1119 2021-10-18 08:34:13.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/classes.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     7691 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/control.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1962 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/discover.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)       77 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/exceptions.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     4674 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/pytest_plugin.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.191011 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/scripts/
+-rwxr-xr-x   0 vitja     (1000) vitja     (1000)      227 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/scripts/mysql-helper
+-rwxr-xr-x   0 vitja     (1000) vitja     (1000)     2260 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/scripts/service-mysql
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1584 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/service.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      378 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/utils.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.194344 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/__init__.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.194344 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/configs/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      281 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/configs/pg_hba.conf
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/configs/pg_ident.conf
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)     1135 2021-11-01 14:48:23.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/configs/postgresql.conf
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)     2228 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/connection.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)    11951 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/control.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     7378 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/discover.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      132 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/exceptions.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)    11034 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/pytest_plugin.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.194344 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/scripts/
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      436 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/scripts/find-pg.sh
+-rwxr-xr-x   0 vitja     (1000) vitja     (1000)      192 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/scripts/pgmigrate-helper
+-rwxr-xr-x   0 vitja     (1000) vitja     (1000)      233 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/scripts/psql-helper
+-rwxr-xr-x   0 vitja     (1000) vitja     (1000)     1731 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/scripts/service-postgresql
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1364 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/service.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     2720 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/testsuite_db.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1393 2022-09-01 14:52:15.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/utils.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.194344 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/
+-rw-r--r--   0 vitja     (1000) vitja     (1000)        0 2022-11-21 16:33:17.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/__init__.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3695 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/classes.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1619 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/pytest_plugin.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.194344 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/scripts/
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1074 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/scripts/find-rabbitmq.sh
+-rwxr-xr-x   0 vitja     (1000) vitja     (1000)     1495 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/scripts/service-rabbitmq
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1826 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/service.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.194344 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/__init__.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.194344 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/configs/
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      140 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/configs/redis_master.conf.tpl
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      284 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/configs/redis_sentinel.conf.tpl
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      172 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/configs/redis_slave.conf.tpl
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     6397 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/genredis.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3393 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/pytest_plugin.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.194344 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/scripts/
+-rwxr-xr-x   0 vitja     (1000) vitja     (1000)     2031 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/scripts/service-redis
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3558 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/service.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.197677 yandex-taxi-testsuite-0.1.9.1/testsuite/environment/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/environment/__init__.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)       84 2022-02-24 13:39:17.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/environment/__main__.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     4403 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/environment/control.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     5349 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/environment/main.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3560 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/environment/pytest_plugin.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.197677 yandex-taxi-testsuite-0.1.9.1/testsuite/environment/scripts/
+-rwxr-xr-x   0 vitja     (1000) vitja     (1000)     2163 2023-03-28 15:48:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/environment/scripts/utils.sh
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3665 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/environment/service.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     2119 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/environment/shell.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     2588 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/environment/utils.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.197677 yandex-taxi-testsuite-0.1.9.1/testsuite/logging/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/logging/__init__.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     4161 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/logging/logger.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     2953 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/logging/pytest_plugin.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.197677 yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/__init__.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1393 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/classes.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      184 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/exceptions.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3602 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/magicargs.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     8494 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/pytest_plugin.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1549 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/reporter_plugin.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)    20961 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/server.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.201011 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)        0 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/__init__.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)    12195 2023-03-27 14:36:21.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/assertrepr_compare.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)    12040 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/common.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     2017 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/envinfo.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      368 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/loop.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1692 2023-03-27 14:36:21.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/matching.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3123 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/mocked_time.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      953 2020-09-30 14:17:04.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/network.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1419 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/object_hook.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3661 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/servicetest.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3806 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/tcp_mockserver.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3281 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/testpoint.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      715 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/verify_file_paths.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      613 2023-01-23 11:40:18.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/pytest_plugin.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.201011 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      314 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/__init__.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      764 2021-10-18 08:34:13.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/approx.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      231 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/cached_property.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     4749 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/callinfo.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      533 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/colors.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      508 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/compat.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     9977 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/http.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     2036 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/json_util.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     6816 2023-03-27 14:36:21.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/matching.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1057 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/net.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      904 2022-02-22 17:19:51.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/object_hook.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1550 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/ordered_object.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      424 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/subprocess_helper.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     1509 2023-03-17 08:03:10.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/tskv.py
+-rw-rw-r--   0 vitja     (1000) vitja     (1000)      462 2020-02-18 19:06:39.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/url_util.py
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      795 2022-05-26 10:20:57.000000 yandex-taxi-testsuite-0.1.9.1/testsuite/utils/yaml_util.py
+drwxr-xr-x   0 vitja     (1000) vitja     (1000)        0 2023-03-28 15:48:36.204344 yandex-taxi-testsuite-0.1.9.1/yandex_taxi_testsuite.egg-info/
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     3824 2023-03-28 15:48:36.000000 yandex-taxi-testsuite-0.1.9.1/yandex_taxi_testsuite.egg-info/PKG-INFO
+-rw-r--r--   0 vitja     (1000) vitja     (1000)     4820 2023-03-28 15:48:36.000000 yandex-taxi-testsuite-0.1.9.1/yandex_taxi_testsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 vitja     (1000) vitja     (1000)        1 2023-03-28 15:48:36.000000 yandex-taxi-testsuite-0.1.9.1/yandex_taxi_testsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 vitja     (1000) vitja     (1000)        1 2023-03-27 14:36:50.000000 yandex-taxi-testsuite-0.1.9.1/yandex_taxi_testsuite.egg-info/not-zip-safe
+-rw-r--r--   0 vitja     (1000) vitja     (1000)      554 2023-03-28 15:48:36.000000 yandex-taxi-testsuite-0.1.9.1/yandex_taxi_testsuite.egg-info/requires.txt
+-rw-r--r--   0 vitja     (1000) vitja     (1000)       10 2023-03-28 15:48:36.000000 yandex-taxi-testsuite-0.1.9.1/yandex_taxi_testsuite.egg-info/top_level.txt
```

### Comparing `yandex-taxi-testsuite-0.1.9/AUTHORS` & `yandex-taxi-testsuite-0.1.9.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/LICENSE` & `yandex-taxi-testsuite-0.1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/PKG-INFO` & `yandex-taxi-testsuite-0.1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandex-taxi-testsuite
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: Yandex.Taxi Testsuite Package
 Home-page: https://github.com/yandex/yandex-taxi-testsuite
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yandex/yandex-taxi-testsuite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `yandex-taxi-testsuite-0.1.9/README.rst` & `yandex-taxi-testsuite-0.1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/setup.cfg` & `yandex-taxi-testsuite-0.1.9.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = yandex-taxi-testsuite
-version = 0.1.9
+version = 0.1.9.1
 description = Yandex.Taxi Testsuite Package
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/yandex/yandex-taxi-testsuite
 project_urls = 
 	Bug Tracker = https://github.com/yandex/yandex-taxi-testsuite/issues
 license = MIT
```

### Comparing `yandex-taxi-testsuite-0.1.9/setup.py` & `yandex-taxi-testsuite-0.1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/tests/test_ensure_db_indexes.py` & `yandex-taxi-testsuite-0.1.9.1/tests/test_ensure_db_indexes.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/tests/test_http.py` & `yandex-taxi-testsuite-0.1.9.1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/tests/test_json_util.py` & `yandex-taxi-testsuite-0.1.9.1/tests/test_json_util.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/tests/test_loaders.py` & `yandex-taxi-testsuite-0.1.9.1/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/tests/test_ordered_object.py` & `yandex-taxi-testsuite-0.1.9.1/tests/test_ordered_object.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/tests/test_service_client.py` & `yandex-taxi-testsuite-0.1.9.1/tests/test_service_client.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/_internal/fixture_class.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/_internal/fixture_class.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/_internal/fixture_types.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/_internal/fixture_types.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/daemons/pytest_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/daemons/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/daemons/service_client.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/daemons/service_client.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/daemons/service_daemon.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/daemons/service_daemon.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/daemons/spawn.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/daemons/spawn.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/classes.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/classes.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/control.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/control.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/discover.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/discover.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/pytest_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/scripts/find-clickhouse.sh` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/scripts/find-clickhouse.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#!/usr/bin/env bash
+#!/bin/sh
 
 find_clickhouse() {
     CLICKHOUSE_BINPATH=$(which clickhouse)
-    if [ "x$CLICKHOUSE_BINPATH" == "x" ]; then
+    if [ "x$CLICKHOUSE_BINPATH" = "x" ]; then
         return 1
     fi
     return 0
 }
 
-find_clickhouse || 
+find_clickhouse ||
     die "No clickhouse server binary found.
 
 For debian please run these commands:
-sudo apt update && apt install clickhouse-common-static 
+sudo apt update && apt install clickhouse-common-static
 (https://clickhouse.com/docs/en/getting-started/install/#packages),
 
 For macos follow instructions at https://clickhouse.com/docs/en/getting-started/install/#from-binaries-non-linux
 
 If you already have clickhouse installed, please symlink it to /usr/bin/clickhouse
 "
```

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/scripts/service-clickhouse` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/scripts/service-clickhouse`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env bash
+#!/bin/sh
 
 . $TESTSUITE_LIB_UTILS
 . $(dirname $0)/find-clickhouse.sh
 
 # use ramdisk for clickhouse if available
 RAMDISK="/mnt/ramdisk/$USER"
 if mkdir -p "$RAMDISK" 2> /dev/null; then
```

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/clickhouse/service.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/clickhouse/service.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/connection.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/connection.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/ensure_db_indexes.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/ensure_db_indexes.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/mongo_schema.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/mongo_schema.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/pytest_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/scripts/service-mongo` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/scripts/service-mongo`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env bash
+#!/bin/sh
 
 . $TESTSUITE_LIB_UTILS
 
 MONGO=$(which mongo || which mongosh)
 MONGOD=$(which mongod)
 MONGOS=$(which mongos)
```

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mongo/service.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mongo/service.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/classes.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/classes.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/control.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/control.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/discover.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/discover.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/pytest_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/scripts/service-mysql` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/scripts/service-mysql`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env bash
+#!/bin/sh
 
 . $TESTSUITE_LIB_UTILS
 
 if [ "x$MYSQL_PORT" = "x" ]; then
     die "MYSQL_PORT must be set"
 fi
 if [ "x$MYSQL_TMPDIR" = "x" ]; then
@@ -50,30 +50,30 @@
 
 mysql_die() {
     dump_log_stderr "$MYSQL_LOGFILE"
     die "$@"
 }
 
 initialize_db() {
-    if [ "$DBTYPE" == "mysql" ]; then
+    if [ "$DBTYPE" = "mysql" ]; then
         run_mysqld --initialize-insecure || mysql_die "mysqld initialization failed:
 
 if you see permissions denied error for data directory that may be
 caused by AppArmoor rules. Try this:
 
 $ sudo apt-get install apparmor-utils
 $ sudo aa-disable /usr/sbin/mysqld
 "
     else
         mysql_install_db --auth-root-authentication-method=normal --datadir="$MYSQL_DATADIR" || mysql_die "mysql_install_db failed"
     fi
 }
 
 start_db() {
-    if [ "$DBTYPE" == "mysql" ]; then
+    if [ "$DBTYPE" = "mysql" ]; then
         run_mysqld --daemonize || mysql_die "mysqld_safe start failed"
     else
         run_mysqld -- &
     fi
 }
 
 start() {
```

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/mysql/service.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/mysql/service.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/configs/postgresql.conf` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/configs/postgresql.conf`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/connection.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/connection.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/control.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/control.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/discover.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/discover.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/pytest_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/scripts/service-postgresql` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/scripts/service-postgresql`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env bash
+#!/bin/sh
 
 . $TESTSUITE_LIB_UTILS
 . $(dirname $0)/find-pg.sh
 
 if [ "x$POSTGRESQL_CONFIGS_DIR" = "x" ]; then
     die "POSTGRESQL_CONFIGS_DIR must be set"
 fi
```

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/service.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/service.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/testsuite_db.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/testsuite_db.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/pgsql/utils.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/pgsql/utils.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/classes.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/classes.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/pytest_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/scripts/find-rabbitmq.sh` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/scripts/find-rabbitmq.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env bash
+#!/bin/sh
 
 find_rabbitmq() {
     if [ ! -x "$RABBITMQ_BINDIR/rabbitmq-server" ]; then
         die "No rabbitmq-server script found. 
 Please install RabbitMQ following official instructions at 
 https://www.rabbitmq.com/download.html 
 or set TESTSUITE_RABBITMQ_BINDIR environment variable to the directory containing
```

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/scripts/service-rabbitmq` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/scripts/service-rabbitmq`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env bash
+#!/bin/sh
 
 . $TESTSUITE_LIB_UTILS
 . $(dirname $0)/find-rabbitmq.sh
 
 # use ramdisk for rabbitmq if available
 RAMDISK="/mnt/ramdisk/$USER"
 if mkdir -p "$RAMDISK" 2> /dev/null; then
@@ -18,16 +18,16 @@
 if [ "x$RABBITMQ_EPMD_PORT" = "x" ]; then
     die "RABBITMQ_EPMD_PORT must be set"
 fi
 
 RABBITMQ_DATA_DIR=$RABBITMQ_TMPDIR/mnesia
 RABBITMQ_LOG_DIR=$RABBITMQ_TMPDIR/log
 RABBITMQ_STARTUP_LOG=$RABBITMQ_LOG_DIR/startup.log
-RABBITMQ_NODENAME='testsuite@localhost' 
-V_RABBITMQ_ERLANG_COOKIE='testsuite' 
+RABBITMQ_NODENAME='testsuite@localhost'
+V_RABBITMQ_ERLANG_COOKIE='testsuite'
 
 export ERL_EPMD_PORT="$RABBITMQ_EPMD_PORT"
 export RABBITMQ_MNESIA_BASE="$RABBITMQ_DATA_DIR"
 export RABBITMQ_LOG_BASE="$RABBITMQ_LOG_DIR"
 export RABBITMQ_NODE_PORT="$RABBITMQ_TCP_PORT"
 export RABBITMQ_NODENAME="$RABBITMQ_NODENAME"
 export RABBITMQ_ERLANG_COOKIE="$V_RABBITMQ_ERLANG_COOKIE"
```

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/rabbitmq/service.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/rabbitmq/service.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/genredis.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/genredis.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/pytest_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/scripts/service-redis` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/scripts/service-redis`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env bash
+#!/bin/sh
 
 . $TESTSUITE_LIB_UTILS
 
 if [ "x$REDIS_TMPDIR" = "x" ]; then
     die "REDIS_TMPDIR must be set"
 fi
 if [ "x$REDIS_CONFIGS_DIR" = "x" ]; then
```

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/databases/redis/service.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/databases/redis/service.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/environment/control.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/environment/control.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/environment/main.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/environment/main.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/environment/pytest_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/environment/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/environment/scripts/utils.sh` & `yandex-taxi-testsuite-0.1.9.1/testsuite/environment/scripts/utils.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env bash
+#!/bin/sh
 
 PATH=$PATH:/usr/sbin:/sbin
 START_STOP_DAEMON=$(which start-stop-daemon 2>/dev/null)
 
 die() {
     echo "$@" >&2
     exit 1
@@ -39,15 +39,15 @@
     if [ "x$START_STOP_DAEMON" != "x" ]; then
         $START_STOP_DAEMON --stop --retry TERM/5/KILL/3 \
                            -p $pidfile $binary 2> /dev/null >&2
     else
         # MacOS X workaround
         for i in `seq 10`; do
             if [ -f "$pidfile" ]; then
-                if [ $i == "1" ]; then
+                if [ $i = "1" ]; then
                     kill -TERM $(cat "$pidfile")
                 else
                     kill -TERM $(cat "$pidfile") 2> /dev/null >&2
                 fi
             else
                 break
             fi
```

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/environment/service.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/environment/service.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/environment/shell.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/environment/shell.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/environment/utils.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/environment/utils.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/logging/logger.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/logging/logger.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/logging/pytest_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/logging/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/mockserver/classes.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/classes.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/mockserver/magicargs.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/magicargs.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/mockserver/pytest_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/mockserver/reporter_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/reporter_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/mockserver/server.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/mockserver/server.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/plugins/assertrepr_compare.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/assertrepr_compare.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/plugins/common.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/common.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/plugins/envinfo.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/envinfo.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/plugins/matching.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/matching.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/plugins/mocked_time.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/mocked_time.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/plugins/network.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/network.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/plugins/object_hook.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/object_hook.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/plugins/servicetest.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/servicetest.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/plugins/tcp_mockserver.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/tcp_mockserver.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/plugins/testpoint.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/testpoint.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/plugins/verify_file_paths.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/plugins/verify_file_paths.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/pytest_plugin.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/utils/approx.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/utils/approx.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/utils/callinfo.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/utils/callinfo.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/utils/colors.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/utils/colors.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/utils/http.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/utils/http.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/utils/json_util.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/utils/matching.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/utils/matching.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/utils/net.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/utils/net.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/utils/object_hook.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/utils/object_hook.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/utils/ordered_object.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/utils/ordered_object.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/utils/tskv.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/utils/tskv.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/testsuite/utils/yaml_util.py` & `yandex-taxi-testsuite-0.1.9.1/testsuite/utils/yaml_util.py`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/yandex_taxi_testsuite.egg-info/PKG-INFO` & `yandex-taxi-testsuite-0.1.9.1/yandex_taxi_testsuite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandex-taxi-testsuite
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: Yandex.Taxi Testsuite Package
 Home-page: https://github.com/yandex/yandex-taxi-testsuite
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yandex/yandex-taxi-testsuite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `yandex-taxi-testsuite-0.1.9/yandex_taxi_testsuite.egg-info/SOURCES.txt` & `yandex-taxi-testsuite-0.1.9.1/yandex_taxi_testsuite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yandex-taxi-testsuite-0.1.9/yandex_taxi_testsuite.egg-info/requires.txt` & `yandex-taxi-testsuite-0.1.9.1/yandex_taxi_testsuite.egg-info/requires.txt`

 * *Files identical despite different names*


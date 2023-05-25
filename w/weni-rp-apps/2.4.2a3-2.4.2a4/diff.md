# Comparing `tmp/weni_rp_apps-2.4.2a3.tar.gz` & `tmp/weni_rp_apps-2.4.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weni_rp_apps-2.4.2a3.tar", max compression
+gzip compressed data, was "weni_rp_apps-2.4.2a4.tar", max compression
```

## Comparing `weni_rp_apps-2.4.2a3.tar` & `weni_rp_apps-2.4.2a4.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0      646 2023-05-23 20:42:42.108698 weni_rp_apps-2.4.2a3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/activities/__init__.py
--rw-r--r--   0        0        0      245 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/activities/apps.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/activities/migrations/__init__.py
--rw-r--r--   0        0        0     2096 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/activities/signals.py
--rw-r--r--   0        0        0      366 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/activities/tasks.py
--rw-r--r--   0        0        0      325 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/analytics_api/README.md
--rw-r--r--   0        0        0       66 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/analytics_api/__init__.py
--rw-r--r--   0        0        0      264 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/analytics_api/apps.py
--rw-r--r--   0        0        0    13526 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/analytics_api/tests.py
--rw-r--r--   0        0        0      535 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/analytics_api/urls.py
--rw-r--r--   0        0        0     9016 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/analytics_api/views.py
--rw-r--r--   0        0        0       49 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/auth/__init__.py
--rw-r--r--   0        0        0      285 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/auth/apps.py
--rw-r--r--   0        0        0     1321 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/auth/backends.py
--rw-r--r--   0        0        0      430 2023-05-23 20:42:23.144657 weni_rp_apps-2.4.2a3/weni/auth/decorators.py
--rw-r--r--   0        0        0      810 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/auth/urls.py
--rw-r--r--   0        0        0     2645 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/auth/views.py
--rw-r--r--   0        0        0      309 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/channel_stats/README.md
--rw-r--r--   0        0        0       66 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/channel_stats/__init__.py
--rw-r--r--   0        0        0      264 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/channel_stats/apps.py
--rw-r--r--   0        0        0     6157 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/channel_stats/serializers.py
--rw-r--r--   0        0        0      347 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/channel_stats/urls.py
--rw-r--r--   0        0        0     3575 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/channel_stats/views.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/billing/__init__.py
--rw-r--r--   0        0        0      102 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/billing/apps.py
--rw-r--r--   0        0        0     3508 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/billing/queries.py
--rw-r--r--   0        0        0     3194 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/billing/serializers.py
--rw-r--r--   0        0        0     2063 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/billing/services.py
--rw-r--r--   0        0        0    11364 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/billing/tests.py
--rw-r--r--   0        0        0      231 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/billing/urls.py
--rw-r--r--   0        0        0       64 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/channel/__init__.py
--rw-r--r--   0        0        0      103 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/channel/apps.py
--rw-r--r--   0        0        0      352 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/channel/fields.py
--rw-r--r--   0        0        0     4070 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/channel/serializers.py
--rw-r--r--   0        0        0     4081 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/channel/services.py
--rw-r--r--   0        0        0     7987 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/channel/tests.py
--rw-r--r--   0        0        0      341 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/channel/urls.py
--rw-r--r--   0        0        0       70 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/classifier/__init__.py
--rw-r--r--   0        0        0      109 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/classifier/apps.py
--rw-r--r--   0        0        0     1356 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/classifier/serializers.py
--rw-r--r--   0        0        0     1174 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/classifier/services.py
--rw-r--r--   0        0        0     6493 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/classifier/tests.py
--rw-r--r--   0        0        0      249 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/classifier/urls.py
--rw-r--r--   0        0        0       61 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/core/__init__.py
--rw-r--r--   0        0        0      100 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/core/apps.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/core/management/commands/__init__.py
--rw-r--r--   0        0        0     1588 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/core/management/commands/grpc.py
--rw-r--r--   0        0        0     1213 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/core/serializers.py
--rw-r--r--   0        0        0      965 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/core/services.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/core/tests.py
--rw-r--r--   0        0        0      700 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/core/urls.py
--rw-r--r--   0        0        0       58 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/flow/__init__.py
--rw-r--r--   0        0        0       97 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/flow/apps.py
--rw-r--r--   0        0        0      307 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/flow/serializers.py
--rw-r--r--   0        0        0      680 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/flow/services.py
--rw-r--r--   0        0        0     2764 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/flow/tests.py
--rw-r--r--   0        0        0      213 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/flow/urls.py
--rw-r--r--   0        0        0       56 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/org/__init__.py
--rw-r--r--   0        0        0       95 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/org/apps.py
--rw-r--r--   0        0        0     2836 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/org/serializers.py
--rw-r--r--   0        0        0     4020 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/org/services.py
--rw-r--r--   0        0        0     9821 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/org/tests.py
--rw-r--r--   0        0        0      207 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/org/urls.py
--rw-r--r--   0        0        0       68 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/statistic/__init__.py
--rw-r--r--   0        0        0      107 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/statistic/apps.py
--rw-r--r--   0        0        0      672 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/statistic/services.py
--rw-r--r--   0        0        0     3132 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/statistic/tests.py
--rw-r--r--   0        0        0      252 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/statistic/urls.py
--rw-r--r--   0        0        0       58 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/user/__init__.py
--rw-r--r--   0        0        0       97 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/user/apps.py
--rw-r--r--   0        0        0      843 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/user/serializers.py
--rw-r--r--   0        0        0     3916 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/user/services.py
--rw-r--r--   0        0        0    10076 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/user/tests.py
--rw-r--r--   0        0        0      347 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/grpc/user/urls.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/__init__.py
--rw-r--r--   0        0        0      328 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/apps.py
--rw-r--r--   0        0        0      300 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/authenticators.py
--rw-r--r--   0        0        0     1374 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/backends.py
--rw-r--r--   0        0        0     5484 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/channel/serializers.py
--rw-r--r--   0        0        0    16305 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/channel/tests.py
--rw-r--r--   0        0        0      394 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/channel/urls.py
--rw-r--r--   0        0        0     7611 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/channel/views.py
--rw-r--r--   0        0        0     1527 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/classifier/serializers.py
--rw-r--r--   0        0        0     8626 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/classifier/tests.py
--rw-r--r--   0        0        0      318 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/classifier/urls.py
--rw-r--r--   0        0        0     2803 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/classifier/views.py
--rw-r--r--   0        0        0       34 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/clients/__init__.py
--rw-r--r--   0        0        0      692 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/clients/authenticators.py
--rw-r--r--   0        0        0      486 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/clients/base.py
--rw-r--r--   0        0        0      681 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/clients/connect.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/externals/__init__.py
--rw-r--r--   0        0        0     1307 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/externals/serializers.py
--rw-r--r--   0        0        0      294 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/externals/urls.py
--rw-r--r--   0        0        0     1501 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/externals/views.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/flows/__init__.py
--rw-r--r--   0        0        0     1278 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/flows/serializers.py
--rw-r--r--   0        0        0     4318 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/flows/tests.py
--rw-r--r--   0        0        0      308 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/flows/urls.py
--rw-r--r--   0        0        0      974 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/flows/views.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/globals/__init__.py
--rw-r--r--   0        0        0     2286 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/globals/serializers.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/globals/tests/__init__.py
--rw-r--r--   0        0        0     2183 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/globals/tests/test_serializers.py
--rw-r--r--   0        0        0      220 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/globals/urls.py
--rw-r--r--   0        0        0     1484 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/globals/views.py
--rw-r--r--   0        0        0     1247 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/migrations/0001_initial.py
--rw-r--r--   0        0        0     1032 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/migrations/0002_project.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/migrations/__init__.py
--rw-r--r--   0        0        0      916 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/models.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/orgs/__init__.py
--rw-r--r--   0        0        0     3976 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/orgs/serializers.py
--rw-r--r--   0        0        0    14533 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/orgs/tests.py
--rw-r--r--   0        0        0      300 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/orgs/urls.py
--rw-r--r--   0        0        0     4592 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/orgs/views.py
--rw-r--r--   0        0        0      246 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/permissions.py
--rw-r--r--   0        0        0     1993 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/statistic/tests.py
--rw-r--r--   0        0        0      205 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/statistic/urls.py
--rw-r--r--   0        0        0      944 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/statistic/views.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/tests/__init__.py
--rw-r--r--   0        0        0     1249 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/tests/test_models.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/tickets/__init__.py
--rw-r--r--   0        0        0     1150 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/tickets/serializers.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/tickets/tests/__init__.py
--rw-r--r--   0        0        0     3360 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/tickets/tests/test_views.py
--rw-r--r--   0        0        0      443 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/tickets/urls.py
--rw-r--r--   0        0        0     1827 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/tickets/views.py
--rw-r--r--   0        0        0     1315 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/urls.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/users/__init__.py
--rw-r--r--   0        0        0      845 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/users/serializers.py
--rw-r--r--   0        0        0    12563 2023-05-23 20:42:23.148657 weni_rp_apps-2.4.2a3/weni/internal/users/tests.py
--rw-r--r--   0        0        0      711 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/internal/users/urls.py
--rw-r--r--   0        0        0     5849 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/internal/users/views.py
--rw-r--r--   0        0        0      555 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/internal/views.py
--rw-r--r--   0        0        0       55 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/orgs_api/__init__.py
--rw-r--r--   0        0        0      253 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/orgs_api/apps.py
--rw-r--r--   0        0        0      906 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/orgs_api/serializers.py
--rw-r--r--   0        0        0     4030 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/orgs_api/tests.py
--rw-r--r--   0        0        0      178 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/orgs_api/urls.py
--rw-r--r--   0        0        0     1444 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/orgs_api/views.py
--rw-r--r--   0        0        0       45 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/s3/__init__.py
--rw-r--r--   0        0        0      243 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/s3/apps.py
--rw-r--r--   0        0        0      219 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/s3/urls.py
--rw-r--r--   0        0        0      550 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/s3/views.py
--rw-r--r--   0        0        0       93 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/serializers/__init__.py
--rw-r--r--   0        0        0      725 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/serializers/fields.py
--rw-r--r--   0        0        0      281 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/success_orgs/apps.py
--rw-r--r--   0        0        0     2521 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/success_orgs/business.py
--rw-r--r--   0        0        0      563 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/success_orgs/serializers.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/success_orgs/tests/__init__.py
--rw-r--r--   0        0        0     2980 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/success_orgs/tests/test_business.py
--rw-r--r--   0        0        0      494 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/success_orgs/urls.py
--rw-r--r--   0        0        0     2770 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/success_orgs/views.py
--rw-r--r--   0        0        0      318 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/template_message/README.md
--rw-r--r--   0        0        0       72 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/template_message/__init__.py
--rw-r--r--   0        0        0      294 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/template_message/apps.py
--rw-r--r--   0        0        0     2040 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/template_message/serializers.py
--rw-r--r--   0        0        0     5292 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/template_message/tests.py
--rw-r--r--   0        0        0      344 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/template_message/urls.py
--rw-r--r--   0        0        0     1651 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/template_message/views.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/templates/__init__.py
--rw-r--r--   0        0        0      545 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/templates/context_processors.py
--rw-r--r--   0        0        0      315 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/ticketer_queues/README.md
--rw-r--r--   0        0        0       70 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/ticketer_queues/__init__.py
--rw-r--r--   0        0        0      291 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/ticketer_queues/apps.py
--rw-r--r--   0        0        0      242 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/ticketer_queues/serializers.py
--rw-r--r--   0        0        0     1584 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/ticketer_queues/tests.py
--rw-r--r--   0        0        0      378 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/ticketer_queues/urls.py
--rw-r--r--   0        0        0      849 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/ticketer_queues/views.py
--rw-r--r--   0        0        0        0 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/utils/__init__.py
--rw-r--r--   0        0        0     1091 2023-05-23 20:42:23.152657 weni_rp_apps-2.4.2a3/weni/utils/app_config.py
--rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.4.2a3/PKG-INFO
+-rw-r--r--   0        0        0      646 2023-05-25 21:33:01.504262 weni_rp_apps-2.4.2a4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/activities/__init__.py
+-rw-r--r--   0        0        0      245 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/activities/apps.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/activities/migrations/__init__.py
+-rw-r--r--   0        0        0     2096 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/activities/signals.py
+-rw-r--r--   0        0        0      366 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/activities/tasks.py
+-rw-r--r--   0        0        0      325 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/analytics_api/README.md
+-rw-r--r--   0        0        0       66 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/analytics_api/__init__.py
+-rw-r--r--   0        0        0      264 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/analytics_api/apps.py
+-rw-r--r--   0        0        0    13526 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/analytics_api/tests.py
+-rw-r--r--   0        0        0      535 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/analytics_api/urls.py
+-rw-r--r--   0        0        0     9016 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/analytics_api/views.py
+-rw-r--r--   0        0        0       49 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/auth/__init__.py
+-rw-r--r--   0        0        0      285 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/auth/apps.py
+-rw-r--r--   0        0        0     1321 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/auth/backends.py
+-rw-r--r--   0        0        0      430 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/auth/decorators.py
+-rw-r--r--   0        0        0      810 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/auth/urls.py
+-rw-r--r--   0        0        0     2645 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/auth/views.py
+-rw-r--r--   0        0        0      309 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/channel_stats/README.md
+-rw-r--r--   0        0        0       66 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/channel_stats/__init__.py
+-rw-r--r--   0        0        0      264 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/channel_stats/apps.py
+-rw-r--r--   0        0        0     6157 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/channel_stats/serializers.py
+-rw-r--r--   0        0        0      347 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/channel_stats/urls.py
+-rw-r--r--   0        0        0     3575 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/channel_stats/views.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/billing/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/billing/apps.py
+-rw-r--r--   0        0        0     3508 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/billing/queries.py
+-rw-r--r--   0        0        0     3194 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/billing/serializers.py
+-rw-r--r--   0        0        0     2063 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/billing/services.py
+-rw-r--r--   0        0        0    11364 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/billing/tests.py
+-rw-r--r--   0        0        0      231 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/billing/urls.py
+-rw-r--r--   0        0        0       64 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/channel/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/channel/apps.py
+-rw-r--r--   0        0        0      352 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/channel/fields.py
+-rw-r--r--   0        0        0     4070 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/channel/serializers.py
+-rw-r--r--   0        0        0     4081 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/channel/services.py
+-rw-r--r--   0        0        0     7987 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/channel/tests.py
+-rw-r--r--   0        0        0      341 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/channel/urls.py
+-rw-r--r--   0        0        0       70 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/classifier/__init__.py
+-rw-r--r--   0        0        0      109 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/classifier/apps.py
+-rw-r--r--   0        0        0     1356 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/classifier/serializers.py
+-rw-r--r--   0        0        0     1174 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/classifier/services.py
+-rw-r--r--   0        0        0     6493 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/classifier/tests.py
+-rw-r--r--   0        0        0      249 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/classifier/urls.py
+-rw-r--r--   0        0        0       61 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/core/__init__.py
+-rw-r--r--   0        0        0      100 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/core/apps.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.887837 weni_rp_apps-2.4.2a4/weni/grpc/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     1588 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/core/management/commands/grpc.py
+-rw-r--r--   0        0        0     1213 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/core/serializers.py
+-rw-r--r--   0        0        0      965 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/core/services.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/core/tests.py
+-rw-r--r--   0        0        0      700 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/core/urls.py
+-rw-r--r--   0        0        0       58 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/flow/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/flow/apps.py
+-rw-r--r--   0        0        0      307 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/flow/serializers.py
+-rw-r--r--   0        0        0      680 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/flow/services.py
+-rw-r--r--   0        0        0     2764 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/flow/tests.py
+-rw-r--r--   0        0        0      213 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/flow/urls.py
+-rw-r--r--   0        0        0       56 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/org/__init__.py
+-rw-r--r--   0        0        0       95 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/org/apps.py
+-rw-r--r--   0        0        0     2836 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/org/serializers.py
+-rw-r--r--   0        0        0     4020 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/org/services.py
+-rw-r--r--   0        0        0     9821 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/org/tests.py
+-rw-r--r--   0        0        0      207 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/org/urls.py
+-rw-r--r--   0        0        0       68 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/statistic/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/statistic/apps.py
+-rw-r--r--   0        0        0      672 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/statistic/services.py
+-rw-r--r--   0        0        0     3132 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/statistic/tests.py
+-rw-r--r--   0        0        0      252 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/statistic/urls.py
+-rw-r--r--   0        0        0       58 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/user/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/user/apps.py
+-rw-r--r--   0        0        0      843 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/user/serializers.py
+-rw-r--r--   0        0        0     3916 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/user/services.py
+-rw-r--r--   0        0        0    10076 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/user/tests.py
+-rw-r--r--   0        0        0      347 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/grpc/user/urls.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/apps.py
+-rw-r--r--   0        0        0      300 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/authenticators.py
+-rw-r--r--   0        0        0     1374 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/backends.py
+-rw-r--r--   0        0        0     5484 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/channel/serializers.py
+-rw-r--r--   0        0        0    16305 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/channel/tests.py
+-rw-r--r--   0        0        0      394 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/channel/urls.py
+-rw-r--r--   0        0        0     7310 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/channel/views.py
+-rw-r--r--   0        0        0     1527 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/classifier/serializers.py
+-rw-r--r--   0        0        0     8626 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/classifier/tests.py
+-rw-r--r--   0        0        0      318 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/classifier/urls.py
+-rw-r--r--   0        0        0     2803 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/classifier/views.py
+-rw-r--r--   0        0        0       34 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/clients/__init__.py
+-rw-r--r--   0        0        0      692 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/clients/authenticators.py
+-rw-r--r--   0        0        0      486 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/clients/base.py
+-rw-r--r--   0        0        0      681 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/clients/connect.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/externals/__init__.py
+-rw-r--r--   0        0        0     1388 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/externals/serializers.py
+-rw-r--r--   0        0        0      542 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/externals/urls.py
+-rw-r--r--   0        0        0     4841 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/externals/views.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/flows/__init__.py
+-rw-r--r--   0        0        0     1278 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/flows/serializers.py
+-rw-r--r--   0        0        0     4318 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/flows/tests.py
+-rw-r--r--   0        0        0      308 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/flows/urls.py
+-rw-r--r--   0        0        0      974 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/flows/views.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/globals/__init__.py
+-rw-r--r--   0        0        0     2286 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/globals/serializers.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/globals/tests/__init__.py
+-rw-r--r--   0        0        0     2183 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/globals/tests/test_serializers.py
+-rw-r--r--   0        0        0      220 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/globals/urls.py
+-rw-r--r--   0        0        0     1484 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/globals/views.py
+-rw-r--r--   0        0        0     1247 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1032 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/migrations/0002_project.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/migrations/__init__.py
+-rw-r--r--   0        0        0      916 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/models.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/orgs/__init__.py
+-rw-r--r--   0        0        0     3976 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/orgs/serializers.py
+-rw-r--r--   0        0        0    14533 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/orgs/tests.py
+-rw-r--r--   0        0        0      300 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/orgs/urls.py
+-rw-r--r--   0        0        0     4592 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/orgs/views.py
+-rw-r--r--   0        0        0      246 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/permissions.py
+-rw-r--r--   0        0        0     1993 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/statistic/tests.py
+-rw-r--r--   0        0        0      205 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/statistic/urls.py
+-rw-r--r--   0        0        0      944 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/statistic/views.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/tests/__init__.py
+-rw-r--r--   0        0        0     1249 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/tests/test_models.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/tickets/__init__.py
+-rw-r--r--   0        0        0     1150 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/tickets/serializers.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/tickets/tests/__init__.py
+-rw-r--r--   0        0        0     3360 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/tickets/tests/test_views.py
+-rw-r--r--   0        0        0      443 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/tickets/urls.py
+-rw-r--r--   0        0        0     1844 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/tickets/views.py
+-rw-r--r--   0        0        0     1315 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/urls.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/users/__init__.py
+-rw-r--r--   0        0        0      845 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/users/serializers.py
+-rw-r--r--   0        0        0    12563 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/users/tests.py
+-rw-r--r--   0        0        0      711 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/users/urls.py
+-rw-r--r--   0        0        0     5849 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/users/views.py
+-rw-r--r--   0        0        0      555 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/internal/views.py
+-rw-r--r--   0        0        0       55 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/orgs_api/__init__.py
+-rw-r--r--   0        0        0      253 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/orgs_api/apps.py
+-rw-r--r--   0        0        0      906 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/orgs_api/serializers.py
+-rw-r--r--   0        0        0     4030 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/orgs_api/tests.py
+-rw-r--r--   0        0        0      178 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/orgs_api/urls.py
+-rw-r--r--   0        0        0     1444 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/orgs_api/views.py
+-rw-r--r--   0        0        0       45 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/s3/__init__.py
+-rw-r--r--   0        0        0      243 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/s3/apps.py
+-rw-r--r--   0        0        0      219 2023-05-25 21:32:42.891837 weni_rp_apps-2.4.2a4/weni/s3/urls.py
+-rw-r--r--   0        0        0      550 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/s3/views.py
+-rw-r--r--   0        0        0       93 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/serializers/__init__.py
+-rw-r--r--   0        0        0      725 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/serializers/fields.py
+-rw-r--r--   0        0        0      281 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/success_orgs/apps.py
+-rw-r--r--   0        0        0     2521 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/success_orgs/business.py
+-rw-r--r--   0        0        0      563 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/success_orgs/serializers.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/success_orgs/tests/__init__.py
+-rw-r--r--   0        0        0     2980 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/success_orgs/tests/test_business.py
+-rw-r--r--   0        0        0      494 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/success_orgs/urls.py
+-rw-r--r--   0        0        0     2770 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/success_orgs/views.py
+-rw-r--r--   0        0        0      318 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/template_message/README.md
+-rw-r--r--   0        0        0       72 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/template_message/__init__.py
+-rw-r--r--   0        0        0      294 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/template_message/apps.py
+-rw-r--r--   0        0        0     2040 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/template_message/serializers.py
+-rw-r--r--   0        0        0     5292 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/template_message/tests.py
+-rw-r--r--   0        0        0      344 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/template_message/urls.py
+-rw-r--r--   0        0        0     1651 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/template_message/views.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/templates/__init__.py
+-rw-r--r--   0        0        0      545 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/templates/context_processors.py
+-rw-r--r--   0        0        0      315 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/ticketer_queues/README.md
+-rw-r--r--   0        0        0       70 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/ticketer_queues/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/ticketer_queues/apps.py
+-rw-r--r--   0        0        0      242 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/ticketer_queues/serializers.py
+-rw-r--r--   0        0        0     1584 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/ticketer_queues/tests.py
+-rw-r--r--   0        0        0      378 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/ticketer_queues/urls.py
+-rw-r--r--   0        0        0      849 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/ticketer_queues/views.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/utils/__init__.py
+-rw-r--r--   0        0        0     1091 2023-05-25 21:32:42.895837 weni_rp_apps-2.4.2a4/weni/utils/app_config.py
+-rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.4.2a4/PKG-INFO
```

### Comparing `weni_rp_apps-2.4.2a3/pyproject.toml` & `weni_rp_apps-2.4.2a4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weni-rp-apps"
-version = "2.4.2a3"
+version = "2.4.2a4"
 description = "Weni apps for Rapidpro Platform"
 authors = ["jcbalmeida"]
 license = "AGPL-3.0"
 packages = [
     { include = "weni" }
 ]
```

### Comparing `weni_rp_apps-2.4.2a3/weni/activities/signals.py` & `weni_rp_apps-2.4.2a4/weni/activities/signals.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/analytics_api/tests.py` & `weni_rp_apps-2.4.2a4/weni/analytics_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/analytics_api/urls.py` & `weni_rp_apps-2.4.2a4/weni/analytics_api/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/analytics_api/views.py` & `weni_rp_apps-2.4.2a4/weni/analytics_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/auth/backends.py` & `weni_rp_apps-2.4.2a4/weni/auth/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/auth/urls.py` & `weni_rp_apps-2.4.2a4/weni/auth/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/auth/views.py` & `weni_rp_apps-2.4.2a4/weni/auth/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/channel_stats/serializers.py` & `weni_rp_apps-2.4.2a4/weni/channel_stats/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/channel_stats/views.py` & `weni_rp_apps-2.4.2a4/weni/channel_stats/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/billing/queries.py` & `weni_rp_apps-2.4.2a4/weni/grpc/billing/queries.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/billing/serializers.py` & `weni_rp_apps-2.4.2a4/weni/grpc/billing/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/billing/services.py` & `weni_rp_apps-2.4.2a4/weni/grpc/billing/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/billing/tests.py` & `weni_rp_apps-2.4.2a4/weni/grpc/billing/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/channel/serializers.py` & `weni_rp_apps-2.4.2a4/weni/grpc/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/channel/services.py` & `weni_rp_apps-2.4.2a4/weni/grpc/channel/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/channel/tests.py` & `weni_rp_apps-2.4.2a4/weni/grpc/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/classifier/serializers.py` & `weni_rp_apps-2.4.2a4/weni/grpc/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/classifier/services.py` & `weni_rp_apps-2.4.2a4/weni/grpc/classifier/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/classifier/tests.py` & `weni_rp_apps-2.4.2a4/weni/grpc/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/core/management/commands/grpc.py` & `weni_rp_apps-2.4.2a4/weni/grpc/core/management/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/core/serializers.py` & `weni_rp_apps-2.4.2a4/weni/grpc/core/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/core/services.py` & `weni_rp_apps-2.4.2a4/weni/grpc/core/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/core/urls.py` & `weni_rp_apps-2.4.2a4/weni/grpc/core/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/flow/services.py` & `weni_rp_apps-2.4.2a4/weni/grpc/flow/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/flow/tests.py` & `weni_rp_apps-2.4.2a4/weni/grpc/flow/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/org/serializers.py` & `weni_rp_apps-2.4.2a4/weni/grpc/org/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/org/services.py` & `weni_rp_apps-2.4.2a4/weni/grpc/org/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/org/tests.py` & `weni_rp_apps-2.4.2a4/weni/grpc/org/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/statistic/services.py` & `weni_rp_apps-2.4.2a4/weni/grpc/statistic/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/statistic/tests.py` & `weni_rp_apps-2.4.2a4/weni/grpc/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/user/serializers.py` & `weni_rp_apps-2.4.2a4/weni/grpc/user/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/user/services.py` & `weni_rp_apps-2.4.2a4/weni/grpc/user/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/grpc/user/tests.py` & `weni_rp_apps-2.4.2a4/weni/grpc/user/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/backends.py` & `weni_rp_apps-2.4.2a4/weni/internal/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/channel/serializers.py` & `weni_rp_apps-2.4.2a4/weni/internal/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/channel/tests.py` & `weni_rp_apps-2.4.2a4/weni/internal/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/channel/views.py` & `weni_rp_apps-2.4.2a4/weni/internal/channel/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,25 +43,21 @@
 
     def retrieve(self, request, uuid=None):
         try:
             channel = Channel.objects.get(uuid=uuid)
         except Channel.DoesNotExist:
             return Response(status=status.HTTP_404_NOT_FOUND)
 
-        return JsonResponse(
-            data=self.get_serializer(channel).data, status=status.HTTP_200_OK
-        )
+        return JsonResponse(data=self.get_serializer(channel).data, status=status.HTTP_200_OK)
 
     def create(self, request):
         serializer = CreateChannelSerializer(data=request.data)
 
         if not serializer.is_valid():
-            return JsonResponse(
-                data=serializer.errors, status=status.HTTP_400_BAD_REQUEST
-            )
+            return JsonResponse(data=serializer.errors, status=status.HTTP_400_BAD_REQUEST)
 
         serializer.save()
 
         return JsonResponse(data=serializer.data, status=status.HTTP_200_OK)
 
     def destroy(self, request, uuid=None):
         channel = get_object_or_404(Channel, uuid=uuid)
@@ -72,17 +68,15 @@
         return Response(status=status.HTTP_200_OK)
 
     @action(methods=["POST"], detail=False)
     def create_wac(self, request):
         serializer = ChannelWACSerializer(data=request.data)
 
         if not serializer.is_valid():
-            return JsonResponse(
-                data=serializer.errors, status=status.HTTP_400_BAD_REQUEST
-            )
+            return JsonResponse(data=serializer.errors, status=status.HTTP_400_BAD_REQUEST)
 
         serializer.save()
 
         return JsonResponse(data=serializer.data, status=status.HTTP_200_OK)
 
 
 class AvailableChannels(viewsets.ViewSet, InternalGenericViewSet):
@@ -155,19 +149,15 @@
         "claim_view_kwargs",
         "extra_links",
         "redact_request_keys",
     ]
 
     for i in _class.__class__.__dict__.items():
         if not i[0].startswith("_"):
-            if (
-                not inspect.isclass(i[1])
-                and str(type(i[1])) not in (type_exclude)
-                and i[0] not in items_exclude
-            ):
+            if not inspect.isclass(i[1]) and str(type(i[1])) not in (type_exclude) and i[0] not in items_exclude:
                 if str(type(i[1])) == "<enum 'Category'>":
                     channel[i[0]] = {
                         "name": i[1].name if i[1].name else "",
                         "value": i[1].value if i[1].value else "",
                     }
 
                 elif i[0] == "configuration_urls":
@@ -179,17 +169,15 @@
                                 if url.get("label"):
                                     url_dict["label"] = str(url.get("label"))
 
                                 if i[1][0].get("url"):
                                     url_dict["url"] = str(url.get("url"))
 
                                 if i[1][0].get("description"):
-                                    url_dict["description"] = str(
-                                        url.get("description")
-                                    )
+                                    url_dict["description"] = str(url.get("description"))
 
                             urls_list.append(url_dict)
                             channel[i[0]] = urls_list
 
                 elif i[0] == "configuration_blurb":
                     channel[i[0]] = str(i[1])
 
@@ -200,33 +188,29 @@
                     channel[i[0]] = {
                         "name": i[1].name if i[1].name else "",
                         "value": i[1].value if i[1].value else "",
                     }
                 else:
                     channel[i[0]] = i[1]
 
-    if (
-        (not (channel.get("code")))
-        or (not (len(channel)) > 0)
-        or (not (channel.get("name")))
-    ):
+    if (not (channel.get("code"))) or (not (len(channel)) > 0) or (not (channel.get("name"))):
         return None
 
     channel["num_fields"] = len(channel)
     return channel
 
 
 def extract_form_info(_form, name_form):
     detail = {}
     detail["name"] = name_form if name_form else None
 
     try:
         detail["type"] = str(_form.widget.input_type)
-    except AttributeError:
-        detail["type"] = str(_form.widget.__class__.__name__).lower()
+    except Exception:
+        detail["type"] = None
 
     if _form.help_text:
         detail["help_text"] = str(_form.help_text)
     else:
         detail["help_text"] = ""
 
     if detail.get("type") == "select":
```

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/classifier/serializers.py` & `weni_rp_apps-2.4.2a4/weni/internal/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/classifier/tests.py` & `weni_rp_apps-2.4.2a4/weni/internal/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/classifier/views.py` & `weni_rp_apps-2.4.2a4/weni/internal/classifier/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/clients/authenticators.py` & `weni_rp_apps-2.4.2a4/weni/internal/clients/authenticators.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/clients/connect.py` & `weni_rp_apps-2.4.2a4/weni/internal/clients/connect.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/externals/serializers.py` & `weni_rp_apps-2.4.2a4/weni/internal/externals/serializers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from rest_framework import serializers
 
 
-from weni.serializers import OrgUUIDRelatedField, UserEmailRelatedField
+from weni.serializers import UserEmailRelatedField
 from temba.externals.models import ExternalService
+from weni.serializers.fields import ProjectUUIDRelatedField
 
 
 class ExternalServicesSerializer(serializers.Serializer):
     uuid = serializers.UUIDField(read_only=True)
     type_code = serializers.CharField(write_only=True)
     type_fields = serializers.JSONField(write_only=True)
-    org = OrgUUIDRelatedField(write_only=True)
+    project = ProjectUUIDRelatedField(write_only=True)
     user = UserEmailRelatedField(write_only=True)
 
     external_service_type = serializers.CharField(read_only=True)
     name = serializers.CharField(read_only=True)
     config = serializers.JSONField(read_only=True)
 
     def create(self, validated_data: dict):
         validated_data = validated_data
 
         type_code = validated_data.get("type_code")
         type_fields = validated_data.get("type_fields")
         user = validated_data.get("user")
-        org = validated_data.get("org")
+        project = validated_data.get("project")
 
         try:
             type_ = ExternalService.get_type_from_code(type_code)
         except KeyError as error:
             raise serializers.ValidationError(error)
 
         type_serializer = type_.serializer_class(data=type_fields)
         type_serializer.is_valid(raise_exception=True)
-        return type_serializer.save(type=type_, created_by=user, modified_by=user, org=org)
+        return type_serializer.save(
+            type=type_, created_by=user, modified_by=user, org=project
+        )
```

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/externals/views.py` & `weni_rp_apps-2.4.2a4/weni/internal/globals/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-from typing import TYPE_CHECKING
-
-from django.contrib.auth.models import User
-from django.shortcuts import get_object_or_404
-from rest_framework.views import APIView
-from rest_framework.response import Response
-from rest_framework.renderers import JSONRenderer
-from rest_framework.permissions import IsAuthenticated
+from rest_framework import mixins
 from rest_framework import status
+from rest_framework.response import Response
+from rest_framework.exceptions import ValidationError
 
-from weni.internal.authenticators import InternalOIDCAuthentication
-from weni.internal.permissions import CanCommunicateInternally
-from weni.internal.externals.serializers import ExternalServicesSerializer
-from temba.externals.models import ExternalService
-
-
-if TYPE_CHECKING:
-    from rest_framework.request import Request
-
+from temba.globals.models import Global
+from temba.orgs.models import Org
+from weni.internal.views import InternalGenericViewSet
+from weni.internal.globals.serializers import GlobalSerializer
+
+
+class GlobalViewSet(
+    mixins.CreateModelMixin,
+    mixins.RetrieveModelMixin,
+    mixins.DestroyModelMixin,
+    mixins.ListModelMixin,
+    InternalGenericViewSet,
+):
+    serializer_class = GlobalSerializer
+    lookup_field = "uuid"
+
+    def get_queryset(self):
+        queryset = Global.objects.filter(is_active=True)
+        org = self.request.query_params.get("org")
+
+        try:
+            org_object = Org.objects.get(uuid=org)
+            queryset = queryset.filter(org=org_object)
+            return queryset
 
-class ExternalServicesAPIView(APIView):
-    authentication_classes = [InternalOIDCAuthentication]
-    permission_classes = [IsAuthenticated, CanCommunicateInternally]
-    pagination_class = None
-    renderer_classes = [JSONRenderer]
-    throttle_classes = []
+        except Org.DoesNotExist as error:
+            raise ValidationError(detail={"message": str(error)})
 
-    def post(self, request: "Request") -> Response:
-        serializer = ExternalServicesSerializer(data=request.data)
+    def create(self, request, *args, **kwargs):
+        serializer = self.get_serializer(data=request.data, many=True)
         serializer.is_valid(raise_exception=True)
-        serializer.save()
 
-        return Response(serializer.data, status=status.HTTP_201_CREATED)
+        self.perform_create(serializer.validated_data)
 
-    def delete(self, request, uuid=None):
-        external_service = get_object_or_404(ExternalService, uuid=uuid)
-        user = get_object_or_404(User, email=request.query_params.get("user"))
+        headers = self.get_success_headers(serializer.data)
 
-        external_service.release(user)
+        return Response(serializer.data, status=status.HTTP_201_CREATED, headers=headers)
 
-        return Response(status=status.HTTP_204_NO_CONTENT)
+    def perform_create(self, validated_data_list):
+        self.get_serializer().create_many(validated_data_list)
```

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/flows/serializers.py` & `weni_rp_apps-2.4.2a4/weni/internal/flows/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/flows/tests.py` & `weni_rp_apps-2.4.2a4/weni/internal/flows/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/flows/views.py` & `weni_rp_apps-2.4.2a4/weni/internal/flows/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/globals/serializers.py` & `weni_rp_apps-2.4.2a4/weni/internal/globals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/globals/tests/test_serializers.py` & `weni_rp_apps-2.4.2a4/weni/internal/globals/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/migrations/0001_initial.py` & `weni_rp_apps-2.4.2a4/weni/internal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/migrations/0002_project.py` & `weni_rp_apps-2.4.2a4/weni/internal/migrations/0002_project.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/models.py` & `weni_rp_apps-2.4.2a4/weni/internal/models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/orgs/serializers.py` & `weni_rp_apps-2.4.2a4/weni/internal/orgs/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/orgs/tests.py` & `weni_rp_apps-2.4.2a4/weni/internal/orgs/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/orgs/views.py` & `weni_rp_apps-2.4.2a4/weni/internal/orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/statistic/tests.py` & `weni_rp_apps-2.4.2a4/weni/internal/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/statistic/views.py` & `weni_rp_apps-2.4.2a4/weni/internal/statistic/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/tests/test_models.py` & `weni_rp_apps-2.4.2a4/weni/internal/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/tickets/serializers.py` & `weni_rp_apps-2.4.2a4/weni/internal/tickets/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/tickets/tests/test_views.py` & `weni_rp_apps-2.4.2a4/weni/internal/tickets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/tickets/views.py` & `weni_rp_apps-2.4.2a4/weni/internal/tickets/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,8 +58,8 @@
         partial = kwargs.get("partial", False)
         if not partial:
             self.http_method_not_allowed(request, *args, **kwargs)
 
         return super().update(request, *args, **kwargs)
 
     def perform_destroy(self, instance):
-        instance.release()
+        instance.release(self.request.user)
```

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/urls.py` & `weni_rp_apps-2.4.2a4/weni/internal/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/users/serializers.py` & `weni_rp_apps-2.4.2a4/weni/internal/users/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/users/tests.py` & `weni_rp_apps-2.4.2a4/weni/internal/users/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/users/urls.py` & `weni_rp_apps-2.4.2a4/weni/internal/users/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/users/views.py` & `weni_rp_apps-2.4.2a4/weni/internal/users/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/internal/views.py` & `weni_rp_apps-2.4.2a4/weni/internal/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/orgs_api/serializers.py` & `weni_rp_apps-2.4.2a4/weni/orgs_api/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/orgs_api/tests.py` & `weni_rp_apps-2.4.2a4/weni/orgs_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/orgs_api/views.py` & `weni_rp_apps-2.4.2a4/weni/orgs_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/s3/views.py` & `weni_rp_apps-2.4.2a4/weni/s3/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/serializers/fields.py` & `weni_rp_apps-2.4.2a4/weni/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/success_orgs/business.py` & `weni_rp_apps-2.4.2a4/weni/success_orgs/business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/success_orgs/serializers.py` & `weni_rp_apps-2.4.2a4/weni/success_orgs/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/success_orgs/tests/test_business.py` & `weni_rp_apps-2.4.2a4/weni/success_orgs/tests/test_business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/success_orgs/views.py` & `weni_rp_apps-2.4.2a4/weni/success_orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/template_message/serializers.py` & `weni_rp_apps-2.4.2a4/weni/template_message/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/template_message/tests.py` & `weni_rp_apps-2.4.2a4/weni/template_message/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/template_message/views.py` & `weni_rp_apps-2.4.2a4/weni/template_message/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/templates/context_processors.py` & `weni_rp_apps-2.4.2a4/weni/templates/context_processors.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/ticketer_queues/tests.py` & `weni_rp_apps-2.4.2a4/weni/ticketer_queues/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/ticketer_queues/views.py` & `weni_rp_apps-2.4.2a4/weni/ticketer_queues/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/weni/utils/app_config.py` & `weni_rp_apps-2.4.2a4/weni/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.4.2a3/PKG-INFO` & `weni_rp_apps-2.4.2a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weni-rp-apps
-Version: 2.4.2a3
+Version: 2.4.2a4
 Summary: Weni apps for Rapidpro Platform
 License: AGPL-3.0
 Author: jcbalmeida
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```


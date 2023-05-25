# Comparing `tmp/betfairlightweight-2.9.1.tar.gz` & `tmp/betfairlightweight-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/betfairlightweight-2.9.1.tar", last modified: Mon Oct 26 09:34:07 2020, max compression
+gzip compressed data, was "dist/betfairlightweight-2.9.2.tar", last modified: Mon Oct 26 13:04:40 2020, max compression
```

## Comparing `betfairlightweight-2.9.1.tar` & `betfairlightweight-2.9.2.tar`

### file list

```diff
@@ -1,162 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1069 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       90 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      642 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5562 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/betfairlightweight/
--rw-r--r--   0 runner    (1001) docker     (116)      337 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      220 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/__version__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2191 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (116)     6873 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/baseclient.py
--rw-r--r--   0 runner    (1001) docker     (116)      711 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/
--rw-r--r--   0 runner    (1001) docker     (116)      388 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4805 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/account.py
--rw-r--r--   0 runner    (1001) docker     (116)     3985 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/baseendpoint.py
--rw-r--r--   0 runner    (1001) docker     (116)    26582 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/betting.py
--rw-r--r--   0 runner    (1001) docker     (116)     8105 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/historic.py
--rw-r--r--   0 runner    (1001) docker     (116)     4326 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/inplayservice.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/keepalive.py
--rw-r--r--   0 runner    (1001) docker     (116)     2414 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/login.py
--rw-r--r--   0 runner    (1001) docker     (116)     2355 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/logininteractive.py
--rw-r--r--   0 runner    (1001) docker     (116)     2101 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/logout.py
--rw-r--r--   0 runner    (1001) docker     (116)     1510 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/navigation.py
--rw-r--r--   0 runner    (1001) docker     (116)     5140 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/racecard.py
--rw-r--r--   0 runner    (1001) docker     (116)     4681 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/scores.py
--rw-r--r--   0 runner    (1001) docker     (116)     2714 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/endpoints/streaming.py
--rw-r--r--   0 runner    (1001) docker     (116)    14410 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/enums.py
--rw-r--r--   0 runner    (1001) docker     (116)     4197 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    13217 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/filters.py
--rw-r--r--   0 runner    (1001) docker     (116)     2509 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/betfairlightweight/resources/
--rw-r--r--   0 runner    (1001) docker     (116)      848 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3738 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/resources/accountresources.py
--rw-r--r--   0 runner    (1001) docker     (116)      879 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/resources/authresources.py
--rw-r--r--   0 runner    (1001) docker     (116)     1242 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/resources/baseresource.py
--rw-r--r--   0 runner    (1001) docker     (116)    33133 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/resources/bettingresources.py
--rw-r--r--   0 runner    (1001) docker     (116)     6365 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/resources/inplayserviceresources.py
--rw-r--r--   0 runner    (1001) docker     (116)    10404 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/resources/racecardresources.py
--rw-r--r--   0 runner    (1001) docker     (116)     2063 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/resources/scoresresources.py
--rw-r--r--   0 runner    (1001) docker     (116)     5379 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/resources/streamingresources.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/betfairlightweight/streaming/
--rw-r--r--   0 runner    (1001) docker     (116)      183 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11350 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/streaming/betfairstream.py
--rw-r--r--   0 runner    (1001) docker     (116)    17726 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/streaming/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)     6549 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/streaming/listener.py
--rw-r--r--   0 runner    (1001) docker     (116)     6821 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/streaming/stream.py
--rw-r--r--   0 runner    (1001) docker     (116)     1539 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/betfairlightweight/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/betfairlightweight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      642 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/betfairlightweight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5456 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/betfairlightweight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/betfairlightweight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       55 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/betfairlightweight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/betfairlightweight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1412 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      914 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/integration/test_historicalstream.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (116)     1796 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/availableevents.json
--rw-r--r--   0 runner    (1001) docker     (116)       22 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/base_endpoint_fail.json
--rw-r--r--   0 runner    (1001) docker     (116)       24 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/base_endpoint_success.json
--rw-r--r--   0 runner    (1001) docker     (116)       12 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/base_resource.json
--rw-r--r--   0 runner    (1001) docker     (116)      110 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/base_resource_dict.json
--rw-r--r--   0 runner    (1001) docker     (116)      143 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/base_resource_sub.json
--rw-r--r--   0 runner    (1001) docker     (116)      281 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/cancel_orders.json
--rw-r--r--   0 runner    (1001) docker     (116)     2318 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/eventtimeline.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/tests/resources/historicaldata/
--rwxr-xr-x   0 runner    (1001) docker     (116)   101027 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/historicaldata/BASIC-1.132153978
--rw-r--r--   0 runner    (1001) docker     (116)    48798 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/incidents.json
--rw-r--r--   0 runner    (1001) docker     (116)       81 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/keep_alive_fail.json
--rw-r--r--   0 runner    (1001) docker     (116)       75 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/keep_alive_success.json
--rw-r--r--   0 runner    (1001) docker     (116)      514 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_cleared_orders.json
--rw-r--r--   0 runner    (1001) docker     (116)     2270 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_competitions.json
--rw-r--r--   0 runner    (1001) docker     (116)      188 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_countries.json
--rw-r--r--   0 runner    (1001) docker     (116)      589 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_current_orders.json
--rw-r--r--   0 runner    (1001) docker     (116)      161 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_event_types.json
--rw-r--r--   0 runner    (1001) docker     (116)     1220 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_events.json
--rw-r--r--   0 runner    (1001) docker     (116)    32759 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_market_book.json
--rw-r--r--   0 runner    (1001) docker     (116)     2531 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_market_catalogue.json
--rw-r--r--   0 runner    (1001) docker     (116)     4102 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_market_catalogue_no_ero.json
--rw-r--r--   0 runner    (1001) docker     (116)      626 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_market_profit_and_loss.json
--rw-r--r--   0 runner    (1001) docker     (116)     1213 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_market_types.json
--rw-r--r--   0 runner    (1001) docker     (116)    64621 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_race_details.json
--rw-r--r--   0 runner    (1001) docker     (116)      506 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_runner_book.json
--rw-r--r--   0 runner    (1001) docker     (116)     2980 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_time_ranges.json
--rw-r--r--   0 runner    (1001) docker     (116)     1218 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/list_venues.json
--rw-r--r--   0 runner    (1001) docker     (116)       46 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/login_fail.json
--rw-r--r--   0 runner    (1001) docker     (116)       41 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/login_interactive_fail.json
--rw-r--r--   0 runner    (1001) docker     (116)       44 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/login_interactive_success.json
--rw-r--r--   0 runner    (1001) docker     (116)       56 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/login_success.json
--rw-r--r--   0 runner    (1001) docker     (116)       82 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/logout_fail.json
--rw-r--r--   0 runner    (1001) docker     (116)       75 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/logout_success.json
--rw-r--r--   0 runner    (1001) docker     (116)      380 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/place_orders.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/tests/resources/racecards/
--rw-r--r--   0 runner    (1001) docker     (116)    10466 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards.json
--rw-r--r--   0 runner    (1001) docker     (116)    19867 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards0.json
--rw-r--r--   0 runner    (1001) docker     (116)    18171 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards1.json
--rw-r--r--   0 runner    (1001) docker     (116)    17722 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards10.json
--rw-r--r--   0 runner    (1001) docker     (116)    14387 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards2.json
--rw-r--r--   0 runner    (1001) docker     (116)    16375 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards3.json
--rw-r--r--   0 runner    (1001) docker     (116)    14542 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards4.json
--rw-r--r--   0 runner    (1001) docker     (116)    14747 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards5.json
--rw-r--r--   0 runner    (1001) docker     (116)    14798 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards6.json
--rw-r--r--   0 runner    (1001) docker     (116)    14519 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards7.json
--rw-r--r--   0 runner    (1001) docker     (116)    19429 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards8.json
--rw-r--r--   0 runner    (1001) docker     (116)    20055 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racecards/racecards9.json
--rw-r--r--   0 runner    (1001) docker     (116)      151 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/racedetails.json
--rw-r--r--   0 runner    (1001) docker     (116)      560 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/replace_orders.json
--rw-r--r--   0 runner    (1001) docker     (116)      523 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/score.json
--rw-r--r--   0 runner    (1001) docker     (116)     1226 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/scores.json
--rw-r--r--   0 runner    (1001) docker     (116)       32 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_503.json
--rw-r--r--   0 runner    (1001) docker     (116)       60 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_connection.json
--rw-r--r--   0 runner    (1001) docker     (116)     1219 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_market_definition.json
--rw-r--r--   0 runner    (1001) docker     (116)       76 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_mcm_HEARTBEAT.json
--rw-r--r--   0 runner    (1001) docker     (116)    20452 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_mcm_RESUB_DELTA.json
--rw-r--r--   0 runner    (1001) docker     (116)     1816 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_mcm_SUB_IMAGE.json
--rw-r--r--   0 runner    (1001) docker     (116)   186255 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_mcm_SUB_IMAGE_no_market_def.json
--rw-r--r--   0 runner    (1001) docker     (116)      807 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_mcm_UPDATE_md.json
--rw-r--r--   0 runner    (1001) docker     (116)       99 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_mcm_UPDATE_tv.json
--rw-r--r--   0 runner    (1001) docker     (116)      133 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_mcm_update.json
--rw-r--r--   0 runner    (1001) docker     (116)     1381 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_ocm_FULL_IMAGE.json
--rw-r--r--   0 runner    (1001) docker     (116)      278 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_ocm_SUB_IMAGE.json
--rw-r--r--   0 runner    (1001) docker     (116)      305 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_ocm_UPDATE.json
--rw-r--r--   0 runner    (1001) docker     (116)       70 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/streaming_status.json
--rw-r--r--   0 runner    (1001) docker     (116)      192 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/resources/update_orders.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 09:34:07.000000 betfairlightweight-2.9.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3330 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_account.py
--rw-r--r--   0 runner    (1001) docker     (116)     1302 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_accountresources.py
--rw-r--r--   0 runner    (1001) docker     (116)      307 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_apiclient.py
--rw-r--r--   0 runner    (1001) docker     (116)     8888 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_baseclient.py
--rw-r--r--   0 runner    (1001) docker     (116)     6711 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_baseendpoint.py
--rw-r--r--   0 runner    (1001) docker     (116)     2181 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_baseresource.py
--rw-r--r--   0 runner    (1001) docker     (116)    15598 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_betfairstream.py
--rw-r--r--   0 runner    (1001) docker     (116)    10863 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_betting.py
--rw-r--r--   0 runner    (1001) docker     (116)    24115 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_bettingresources.py
--rw-r--r--   0 runner    (1001) docker     (116)    21317 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (116)      819 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (116)     4306 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (116)     5273 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_historical.py
--rw-r--r--   0 runner    (1001) docker     (116)     5605 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_inplayservice.py
--rw-r--r--   0 runner    (1001) docker     (116)      694 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_inplayserviceresources.py
--rw-r--r--   0 runner    (1001) docker     (116)     3129 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_keepalive.py
--rw-r--r--   0 runner    (1001) docker     (116)     9739 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (116)     3449 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_login.py
--rw-r--r--   0 runner    (1001) docker     (116)     3360 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_logininteractive.py
--rw-r--r--   0 runner    (1001) docker     (116)     3135 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_logout.py
--rw-r--r--   0 runner    (1001) docker     (116)     2468 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)     3037 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_navigation.py
--rw-r--r--   0 runner    (1001) docker     (116)     6991 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_racecard.py
--rw-r--r--   0 runner    (1001) docker     (116)      928 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_racecardresources.py
--rw-r--r--   0 runner    (1001) docker     (116)     3274 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_scores.py
--rw-r--r--   0 runner    (1001) docker     (116)     1122 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_scoresresources.py
--rw-r--r--   0 runner    (1001) docker     (116)    11427 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (116)     1811 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_streamingendpoint.py
--rw-r--r--   0 runner    (1001) docker     (116)     1924 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_streamingresources.py
--rw-r--r--   0 runner    (1001) docker     (116)     1074 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      344 2020-10-26 09:33:42.000000 betfairlightweight-2.9.1/tests/unit/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (116)     1069 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      141 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      642 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5521 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/betfairlightweight/
+-rw-r--r--   0 runner    (1001) docker     (116)      337 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      220 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2191 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6873 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (116)      711 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (116)      388 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4805 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/account.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3985 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/baseendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26582 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/betting.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8105 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/historic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4326 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/inplayservice.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2162 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/keepalive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2414 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/login.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2355 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/logininteractive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2101 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/logout.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1510 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5140 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/racecard.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4681 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/scores.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2714 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/endpoints/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14410 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/enums.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4197 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13217 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/filters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2509 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/betfairlightweight/resources/
+-rw-r--r--   0 runner    (1001) docker     (116)      848 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3738 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/resources/accountresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)      879 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/resources/authresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1242 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/resources/baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (116)    33133 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/resources/bettingresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6365 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/resources/inplayserviceresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10404 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/resources/racecardresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2063 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/resources/scoresresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5379 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/resources/streamingresources.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/betfairlightweight/streaming/
+-rw-r--r--   0 runner    (1001) docker     (116)      183 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11350 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/streaming/betfairstream.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17726 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/streaming/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6549 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/streaming/listener.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6821 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/streaming/stream.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1539 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/betfairlightweight/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/betfairlightweight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      642 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/betfairlightweight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5479 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/betfairlightweight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/betfairlightweight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       55 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/betfairlightweight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/betfairlightweight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       30 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/requirements-speed.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1412 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      914 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/integration/test_historicalstream.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (116)     1796 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/availableevents.json
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/base_endpoint_fail.json
+-rw-r--r--   0 runner    (1001) docker     (116)       24 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/base_endpoint_success.json
+-rw-r--r--   0 runner    (1001) docker     (116)       12 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/base_resource.json
+-rw-r--r--   0 runner    (1001) docker     (116)      110 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/base_resource_dict.json
+-rw-r--r--   0 runner    (1001) docker     (116)      143 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/base_resource_sub.json
+-rw-r--r--   0 runner    (1001) docker     (116)      281 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/cancel_orders.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2318 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/eventtimeline.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/tests/resources/historicaldata/
+-rwxr-xr-x   0 runner    (1001) docker     (116)   101027 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/historicaldata/BASIC-1.132153978
+-rw-r--r--   0 runner    (1001) docker     (116)    48798 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/incidents.json
+-rw-r--r--   0 runner    (1001) docker     (116)       81 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/keep_alive_fail.json
+-rw-r--r--   0 runner    (1001) docker     (116)       75 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/keep_alive_success.json
+-rw-r--r--   0 runner    (1001) docker     (116)      514 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_cleared_orders.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2270 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_competitions.json
+-rw-r--r--   0 runner    (1001) docker     (116)      188 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_countries.json
+-rw-r--r--   0 runner    (1001) docker     (116)      589 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_current_orders.json
+-rw-r--r--   0 runner    (1001) docker     (116)      161 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_event_types.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1220 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_events.json
+-rw-r--r--   0 runner    (1001) docker     (116)    32759 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_market_book.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2531 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_market_catalogue.json
+-rw-r--r--   0 runner    (1001) docker     (116)     4102 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_market_catalogue_no_ero.json
+-rw-r--r--   0 runner    (1001) docker     (116)      626 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_market_profit_and_loss.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1213 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_market_types.json
+-rw-r--r--   0 runner    (1001) docker     (116)    64621 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_race_details.json
+-rw-r--r--   0 runner    (1001) docker     (116)      506 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_runner_book.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2980 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_time_ranges.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1218 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/list_venues.json
+-rw-r--r--   0 runner    (1001) docker     (116)       46 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/login_fail.json
+-rw-r--r--   0 runner    (1001) docker     (116)       41 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/login_interactive_fail.json
+-rw-r--r--   0 runner    (1001) docker     (116)       44 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/login_interactive_success.json
+-rw-r--r--   0 runner    (1001) docker     (116)       56 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/login_success.json
+-rw-r--r--   0 runner    (1001) docker     (116)       82 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/logout_fail.json
+-rw-r--r--   0 runner    (1001) docker     (116)       75 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/logout_success.json
+-rw-r--r--   0 runner    (1001) docker     (116)      380 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/place_orders.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/tests/resources/racecards/
+-rw-r--r--   0 runner    (1001) docker     (116)    10466 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards.json
+-rw-r--r--   0 runner    (1001) docker     (116)    19867 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards0.json
+-rw-r--r--   0 runner    (1001) docker     (116)    18171 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards1.json
+-rw-r--r--   0 runner    (1001) docker     (116)    17722 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards10.json
+-rw-r--r--   0 runner    (1001) docker     (116)    14387 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards2.json
+-rw-r--r--   0 runner    (1001) docker     (116)    16375 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards3.json
+-rw-r--r--   0 runner    (1001) docker     (116)    14542 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards4.json
+-rw-r--r--   0 runner    (1001) docker     (116)    14747 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards5.json
+-rw-r--r--   0 runner    (1001) docker     (116)    14798 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards6.json
+-rw-r--r--   0 runner    (1001) docker     (116)    14519 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards7.json
+-rw-r--r--   0 runner    (1001) docker     (116)    19429 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards8.json
+-rw-r--r--   0 runner    (1001) docker     (116)    20055 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racecards/racecards9.json
+-rw-r--r--   0 runner    (1001) docker     (116)      151 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/racedetails.json
+-rw-r--r--   0 runner    (1001) docker     (116)      560 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/replace_orders.json
+-rw-r--r--   0 runner    (1001) docker     (116)      523 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/score.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1226 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/scores.json
+-rw-r--r--   0 runner    (1001) docker     (116)       32 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_503.json
+-rw-r--r--   0 runner    (1001) docker     (116)       60 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_connection.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1219 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_market_definition.json
+-rw-r--r--   0 runner    (1001) docker     (116)       76 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_mcm_HEARTBEAT.json
+-rw-r--r--   0 runner    (1001) docker     (116)    20452 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_mcm_RESUB_DELTA.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1816 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_mcm_SUB_IMAGE.json
+-rw-r--r--   0 runner    (1001) docker     (116)   186255 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_mcm_SUB_IMAGE_no_market_def.json
+-rw-r--r--   0 runner    (1001) docker     (116)      807 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_mcm_UPDATE_md.json
+-rw-r--r--   0 runner    (1001) docker     (116)       99 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_mcm_UPDATE_tv.json
+-rw-r--r--   0 runner    (1001) docker     (116)      133 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_mcm_update.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1381 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_ocm_FULL_IMAGE.json
+-rw-r--r--   0 runner    (1001) docker     (116)      278 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_ocm_SUB_IMAGE.json
+-rw-r--r--   0 runner    (1001) docker     (116)      305 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_ocm_UPDATE.json
+-rw-r--r--   0 runner    (1001) docker     (116)       70 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/streaming_status.json
+-rw-r--r--   0 runner    (1001) docker     (116)      192 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/resources/update_orders.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:40.000000 betfairlightweight-2.9.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3330 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1302 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_accountresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)      307 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8888 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6711 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_baseendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2181 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15598 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_betfairstream.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10863 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_betting.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24115 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_bettingresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21317 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)      819 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4306 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5273 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_historical.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5605 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_inplayservice.py
+-rw-r--r--   0 runner    (1001) docker     (116)      694 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_inplayserviceresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3129 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_keepalive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9739 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3449 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3360 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_logininteractive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3135 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_logout.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2468 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3037 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_navigation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6991 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_racecard.py
+-rw-r--r--   0 runner    (1001) docker     (116)      928 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_racecardresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3274 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_scores.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1122 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_scoresresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11427 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1811 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_streamingendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1924 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_streamingresources.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1074 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      344 2020-10-26 13:04:17.000000 betfairlightweight-2.9.2/tests/unit/tools.py
```

### Comparing `betfairlightweight-2.9.1/LICENSE` & `betfairlightweight-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/PKG-INFO` & `betfairlightweight-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfairlightweight
-Version: 2.9.1
+Version: 2.9.2
 Summary: Lightweight python wrapper for Betfair API-NG
 Home-page: https://github.com/liampauling/betfair
 Author: Liam Pauling
 Author-email: a@unknown.invalid
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `betfairlightweight-2.9.1/README.md` & `betfairlightweight-2.9.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # betfairlightweight
 
-[![Build Status](https://travis-ci.org/liampauling/betfair.svg?branch=master)](https://travis-ci.org/liampauling/betfair) [![Coverage Status](https://coveralls.io/repos/github/liampauling/betfair/badge.svg?branch=master)](https://coveralls.io/github/liampauling/betfair?branch=master) [![PyPI version](https://badge.fury.io/py/betfairlightweight.svg)](https://pypi.python.org/pypi/betfairlightweight) [![Downloads](https://pepy.tech/badge/betfairlightweight)](https://pepy.tech/project/betfairlightweight)
+![Build Status](https://github.com/liampauling/betfair/workflows/test/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/liampauling/betfair/badge.svg?branch=master)](https://coveralls.io/github/liampauling/betfair?branch=master) [![PyPI version](https://badge.fury.io/py/betfairlightweight.svg)](https://pypi.python.org/pypi/betfairlightweight) [![Downloads](https://pepy.tech/badge/betfairlightweight)](https://pepy.tech/project/betfairlightweight)
 
 Lightweight, super fast (uses C and Rust libraries) pythonic wrapper for [Betfair API-NG](https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni) allowing all betting operations (including market and order streaming) and account operations, see [examples](https://github.com/liampauling/betfair/tree/master/examples).
 
 [docs](https://liampauling.github.io/betfair/)
 
 [join slack group](https://betfairlightweight.herokuapp.com)
```

### Comparing `betfairlightweight-2.9.1/betfairlightweight/apiclient.py` & `betfairlightweight-2.9.2/betfairlightweight/apiclient.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/baseclient.py` & `betfairlightweight-2.9.2/betfairlightweight/baseclient.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/compat.py` & `betfairlightweight-2.9.2/betfairlightweight/compat.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/account.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/account.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/baseendpoint.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/baseendpoint.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/betting.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/betting.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/historic.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/historic.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/inplayservice.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/inplayservice.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/keepalive.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/keepalive.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/login.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/login.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/logininteractive.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/logininteractive.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/logout.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/logout.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/navigation.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/navigation.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/racecard.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/racecard.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/scores.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/scores.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/endpoints/streaming.py` & `betfairlightweight-2.9.2/betfairlightweight/endpoints/streaming.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/enums.py` & `betfairlightweight-2.9.2/betfairlightweight/enums.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/exceptions.py` & `betfairlightweight-2.9.2/betfairlightweight/exceptions.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/filters.py` & `betfairlightweight-2.9.2/betfairlightweight/filters.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/metadata.py` & `betfairlightweight-2.9.2/betfairlightweight/metadata.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/resources/__init__.py` & `betfairlightweight-2.9.2/betfairlightweight/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/resources/accountresources.py` & `betfairlightweight-2.9.2/betfairlightweight/resources/accountresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/resources/authresources.py` & `betfairlightweight-2.9.2/betfairlightweight/resources/authresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/resources/baseresource.py` & `betfairlightweight-2.9.2/betfairlightweight/resources/baseresource.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/resources/bettingresources.py` & `betfairlightweight-2.9.2/betfairlightweight/resources/bettingresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/resources/inplayserviceresources.py` & `betfairlightweight-2.9.2/betfairlightweight/resources/inplayserviceresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/resources/racecardresources.py` & `betfairlightweight-2.9.2/betfairlightweight/resources/racecardresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/resources/scoresresources.py` & `betfairlightweight-2.9.2/betfairlightweight/resources/scoresresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/resources/streamingresources.py` & `betfairlightweight-2.9.2/betfairlightweight/resources/streamingresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/streaming/betfairstream.py` & `betfairlightweight-2.9.2/betfairlightweight/streaming/betfairstream.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/streaming/cache.py` & `betfairlightweight-2.9.2/betfairlightweight/streaming/cache.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/streaming/listener.py` & `betfairlightweight-2.9.2/betfairlightweight/streaming/listener.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/streaming/stream.py` & `betfairlightweight-2.9.2/betfairlightweight/streaming/stream.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight/utils.py` & `betfairlightweight-2.9.2/betfairlightweight/utils.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/betfairlightweight.egg-info/PKG-INFO` & `betfairlightweight-2.9.2/betfairlightweight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfairlightweight
-Version: 2.9.1
+Version: 2.9.2
 Summary: Lightweight python wrapper for Betfair API-NG
 Home-page: https://github.com/liampauling/betfair
 Author: Liam Pauling
 Author-email: a@unknown.invalid
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `betfairlightweight-2.9.1/betfairlightweight.egg-info/SOURCES.txt` & `betfairlightweight-2.9.2/betfairlightweight.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements-speed.txt
 requirements.txt
 setup.py
 betfairlightweight/__init__.py
 betfairlightweight/__version__.py
 betfairlightweight/apiclient.py
 betfairlightweight/baseclient.py
 betfairlightweight/compat.py
```

### Comparing `betfairlightweight-2.9.1/setup.py` & `betfairlightweight-2.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/integration/test_historicalstream.py` & `betfairlightweight-2.9.2/tests/integration/test_historicalstream.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/availableevents.json` & `betfairlightweight-2.9.2/tests/resources/availableevents.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/eventtimeline.json` & `betfairlightweight-2.9.2/tests/resources/eventtimeline.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/historicaldata/BASIC-1.132153978` & `betfairlightweight-2.9.2/tests/resources/historicaldata/BASIC-1.132153978`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/incidents.json` & `betfairlightweight-2.9.2/tests/resources/incidents.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_cleared_orders.json` & `betfairlightweight-2.9.2/tests/resources/list_cleared_orders.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_competitions.json` & `betfairlightweight-2.9.2/tests/resources/list_competitions.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_current_orders.json` & `betfairlightweight-2.9.2/tests/resources/list_current_orders.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_events.json` & `betfairlightweight-2.9.2/tests/resources/list_events.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_market_book.json` & `betfairlightweight-2.9.2/tests/resources/list_market_book.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_market_catalogue.json` & `betfairlightweight-2.9.2/tests/resources/list_market_catalogue.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_market_catalogue_no_ero.json` & `betfairlightweight-2.9.2/tests/resources/list_market_catalogue_no_ero.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_market_profit_and_loss.json` & `betfairlightweight-2.9.2/tests/resources/list_market_profit_and_loss.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_market_types.json` & `betfairlightweight-2.9.2/tests/resources/list_market_types.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_race_details.json` & `betfairlightweight-2.9.2/tests/resources/list_race_details.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_time_ranges.json` & `betfairlightweight-2.9.2/tests/resources/list_time_ranges.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/list_venues.json` & `betfairlightweight-2.9.2/tests/resources/list_venues.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards0.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards0.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards1.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards1.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards10.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards10.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards2.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards2.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards3.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards3.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards4.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards4.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards5.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards5.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards6.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards6.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards7.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards7.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards8.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards8.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/racecards/racecards9.json` & `betfairlightweight-2.9.2/tests/resources/racecards/racecards9.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/replace_orders.json` & `betfairlightweight-2.9.2/tests/resources/replace_orders.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/score.json` & `betfairlightweight-2.9.2/tests/resources/score.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/scores.json` & `betfairlightweight-2.9.2/tests/resources/scores.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/streaming_market_definition.json` & `betfairlightweight-2.9.2/tests/resources/streaming_market_definition.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/streaming_mcm_RESUB_DELTA.json` & `betfairlightweight-2.9.2/tests/resources/streaming_mcm_RESUB_DELTA.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/streaming_mcm_SUB_IMAGE.json` & `betfairlightweight-2.9.2/tests/resources/streaming_mcm_SUB_IMAGE.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/streaming_mcm_SUB_IMAGE_no_market_def.json` & `betfairlightweight-2.9.2/tests/resources/streaming_mcm_SUB_IMAGE_no_market_def.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/streaming_mcm_UPDATE_md.json` & `betfairlightweight-2.9.2/tests/resources/streaming_mcm_UPDATE_md.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/resources/streaming_ocm_FULL_IMAGE.json` & `betfairlightweight-2.9.2/tests/resources/streaming_ocm_FULL_IMAGE.json`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_account.py` & `betfairlightweight-2.9.2/tests/unit/test_account.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_accountresources.py` & `betfairlightweight-2.9.2/tests/unit/test_accountresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_baseclient.py` & `betfairlightweight-2.9.2/tests/unit/test_baseclient.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_baseendpoint.py` & `betfairlightweight-2.9.2/tests/unit/test_baseendpoint.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_baseresource.py` & `betfairlightweight-2.9.2/tests/unit/test_baseresource.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_betfairstream.py` & `betfairlightweight-2.9.2/tests/unit/test_betfairstream.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_betting.py` & `betfairlightweight-2.9.2/tests/unit/test_betting.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_bettingresources.py` & `betfairlightweight-2.9.2/tests/unit/test_bettingresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_cache.py` & `betfairlightweight-2.9.2/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_compat.py` & `betfairlightweight-2.9.2/tests/unit/test_compat.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_filters.py` & `betfairlightweight-2.9.2/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_historical.py` & `betfairlightweight-2.9.2/tests/unit/test_historical.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_inplayservice.py` & `betfairlightweight-2.9.2/tests/unit/test_inplayservice.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_inplayserviceresources.py` & `betfairlightweight-2.9.2/tests/unit/test_inplayserviceresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_keepalive.py` & `betfairlightweight-2.9.2/tests/unit/test_keepalive.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_listener.py` & `betfairlightweight-2.9.2/tests/unit/test_listener.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_login.py` & `betfairlightweight-2.9.2/tests/unit/test_login.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_logininteractive.py` & `betfairlightweight-2.9.2/tests/unit/test_logininteractive.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_logout.py` & `betfairlightweight-2.9.2/tests/unit/test_logout.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_metadata.py` & `betfairlightweight-2.9.2/tests/unit/test_metadata.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_navigation.py` & `betfairlightweight-2.9.2/tests/unit/test_navigation.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_racecard.py` & `betfairlightweight-2.9.2/tests/unit/test_racecard.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_racecardresources.py` & `betfairlightweight-2.9.2/tests/unit/test_racecardresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_scores.py` & `betfairlightweight-2.9.2/tests/unit/test_scores.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_scoresresources.py` & `betfairlightweight-2.9.2/tests/unit/test_scoresresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_stream.py` & `betfairlightweight-2.9.2/tests/unit/test_stream.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_streamingendpoint.py` & `betfairlightweight-2.9.2/tests/unit/test_streamingendpoint.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_streamingresources.py` & `betfairlightweight-2.9.2/tests/unit/test_streamingresources.py`

 * *Files identical despite different names*

### Comparing `betfairlightweight-2.9.1/tests/unit/test_utils.py` & `betfairlightweight-2.9.2/tests/unit/test_utils.py`

 * *Files identical despite different names*


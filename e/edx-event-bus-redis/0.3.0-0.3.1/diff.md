# Comparing `tmp/edx_event_bus_redis-0.3.0.tar.gz` & `tmp/edx_event_bus_redis-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx_event_bus_redis-0.3.0.tar", last modified: Tue May 23 18:16:21 2023, max compression
+gzip compressed data, was "edx_event_bus_redis-0.3.1.tar", last modified: Thu May 25 17:00:39 2023, max compression
```

## Comparing `edx_event_bus_redis-0.3.0.tar` & `edx_event_bus_redis-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8537 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6583 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    20754 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/message.py
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/producer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/commands/produce_event.py
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.737677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis/templates/edx_event_bus_redis/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/templates/edx_event_bus_redis/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8537 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-23 18:16:21.000000 edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5113 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 18:16:21.741677 edx_event_bus_redis-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-05-23 18:16:16.000000 edx_event_bus_redis-0.3.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:00:39.428447 edx_event_bus_redis-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    13050 2023-05-25 17:00:39.428447 edx_event_bus_redis-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10939 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:00:39.428447 edx_event_bus_redis-0.3.1/edx_event_bus_redis/
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:00:39.428447 edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20968 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/message.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5873 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/producer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:00:39.428447 edx_event_bus_redis-0.3.1/edx_event_bus_redis/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:00:39.428447 edx_event_bus_redis-0.3.1/edx_event_bus_redis/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/management/commands/produce_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:00:39.424447 edx_event_bus_redis-0.3.1/edx_event_bus_redis/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:00:39.428447 edx_event_bus_redis-0.3.1/edx_event_bus_redis/templates/edx_event_bus_redis/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/templates/edx_event_bus_redis/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:00:39.428447 edx_event_bus_redis-0.3.1/edx_event_bus_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13050 2023-05-25 17:00:39.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-25 17:00:39.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 17:00:39.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 17:00:39.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-25 17:00:39.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-25 17:00:39.000000 edx_event_bus_redis-0.3.1/edx_event_bus_redis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:00:39.428447 edx_event_bus_redis-0.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-25 17:00:39.432447 edx_event_bus_redis-0.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5113 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:00:39.428447 edx_event_bus_redis-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-05-25 17:00:32.000000 edx_event_bus_redis-0.3.1/tests/test_models.py
```

### Comparing `edx_event_bus_redis-0.3.0/LICENSE.txt` & `edx_event_bus_redis-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/config.py` & `edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/consumer.py` & `edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,20 @@
 # .. toggle_description: If set to False, consumer will exit immediately. This can be used as an emergency kill-switch
 #   to disable a consumer—as long as the management command is killed and restarted when settings change.
 # .. toggle_use_cases: opt_out
 # .. toggle_creation_date: 2022-01-31
 REDIS_CONSUMERS_ENABLED = SettingToggle('EVENT_BUS_REDIS_CONSUMERS_ENABLED', default=True)
 
 # .. setting_name: EVENT_BUS_REDIS_CONSUMER_POLL_TIMEOUT
-# .. setting_default: 1
-# .. setting_description: How long the consumer should wait, in seconds, for the Redis broker
-#   to respond to a poll() call.
-CONSUMER_POLL_TIMEOUT = getattr(settings, 'EVENT_BUS_REDIS_CONSUMER_POLL_TIMEOUT', 1)
+# .. setting_default: 60
+# .. setting_description: How long the consumer should wait for new entries in a stream.
+# .. As we are running the consumer in a while True loop, changing this setting doesn't make much difference
+# .. expect for changing number of monitoring messages while waiting for new events.
+# .. https://redis.io/commands/xread/#blocking-for-data
+CONSUMER_POLL_TIMEOUT = getattr(settings, 'EVENT_BUS_REDIS_CONSUMER_POLL_TIMEOUT', 60)
 
 # .. setting_name: EVENT_BUS_REDIS_CONSUMER_POLL_FAILURE_SLEEP
 # .. setting_default: 1.0
 # .. setting_description: When the consumer fails to retrieve an event from the broker,
 #   it will sleep for this many seconds before trying again. This is to prevent fast error-loops
 #   if the broker is down or the consumer is misconfigured. It *may* also sleep for errors that
 #   involve receiving an unreadable event, but this could change in the future to be more
```

### Comparing `edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/message.py` & `edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/message.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/producer.py` & `edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/producer.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,35 @@
 Main function is ``create_producer()``, which should be referred to from ``EVENT_BUS_PRODUCER``.
 """
 
 import logging
 from typing import Optional
 
 import attr
+from django.conf import settings
 from edx_django_utils.monitoring import record_exception
 from openedx_events.data import EventsMetadata
 from openedx_events.event_bus import EventBusProducer
 from openedx_events.event_bus.avro.serializer import serialize_event_data_to_bytes
 from openedx_events.tooling import OpenEdxPublicSignal
 from walrus import Database
 
 from edx_event_bus_redis.internal.message import RedisMessage
 
 from .config import get_full_topic, load_common_settings
 from .utils import AUDIT_LOGGING_ENABLED
 
 logger = logging.getLogger(__name__)
 
+# .. setting_name: EVENT_BUS_REDIS_STREAM_MAX_LEN
+# .. setting_default: 10000
+# .. setting_description: Limits stream size to approximately this number, more info can be found in
+# .. docs/decisions/0003-limiting-stream-length.rst
+STREAM_MAX_LEN = int(getattr(settings, 'EVENT_BUS_REDIS_STREAM_MAX_LEN', 10_000))
+
 
 def record_producing_error(error, context):
     """
     Record an error in producing an event to both the monitoring system and the regular logs
 
     Arguments:
         error: The exception or error raised during producing
@@ -117,15 +124,16 @@
             full_topic = get_full_topic(topic)
             context.full_topic = full_topic
             event_bytes = serialize_event_data_to_bytes(event_data, signal)
             message = RedisMessage(topic=full_topic, event_data=event_bytes, event_metadata=event_metadata)
             stream_data = message.to_binary_dict()
 
             stream = self.client.Stream(full_topic)
-            msg_id = stream.add(stream_data)
+            # Read docs/decisions/0003-limiting-stream-length.rst for explanation about maxlen and approximate options.
+            msg_id = stream.add(stream_data, maxlen=STREAM_MAX_LEN, approximate=True)
             context.on_event_deliver(msg_id)
         except Exception as e:  # pylint: disable=broad-except
             record_producing_error(e, context)
 
 
 def create_producer() -> Optional[RedisEventProducer]:
     """
```

### Comparing `edx_event_bus_redis-0.3.0/edx_event_bus_redis/internal/utils.py` & `edx_event_bus_redis-0.3.1/edx_event_bus_redis/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.3.0/edx_event_bus_redis/management/commands/produce_event.py` & `edx_event_bus_redis-0.3.1/edx_event_bus_redis/management/commands/produce_event.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.3.0/edx_event_bus_redis/templates/edx_event_bus_redis/base.html` & `edx_event_bus_redis-0.3.1/edx_event_bus_redis/templates/edx_event_bus_redis/base.html`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.3.0/edx_event_bus_redis.egg-info/SOURCES.txt` & `edx_event_bus_redis-0.3.1/edx_event_bus_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.3.0/requirements/constraints.txt` & `edx_event_bus_redis-0.3.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.3.0/setup.py` & `edx_event_bus_redis-0.3.1/setup.py`

 * *Files identical despite different names*


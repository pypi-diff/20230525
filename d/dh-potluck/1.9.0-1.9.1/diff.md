# Comparing `tmp/dh-potluck-1.9.0.tar.gz` & `tmp/dh-potluck-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dh-potluck-1.9.0.tar", max compression
+gzip compressed data, was "dh-potluck-1.9.1.tar", max compression
```

## Comparing `dh-potluck-1.9.0.tar` & `dh-potluck-1.9.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1573 2022-12-07 15:36:56.064096 dh-potluck-1.9.0/dh_potluck/__init__.py
--rw-r--r--   0        0        0     5102 2022-12-07 15:36:56.064299 dh-potluck-1.9.0/dh_potluck/api_docs.py
--rw-r--r--   0        0        0     7147 2022-12-07 15:36:56.064622 dh-potluck-1.9.0/dh_potluck/auth.py
--rw-r--r--   0        0        0        0 2021-06-30 19:26:49.415438 dh-potluck-1.9.0/dh_potluck/celery/__init__.py
--rw-r--r--   0        0        0      643 2022-04-05 17:39:25.291767 dh-potluck-1.9.0/dh_potluck/celery/crontab_parser.py
--rw-r--r--   0        0        0      718 2022-09-01 18:41:10.130796 dh-potluck-1.9.0/dh_potluck/celery/signals.py
--rw-r--r--   0        0        0     2779 2022-12-07 15:36:56.064989 dh-potluck-1.9.0/dh_potluck/celery/synchronization.py
--rw-r--r--   0        0        0     2323 2022-09-01 18:41:10.131692 dh-potluck-1.9.0/dh_potluck/decorators.py
--rw-r--r--   0        0        0      126 2022-04-05 16:32:01.487913 dh-potluck-1.9.0/dh_potluck/email/__init__.py
--rw-r--r--   0        0        0     1802 2022-12-07 15:36:56.065321 dh-potluck-1.9.0/dh_potluck/email/email_service.py
--rw-r--r--   0        0        0     2838 2022-12-07 15:36:56.066002 dh-potluck-1.9.0/dh_potluck/email/mandrill_email_client.py
--rw-r--r--   0        0        0      184 2021-06-30 19:26:49.416012 dh-potluck-1.9.0/dh_potluck/environment.py
--rw-r--r--   0        0        0    10495 2022-12-07 15:36:56.066528 dh-potluck-1.9.0/dh_potluck/extension.py
--rw-r--r--   0        0        0     2567 2022-04-05 16:32:01.490304 dh-potluck-1.9.0/dh_potluck/fields.py
--rw-r--r--   0        0        0      686 2021-06-30 19:26:49.416483 dh-potluck-1.9.0/dh_potluck/health_checks.py
--rw-r--r--   0        0        0     3047 2022-12-07 15:36:56.066935 dh-potluck-1.9.0/dh_potluck/image_api.py
--rw-r--r--   0        0        0     4303 2022-12-07 15:36:56.067319 dh-potluck-1.9.0/dh_potluck/logging.py
--rw-r--r--   0        0        0      552 2022-12-09 17:33:09.122231 dh-potluck-1.9.0/dh_potluck/messaging/__init__.py
--rw-r--r--   0        0        0     6666 2022-12-09 18:21:56.734430 dh-potluck-1.9.0/dh_potluck/messaging/batching_consumer.py
--rw-r--r--   0        0        0     2587 2022-12-09 17:33:09.124271 dh-potluck-1.9.0/dh_potluck/messaging/consumer.py
--rw-r--r--   0        0        0      353 2022-12-09 17:33:09.125032 dh-potluck-1.9.0/dh_potluck/messaging/exceptions.py
--rw-r--r--   0        0        0     3229 2022-12-09 17:33:09.126176 dh-potluck-1.9.0/dh_potluck/messaging/incoming_message_router.py
--rw-r--r--   0        0        0      868 2022-12-07 15:36:56.068996 dh-potluck-1.9.0/dh_potluck/messaging/message.py
--rw-r--r--   0        0        0     1321 2022-12-09 17:33:09.127235 dh-potluck-1.9.0/dh_potluck/messaging/message_consumer_app.py
--rw-r--r--   0        0        0      271 2021-06-30 19:26:49.417759 dh-potluck-1.9.0/dh_potluck/messaging/message_envelope_schema.py
--rw-r--r--   0        0        0     6107 2022-12-07 15:36:56.069708 dh-potluck-1.9.0/dh_potluck/messaging/producer.py
--rw-r--r--   0        0        0      223 2022-12-09 17:33:09.127839 dh-potluck-1.9.0/dh_potluck/messaging/typings.py
--rw-r--r--   0        0        0      848 2022-12-09 17:33:09.128378 dh-potluck-1.9.0/dh_potluck/messaging/utils.py
--rw-r--r--   0        0        0     1056 2022-12-07 15:36:56.070036 dh-potluck-1.9.0/dh_potluck/mixpanel.py
--rw-r--r--   0        0        0     2279 2021-06-30 19:26:49.418076 dh-potluck-1.9.0/dh_potluck/platform_connection.py
--rw-r--r--   0        0        0     1703 2021-06-30 19:26:49.418210 dh-potluck-1.9.0/dh_potluck/queries_summary.py
--rw-r--r--   0        0        0     2575 2022-12-07 15:36:56.070393 dh-potluck-1.9.0/dh_potluck/s3_service.py
--rw-r--r--   0        0        0      557 2022-12-07 15:36:56.070681 dh-potluck-1.9.0/dh_potluck/templates/redoc.html
--rw-r--r--   0        0        0        0 2022-12-07 15:36:56.070841 dh-potluck-1.9.0/dh_potluck/types/__init__.py
--rw-r--r--   0        0        0      884 2022-12-07 15:36:56.071318 dh-potluck-1.9.0/dh_potluck/types/json_serializable.py
--rw-r--r--   0        0        0        0 2021-06-30 19:26:49.418529 dh-potluck-1.9.0/dh_potluck/utils/__init__.py
--rw-r--r--   0        0        0      478 2021-06-30 19:26:49.418652 dh-potluck-1.9.0/dh_potluck/utils/term.py
--rw-r--r--   0        0        0     2019 2022-12-09 18:29:49.038991 dh-potluck-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1174 2022-12-09 18:30:30.072053 dh-potluck-1.9.0/setup.py
--rw-r--r--   0        0        0      974 2022-12-09 18:30:30.072282 dh-potluck-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1573 2022-10-28 13:13:57.294362 dh-potluck-1.9.1/dh_potluck/__init__.py
+-rw-r--r--   0        0        0     5102 2022-12-16 14:39:36.592182 dh-potluck-1.9.1/dh_potluck/api_docs.py
+-rw-r--r--   0        0        0     7147 2022-10-28 13:13:57.295426 dh-potluck-1.9.1/dh_potluck/auth.py
+-rw-r--r--   0        0        0        0 2020-11-05 18:11:29.230651 dh-potluck-1.9.1/dh_potluck/celery/__init__.py
+-rw-r--r--   0        0        0      643 2022-08-02 13:50:42.560274 dh-potluck-1.9.1/dh_potluck/celery/crontab_parser.py
+-rw-r--r--   0        0        0      718 2022-08-02 13:50:42.560663 dh-potluck-1.9.1/dh_potluck/celery/signals.py
+-rw-r--r--   0        0        0     2779 2022-09-22 16:49:17.725906 dh-potluck-1.9.1/dh_potluck/celery/synchronization.py
+-rw-r--r--   0        0        0     2323 2022-08-02 13:50:42.561307 dh-potluck-1.9.1/dh_potluck/decorators.py
+-rw-r--r--   0        0        0      126 2022-08-02 13:50:42.561624 dh-potluck-1.9.1/dh_potluck/email/__init__.py
+-rw-r--r--   0        0        0     1802 2022-09-22 16:49:17.726424 dh-potluck-1.9.1/dh_potluck/email/email_service.py
+-rw-r--r--   0        0        0     2838 2022-09-22 16:49:17.726986 dh-potluck-1.9.1/dh_potluck/email/mandrill_email_client.py
+-rw-r--r--   0        0        0      184 2021-03-04 17:49:50.739841 dh-potluck-1.9.1/dh_potluck/environment.py
+-rw-r--r--   0        0        0    10495 2022-10-28 13:13:57.296126 dh-potluck-1.9.1/dh_potluck/extension.py
+-rw-r--r--   0        0        0     2567 2022-08-02 13:50:42.562885 dh-potluck-1.9.1/dh_potluck/fields.py
+-rw-r--r--   0        0        0      686 2021-03-04 17:49:50.740860 dh-potluck-1.9.1/dh_potluck/health_checks.py
+-rw-r--r--   0        0        0     3047 2022-09-22 16:49:17.727468 dh-potluck-1.9.1/dh_potluck/image_api.py
+-rw-r--r--   0        0        0     4303 2022-09-22 16:49:17.747736 dh-potluck-1.9.1/dh_potluck/logging.py
+-rw-r--r--   0        0        0      552 2022-12-16 14:39:36.593043 dh-potluck-1.9.1/dh_potluck/messaging/__init__.py
+-rw-r--r--   0        0        0     7109 2022-12-16 15:13:43.431889 dh-potluck-1.9.1/dh_potluck/messaging/batching_consumer.py
+-rw-r--r--   0        0        0       94 2022-12-16 14:53:41.310081 dh-potluck-1.9.1/dh_potluck/messaging/constants.py
+-rw-r--r--   0        0        0     3030 2022-12-16 15:13:43.405410 dh-potluck-1.9.1/dh_potluck/messaging/consumer.py
+-rw-r--r--   0        0        0      258 2022-12-16 15:04:19.108851 dh-potluck-1.9.1/dh_potluck/messaging/exceptions.py
+-rw-r--r--   0        0        0     3672 2022-12-16 15:13:43.478070 dh-potluck-1.9.1/dh_potluck/messaging/incoming_message_router.py
+-rw-r--r--   0        0        0      868 2022-09-22 16:49:17.729603 dh-potluck-1.9.1/dh_potluck/messaging/message.py
+-rw-r--r--   0        0        0     1795 2022-12-16 15:13:43.471940 dh-potluck-1.9.1/dh_potluck/messaging/message_consumer_app.py
+-rw-r--r--   0        0        0      271 2021-03-11 18:09:22.795121 dh-potluck-1.9.1/dh_potluck/messaging/message_envelope_schema.py
+-rw-r--r--   0        0        0     6773 2022-12-16 15:13:28.171113 dh-potluck-1.9.1/dh_potluck/messaging/producer.py
+-rw-r--r--   0        0        0      223 2022-12-16 14:39:36.598070 dh-potluck-1.9.1/dh_potluck/messaging/typings.py
+-rw-r--r--   0        0        0     1237 2022-12-16 15:09:52.024881 dh-potluck-1.9.1/dh_potluck/messaging/utils.py
+-rw-r--r--   0        0        0     1056 2022-09-22 16:49:17.730980 dh-potluck-1.9.1/dh_potluck/mixpanel.py
+-rw-r--r--   0        0        0     2279 2021-03-04 17:49:50.742112 dh-potluck-1.9.1/dh_potluck/platform_connection.py
+-rw-r--r--   0        0        0     1703 2021-03-04 17:49:50.742425 dh-potluck-1.9.1/dh_potluck/queries_summary.py
+-rw-r--r--   0        0        0     2575 2022-09-22 16:49:17.731301 dh-potluck-1.9.1/dh_potluck/s3_service.py
+-rw-r--r--   0        0        0      557 2022-10-28 13:13:57.296625 dh-potluck-1.9.1/dh_potluck/templates/redoc.html
+-rw-r--r--   0        0        0        0 2022-09-22 16:49:17.731458 dh-potluck-1.9.1/dh_potluck/types/__init__.py
+-rw-r--r--   0        0        0      884 2022-09-22 16:49:17.731721 dh-potluck-1.9.1/dh_potluck/types/json_serializable.py
+-rw-r--r--   0        0        0        0 2020-11-05 18:11:29.232285 dh-potluck-1.9.1/dh_potluck/utils/__init__.py
+-rw-r--r--   0        0        0      478 2021-03-04 17:49:50.742907 dh-potluck-1.9.1/dh_potluck/utils/term.py
+-rw-r--r--   0        0        0     2019 2022-12-16 15:51:42.911759 dh-potluck-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1174 2022-12-19 20:20:48.316770 dh-potluck-1.9.1/setup.py
+-rw-r--r--   0        0        0     1025 2022-12-19 20:20:48.317007 dh-potluck-1.9.1/PKG-INFO
```

### Comparing `dh-potluck-1.9.0/dh_potluck/__init__.py` & `dh-potluck-1.9.1/dh_potluck/__init__.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/api_docs.py` & `dh-potluck-1.9.1/dh_potluck/api_docs.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/auth.py` & `dh-potluck-1.9.1/dh_potluck/auth.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/celery/crontab_parser.py` & `dh-potluck-1.9.1/dh_potluck/celery/crontab_parser.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/celery/signals.py` & `dh-potluck-1.9.1/dh_potluck/celery/signals.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/celery/synchronization.py` & `dh-potluck-1.9.1/dh_potluck/celery/synchronization.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/decorators.py` & `dh-potluck-1.9.1/dh_potluck/decorators.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/email/email_service.py` & `dh-potluck-1.9.1/dh_potluck/email/email_service.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/email/mandrill_email_client.py` & `dh-potluck-1.9.1/dh_potluck/email/mandrill_email_client.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/extension.py` & `dh-potluck-1.9.1/dh_potluck/extension.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/fields.py` & `dh-potluck-1.9.1/dh_potluck/fields.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/health_checks.py` & `dh-potluck-1.9.1/dh_potluck/health_checks.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/image_api.py` & `dh-potluck-1.9.1/dh_potluck/image_api.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/logging.py` & `dh-potluck-1.9.1/dh_potluck/logging.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/messaging/__init__.py` & `dh-potluck-1.9.1/dh_potluck/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/messaging/batching_consumer.py` & `dh-potluck-1.9.1/dh_potluck/messaging/batching_consumer.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,28 +34,36 @@
         self,
         consumer_group_id: str,
         batch_size: int,
         release_after: float,
         auto_commit: bool = True,
         poll_timeout: float = 1.0,
         config_overrides: Optional[ConsumerConfig] = None,
+        brokers: Optional[str] = None,
+        should_connect_ssl: Optional[bool] = None,
     ) -> None:
         """
         BatchingMessageConsumer is a consumer that waits to collect batches of messages before
         releasing them for consumption
         :param str consumer_group_id: The kafka consumer group ID to use
         :param int batch_size: The max number of messages to collect before releasing a batch
         :param float release_after: How long to wait before releasing a batch if batch_size isn't
             exceeded (in milliseconds)
         :param bool auto_commit: If truthy, BatchingMessageConsumer will commit offsets for a batch
             under the hood. If falsy, then developers will be responsible for this behavior
         :param float poll_timeout: The poll_timeout config to pass to the inner Kafka consumer
         :param dict config_overrides: Custom config to pass to the inner Kafka consumer
+        :param str brokers: list of brokers to connect to (also can be provided via the flask
+            config `KAFKA_BROKERS_LIST`)
+        :param bool should_connect_ssl: if a ssl connection should be used to kafka (also can be
+            provided via the flask config `KAFKA_USE_SSL_CONNECTION`)
         """
-        self._consumer = Consumer(build_consumer_config(consumer_group_id, config_overrides))
+        self._consumer = Consumer(
+            build_consumer_config(consumer_group_id, config_overrides, brokers, should_connect_ssl)
+        )
         self._batch_size = batch_size
         self._release_after = release_after
         self._auto_commit = auto_commit
         self._poll_timeout = poll_timeout
         self._shutdown = False
         self._batch_results = []
         self._batch_deadline = None
```

### Comparing `dh-potluck-1.9.0/dh_potluck/messaging/consumer.py` & `dh-potluck-1.9.1/dh_potluck/messaging/consumer.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,20 +16,28 @@
     _is_consuming: bool = False
     _message_schema: MessageEnvelopeSchema = MessageEnvelopeSchema()
 
     def __init__(
         self,
         consumer_group: str,
         config_overrides: Optional[ConsumerConfig] = None,
+        brokers: Optional[str] = None,
+        should_connect_ssl: Optional[bool] = None,
     ):
         """
         :param str consumer_group: The kafka consumer group to use
         :param dict config_overrides: Any kafka configuration overrides
+        :param str brokers: list of brokers to connect to (also can be provided via the flask
+            config `KAFKA_BROKERS_LIST`)
+        :param bool should_connect_ssl: if a ssl connection should be used to kafka (also can be
+            provided via the flask config `KAFKA_USE_SSL_CONNECTION`)
         """
-        self._consumer = Consumer(build_consumer_config(consumer_group, config_overrides))
+        self._consumer = Consumer(
+            build_consumer_config(consumer_group, config_overrides, brokers, should_connect_ssl)
+        )
 
     def subscribe(self, topics: List[str]) -> None:
         """
         Subscribe to the list of topics, this makes the connection to Kafka
         :param topics: Topics to connect to
         :return: None
         """
```

### Comparing `dh-potluck-1.9.0/dh_potluck/messaging/incoming_message_router.py` & `dh-potluck-1.9.1/dh_potluck/messaging/incoming_message_router.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,21 +49,29 @@
     _consumer: MessageConsumer
 
     def __init__(
         self,
         handlers: Dict[str, MessageHandler],
         consumer_group: str,
         config_overrides: Optional[ConsumerConfig] = None,
+        brokers: Optional[str] = None,
+        should_connect_ssl: Optional[bool] = None,
     ):
         """
         :param dict handlers: Dictionary of topic -> MessageHandler
         :param str consumer_group: The kafka consumer group to use
         :param dict config_overrides: Any kafka configuration overrides
+        :param str brokers: list of brokers to connect to (also can be provided via the flask
+            config `KAFKA_BROKERS_LIST`)
+        :param bool should_connect_ssl: if a ssl connection should be used to kafka (also can be
+            provided via the flask config `KAFKA_USE_SSL_CONNECTION`)
         """
-        self._consumer = MessageConsumer(consumer_group, config_overrides)
+        self._consumer = MessageConsumer(
+            consumer_group, config_overrides, brokers, should_connect_ssl
+        )
         self._handlers = handlers
 
     def run(self) -> None:
         """
         Start consuming messages. On new messages, check the handlers map, if the message's topic
         matches a handler key, use it to serialize the message, and handle it.
         :return: None
```

### Comparing `dh-potluck-1.9.0/dh_potluck/messaging/message.py` & `dh-potluck-1.9.1/dh_potluck/messaging/message.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/messaging/message_consumer_app.py` & `dh-potluck-1.9.1/dh_potluck/messaging/message_consumer_app.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,20 +26,32 @@
     return decorator_register_message_handler
 
 
 class MessageConsumerApp(object):
 
     _router: IncomingMessageRouter
 
-    def __init__(self, consumer_group: str, config_overrides: Optional[ConsumerConfig] = None):
+    def __init__(
+        self,
+        consumer_group: str,
+        config_overrides: Optional[ConsumerConfig] = None,
+        brokers: Optional[str] = None,
+        should_connect_ssl: Optional[bool] = None,
+    ):
         """
         :param str consumer_group: The kafka consumer group to use
         :param dict config_overrides: Any kafka configuration overrides
+        :param str brokers: list of brokers to connect to (also can be provided via the flask
+            config `KAFKA_BROKERS_LIST`)
+        :param bool should_connect_ssl: if a ssl connection should be used to kafka (also can be
+            provided via the flask config `KAFKA_USE_SSL_CONNECTION`)
         """
-        self._router = IncomingMessageRouter(_HANDLERS, consumer_group, config_overrides)
+        self._router = IncomingMessageRouter(
+            _HANDLERS, consumer_group, config_overrides, brokers, should_connect_ssl
+        )
 
     def run(self):
         """
         Start consuming messages. On new messages, use the registered message_handler to handle it.
         :return: None
         """
         self._router.run()
```

### Comparing `dh-potluck-1.9.0/dh_potluck/messaging/producer.py` & `dh-potluck-1.9.1/dh_potluck/messaging/producer.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,35 +6,48 @@
 from confluent_kafka.cimpl import KafkaError, KafkaException
 from confluent_kafka.cimpl import Message as KafkaMessage
 from ddtrace import tracer
 from flask import current_app
 from marshmallow import Schema, ValidationError
 
 from dh_potluck.messaging import MessageEnvelopeSchema
+from dh_potluck.messaging.constants import BROKER_LIST_CONFIG_KEY, USE_SSL_CONFIG_KEY
+from dh_potluck.messaging.exceptions import NoBrokersFoundException
 
 LOG = logging.getLogger(__name__)
 
 
 class MessageProducer(object):
 
     _producer: Producer
     _message_schema: MessageEnvelopeSchema = MessageEnvelopeSchema()
 
-    def __init__(self, config_overrides: Optional[Dict[str, object]] = None):
+    def __init__(
+        self,
+        config_overrides: Optional[Dict[str, object]] = None,
+        brokers: Optional[str] = None,
+        should_connect_ssl: Optional[bool] = None,
+    ):
         """
         :param dict config_overrides: Any kafka configuration overrides
+        :param str brokers: list of brokers to connect to (also can be provided via the flask
+            config `KAFKA_BROKERS_LIST`)
+        :param bool should_connect_ssl: if a ssl connection should be used to kafka (also can be
+            provided via the flask config `KAFKA_USE_SSL_CONNECTION`)
         """
-        brokers: str = current_app.config['KAFKA_BROKERS_LIST']
         if brokers is None:
-            raise RuntimeError(
-                'Tried to instantiate a MessageProducer '
-                'without setting the KAFKA_BROKERS_LIST env var'
+            brokers = current_app.config[BROKER_LIST_CONFIG_KEY]
+        if brokers is None:
+            raise NoBrokersFoundException(
+                'Tried to instantiate a MessageProducer without providing '
+                f'brokers or setting the {BROKER_LIST_CONFIG_KEY} env var'
             )
         config: Dict[str, object] = {'bootstrap.servers': brokers}
-        should_connect_ssl: bool = current_app.config['KAFKA_USE_SSL_CONNECTION']
+        if should_connect_ssl is None:
+            should_connect_ssl = current_app.config[USE_SSL_CONFIG_KEY]
         if should_connect_ssl:
             config['security.protocol'] = 'SSL'
         if config_overrides:
             config.update(config_overrides)
         self._producer = Producer(config)
 
     @staticmethod
```

### Comparing `dh-potluck-1.9.0/dh_potluck/messaging/utils.py` & `dh-potluck-1.9.1/dh_potluck/messaging/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 from typing import Optional
 
 from flask import current_app
 
+from dh_potluck.messaging.constants import BROKER_LIST_CONFIG_KEY, USE_SSL_CONFIG_KEY
 from dh_potluck.messaging.exceptions import NoBrokersFoundException
 from dh_potluck.messaging.typings import ConsumerConfig
 
 
 def build_consumer_config(
-    consumer_group_id: str, config_overrides: Optional[ConsumerConfig] = None
+    consumer_group_id: str,
+    config_overrides: Optional[ConsumerConfig] = None,
+    brokers: Optional[str] = None,
+    should_connect_ssl: Optional[bool] = None,
 ) -> ConsumerConfig:
-    brokers = current_app.config['KAFKA_BROKERS_LIST']
+    if brokers is None:
+        brokers = current_app.config[BROKER_LIST_CONFIG_KEY]
     if not brokers:
-        raise NoBrokersFoundException
+        raise NoBrokersFoundException(
+            'Tried to instantiate a MessageConsumer without providing '
+            f'brokers or setting the {BROKER_LIST_CONFIG_KEY} env var'
+        )
 
     config: ConsumerConfig = {
         'bootstrap.servers': brokers,
         'group.id': consumer_group_id,
         'enable.auto.commit': False,
         'auto.offset.reset': 'earliest',
     }
-    should_connect_ssl = current_app.config.get('KAFKA_USE_SSL_CONNECTION')
+
+    if should_connect_ssl is None:
+        should_connect_ssl = current_app.config.get(USE_SSL_CONFIG_KEY)
     if should_connect_ssl:
         config['security.protocol'] = 'SSL'
     if config_overrides:
         config.update(config_overrides)
     return config
```

### Comparing `dh-potluck-1.9.0/dh_potluck/mixpanel.py` & `dh-potluck-1.9.1/dh_potluck/mixpanel.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/platform_connection.py` & `dh-potluck-1.9.1/dh_potluck/platform_connection.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/queries_summary.py` & `dh-potluck-1.9.1/dh_potluck/queries_summary.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/s3_service.py` & `dh-potluck-1.9.1/dh_potluck/s3_service.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/templates/redoc.html` & `dh-potluck-1.9.1/dh_potluck/templates/redoc.html`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/dh_potluck/types/json_serializable.py` & `dh-potluck-1.9.1/dh_potluck/types/json_serializable.py`

 * *Files identical despite different names*

### Comparing `dh-potluck-1.9.0/pyproject.toml` & `dh-potluck-1.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dh-potluck"
-version = "1.9.0"
+version = "1.9.1"
 authors = []
 description = ""
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Flask = "~2.1.3"
 marshmallow = "^3.18.0"
```

### Comparing `dh-potluck-1.9.0/setup.py` & `dh-potluck-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  'requests>=2.28.1,<3.0.0',
  'setuptools>=65.5.0,<66.0.0',
  'sqlalchemy>=1.3,<2.0',
  'werkzeug>=2.2.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'dh-potluck',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': '',
     'long_description': None,
     'author': None,
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `dh-potluck-1.9.0/PKG-INFO` & `dh-potluck-1.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: dh-potluck
-Version: 1.9.0
+Version: 1.9.1
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask (>=2.1.3,<2.2.0)
 Requires-Dist: boltons (>=20.2.1,<21.0.0)
 Requires-Dist: boto3 (>=1.25.4,<2.0.0)
 Requires-Dist: confluent-kafka (>=1.8.2,<1.9.0)
 Requires-Dist: ddtrace (==1.1.1)
```


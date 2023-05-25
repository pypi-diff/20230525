# Comparing `tmp/tc-messageBroker-1.0.0.tar.gz` & `tmp/tc-messageBroker-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-messageBroker-1.0.0.tar", last modified: Wed May 24 07:57:47 2023, max compression
+gzip compressed data, was "tc-messageBroker-1.1.0.tar", last modified: Thu May 25 12:45:42 2023, max compression
```

## Comparing `tc-messageBroker-1.0.0.tar` & `tc-messageBroker-1.1.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.286259 tc-messageBroker-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-24 07:57:47.286259 tc-messageBroker-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 07:57:47.286259 tc-messageBroker-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.282259 tc-messageBroker-1.0.0/tc_messageBroker/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/message_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.282259 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.282259 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/db_operations/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/db_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.282259 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/event/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/event/events_microservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.282259 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/queue/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/queue/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.286259 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/choreography.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/choreography_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/saga.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.286259 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.282259 tc-messageBroker-1.0.0/tc_messageBroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-24 07:57:47.000000 tc-messageBroker-1.0.0/tc_messageBroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-24 07:57:47.000000 tc-messageBroker-1.0.0/tc_messageBroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:57:47.000000 tc-messageBroker-1.0.0/tc_messageBroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 07:57:47.000000 tc-messageBroker-1.0.0/tc_messageBroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 07:57:47.000000 tc-messageBroker-1.0.0/tc_messageBroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.286259 tc-messageBroker-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.286259 tc-messageBroker-1.0.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/integration/test_message_broker_exchange_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/integration/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/integration/test_saga.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:47.286259 tc-messageBroker-1.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/unit/test_choreagraphy_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/unit/test_enum_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/unit/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/unit/test_message_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/unit/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/unit/test_saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/unit/test_saga_next.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-24 07:57:23.000000 tc-messageBroker-1.0.0/tests/unit/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.178612 tc-messageBroker-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:45:42.178612 tc-messageBroker-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.170612 tc-messageBroker-1.1.0/tc_messageBroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/message_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/db_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/db_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/event/events_microservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/queue/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/choreography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/choreography_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/saga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.170612 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 12:45:42.000000 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-25 12:45:42.000000 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:45:42.000000 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 12:45:42.000000 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 12:45:42.000000 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/integration/test_message_broker_exchange_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/integration/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/integration/test_saga.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_choreagraphy_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_enum_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_message_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_saga_next.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.0.0/PKG-INFO` & `tc-messageBroker-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.0.0
+Version: 1.1.0
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.0.0/README.md` & `tc-messageBroker-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.0.0/tc_messageBroker/message_broker.py` & `tc-messageBroker-1.1.0/tc_messageBroker/message_broker.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,30 @@
 # from typing import Callable
 import logging
 from datetime import datetime
 import json
 
 
 class RabbitMQ:
-    def __init__(self, broker_url: str) -> None:
+    def __init__(self, broker_url: str, port: int, username: str, password: str):
         logging.basicConfig()
         logging.getLogger().setLevel(logging.INFO)
 
         self.broker_url = broker_url
+        self.port = port
+        self._username = username
+        self._password = password
+
         ## it will use the default exchange point if not created
         self.exchange_name = ""
         self.channel = None
         self.connection = None
         self.event_function = {}
 
-    def __new__(cls, broker_url: str):
+    def __new__(cls, broker_url: str, port: int, username: str, password: str):
         ## making it singleton
         if not hasattr(cls, "instance"):
             cls.instance = super(RabbitMQ, cls).__new__(cls)
         return cls.instance
 
     def connect(self, queue_name: str, consume_options: dict = None) -> bool:
         """
@@ -39,17 +43,20 @@
         Returns:
         ---------
         is_successful : bool
             if True, connecting to rabbitMQ server was successful
             otherwise would return False
         """
         try:
+            credentials = pika.PlainCredentials(self._username, self._password)
             amqpServer = self.broker_url
             self.connection = pika.BlockingConnection(
-                pika.ConnectionParameters(amqpServer)
+                pika.ConnectionParameters(
+                    host=amqpServer, port=self.port, credentials=credentials
+                ),
             )
             self.channel = self.connection.channel()
 
             # make sure that the channel is created,
             # if not this statement will create it
             self.channel.queue_declare(queue=queue_name)
 
@@ -84,15 +91,15 @@
         body_serialized = json.loads(body)
         event = body_serialized["event"]
 
         if event not in self.event_function.keys():
             logging.info(" An Event was received that doesn't exist")
             self.channel.basic_reject(delivery_tag=method.delivery_tag, requeue=True)
         else:
-            self.event_function[event]()
+            self.event_function[event](body_serialized)
             self.channel.basic_ack(delivery_tag=method.delivery_tag)
 
     def consume(self, queue_name: str, consume_options: dict = None):
         """
         set consuming events from a queue
         """
         self.channel.queue_declare(queue=queue_name)
@@ -138,15 +145,15 @@
         """
         set a function to be called when an event happened
 
         Parameters:
         -------------
         event_name : str
             the event name we're setting the function for
-        on_message : str
+        on_message : callable
             the message when recieved (consumed) to call the function
 
         """
         self.event_function[event_name] = on_message
 
     def create_exchange(
         self,
```

### Comparing `tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py` & `tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/saga_base.py` & `tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/saga_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py` & `tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/transactions.py` & `tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/transactions.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     ),
     ITransaction(
         Queue.DISCORD_ANALYZER,
         Event.DISCORD_ANALYZER.RUN,
         order=2,
         status=Status.NOT_STARTED,
     ),
-    ITransaction(
-        Queue.DISCORD_ANALYZER,
-        Event.DISCORD_ANALYZER.SAVE,
-        order=3,
-        status=Status.NOT_STARTED,
-    ),
+    # ITransaction(
+    #     Queue.DISCORD_ANALYZER,
+    #     Event.DISCORD_ANALYZER.SAVE,
+    #     order=3,
+    #     status=Status.NOT_STARTED,
+    # ),
     ITransaction(
         Queue.SERVER_API,
         Event.SERVER_API.UPDATE_GUILD,
-        order=4,
+        order=3,
         status=Status.NOT_STARTED,
     ),
 ]
```

### Comparing `tc-messageBroker-1.0.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py` & `tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.0.0/tc_messageBroker.egg-info/PKG-INFO` & `tc-messageBroker-1.1.0/tc_messageBroker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.0.0
+Version: 1.1.0
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.0.0/tc_messageBroker.egg-info/SOURCES.txt` & `tc-messageBroker-1.1.0/tc_messageBroker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.0.0/tests/integration/test_mongodb.py` & `tc-messageBroker-1.1.0/tests/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.0.0/tests/integration/test_saga.py` & `tc-messageBroker-1.1.0/tests/integration/test_saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.0.0/tests/unit/test_saga_base.py` & `tc-messageBroker-1.1.0/tests/unit/test_saga_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     )
 
     ## it should sort the NOT_STARTED transactions
     (tx_sorted, not_started_count) = saga._sort_transactions(
         saga.choreography.transactions
     )
 
-    assert not_started_count == 4
+    assert not_started_count == 3
     order_val = 0
     for tx in tx_sorted:
         if tx.status == Status.NOT_STARTED:
             assert order_val < tx.order
             order_val = tx.order
 
 
@@ -41,15 +41,15 @@
     )
 
     ## it should sort the NOT_STARTED transactions
     (tx_sorted, not_started_count) = saga._sort_transactions(
         saga.choreography.transactions
     )
 
-    assert not_started_count == 4
+    assert not_started_count == 3
 
     condition = False
     for tx in tx_sorted:
         if tx.status == Status.NOT_STARTED:
             assert condition is False
         else:
             condition = True
```

### Comparing `tc-messageBroker-1.0.0/tests/unit/test_saga_next.py` & `tc-messageBroker-1.1.0/tests/unit/test_saga_next.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.0.0/tests/unit/test_transactions.py` & `tc-messageBroker-1.1.0/tests/unit/test_transactions.py`

 * *Files identical despite different names*


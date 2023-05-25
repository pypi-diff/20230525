# Comparing `tmp/rabbitmq-broker-1.0.0.tar.gz` & `tmp/rabbitmq-broker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitmq-broker-1.0.0.tar", last modified: Fri May 19 12:52:32 2023, max compression
+gzip compressed data, was "rabbitmq-broker-1.0.1.tar", last modified: Thu May 25 06:48:20 2023, max compression
```

## Comparing `rabbitmq-broker-1.0.0.tar` & `rabbitmq-broker-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.327794 rabbitmq-broker-1.0.0/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.0/HISTORY.rst
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1074 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.0/LICENSE
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      158 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.0/MANIFEST.in
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     4277 2023-05-19 12:52:32.327794 rabbitmq-broker-1.0.0/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     3893 2023-05-19 12:52:16.000000 rabbitmq-broker-1.0.0/README.md
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2023-05-18 13:42:42.000000 rabbitmq-broker-1.0.0/README.rst
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      599 2023-05-19 12:06:12.000000 rabbitmq-broker-1.0.0/pyproject.toml
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.319795 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     4277 2023-05-19 12:52:32.000000 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      566 2023-05-19 12:52:32.000000 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/SOURCES.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2023-05-19 12:52:32.000000 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/dependency_links.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       70 2023-05-19 12:52:32.000000 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/requires.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       11 2023-05-19 12:52:32.000000 rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/top_level.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      228 2023-05-19 12:06:03.000000 rabbitmq-broker-1.0.0/requirements.txt
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.323794 rabbitmq-broker-1.0.0/rmq_broker/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       22 2023-05-19 12:06:01.000000 rabbitmq-broker-1.0.0/rmq_broker/__init__.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.323794 rabbitmq-broker-1.0.0/rmq_broker/async_chains/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/async_chains/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     7340 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/async_chains/base.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.323794 rabbitmq-broker-1.0.0/rmq_broker/chains/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.0/rmq_broker/chains/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     7304 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/chains/base.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-19 12:52:32.327794 rabbitmq-broker-1.0.0/rmq_broker/queues/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.0/rmq_broker/queues/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1107 2023-05-18 14:09:24.000000 rabbitmq-broker-1.0.0/rmq_broker/queues/base.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1765 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/queues/rabbitmq.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      620 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/schemas.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      512 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.0/rmq_broker/settings.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      928 2023-05-19 12:52:32.327794 rabbitmq-broker-1.0.0/setup.cfg
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-25 06:48:20.145397 rabbitmq-broker-1.0.1/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.1/HISTORY.rst
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1074 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.1/LICENSE
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      158 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.1/MANIFEST.in
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     4263 2023-05-25 06:48:20.145397 rabbitmq-broker-1.0.1/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     3879 2023-05-25 06:48:06.000000 rabbitmq-broker-1.0.1/README.md
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2023-05-18 13:42:42.000000 rabbitmq-broker-1.0.1/README.rst
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      599 2023-05-25 06:48:06.000000 rabbitmq-broker-1.0.1/pyproject.toml
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-25 06:48:20.141397 rabbitmq-broker-1.0.1/rabbitmq_broker.egg-info/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     4263 2023-05-25 06:48:20.000000 rabbitmq-broker-1.0.1/rabbitmq_broker.egg-info/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      566 2023-05-25 06:48:20.000000 rabbitmq-broker-1.0.1/rabbitmq_broker.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2023-05-25 06:48:20.000000 rabbitmq-broker-1.0.1/rabbitmq_broker.egg-info/dependency_links.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       70 2023-05-25 06:48:20.000000 rabbitmq-broker-1.0.1/rabbitmq_broker.egg-info/requires.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       11 2023-05-25 06:48:20.000000 rabbitmq-broker-1.0.1/rabbitmq_broker.egg-info/top_level.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      227 2023-05-25 06:48:06.000000 rabbitmq-broker-1.0.1/requirements.txt
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-25 06:48:20.145397 rabbitmq-broker-1.0.1/rmq_broker/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       22 2023-05-25 06:48:06.000000 rabbitmq-broker-1.0.1/rmq_broker/__init__.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-25 06:48:20.145397 rabbitmq-broker-1.0.1/rmq_broker/async_chains/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.1/rmq_broker/async_chains/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     7529 2023-05-25 06:48:06.000000 rabbitmq-broker-1.0.1/rmq_broker/async_chains/base.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-25 06:48:20.145397 rabbitmq-broker-1.0.1/rmq_broker/chains/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.1/rmq_broker/chains/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     7493 2023-05-25 06:48:06.000000 rabbitmq-broker-1.0.1/rmq_broker/chains/base.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2023-05-25 06:48:20.145397 rabbitmq-broker-1.0.1/rmq_broker/queues/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2023-05-18 13:33:44.000000 rabbitmq-broker-1.0.1/rmq_broker/queues/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1107 2023-05-18 14:09:24.000000 rabbitmq-broker-1.0.1/rmq_broker/queues/base.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1765 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.1/rmq_broker/queues/rabbitmq.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      620 2023-05-18 13:36:17.000000 rabbitmq-broker-1.0.1/rmq_broker/schemas.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      508 2023-05-24 20:33:15.000000 rabbitmq-broker-1.0.1/rmq_broker/settings.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      928 2023-05-25 06:48:20.149398 rabbitmq-broker-1.0.1/setup.cfg
```

### Comparing `rabbitmq-broker-1.0.0/LICENSE` & `rabbitmq-broker-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-1.0.0/PKG-INFO` & `rabbitmq-broker-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitmq-broker
-Version: 1.0.0
+Version: 1.0.1
 Summary: RPC брокер сообщений
 Author-email: Nikita Sysoev <njt55cs@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 # RabbitMQ Broker
 [![Python versions](https://img.shields.io/badge/python-%3E=3.9-blue)](https://www.python.org/)
 [![Docker version](https://img.shields.io/badge/Docker-23.0.1-blue)](https://www.docker.com//)
 [![](https://img.shields.io/badge/-FastAPI-green)](https://fastapi.tiangolo.com/)
 [![Black code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Isort imports](https://img.shields.io/badge/imports-isort-31674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-![coverage](http://192.168.32.52/gazprom-asez/webportal-logic/badges/develop/coverage.svg) 
+![coverage](http://192.168.32.52/gazprom-asez/webportal-logic/badges/develop/coverage.svg)
 
 Не зависящий от фреймворков пакет для общения между микросервисами. Пакет предоставляет интерфейс для работы с брокером сообщений `RabbitMQ` и базовый класс цепочки обработчиков.
 
 Пакет реализует паттерн цепочка обязанностей в синхронном и асинхронном виде.
 
 ## Конфигурация
 
@@ -47,24 +47,24 @@
     def get_response_body(self, data: dict) -> dict:
         ...
 ```
 
 Также, можно унаследоваться от асинхронного варианта реализации:
 ```
 from rmq_broker.async_chains.base import BaseChain
-    
-    
+
+
 class LoginChain(BaseChain):
     request_type = "login"
-    
+
     async def get_response_body(self, data: dict) -> dict:
         ...
 ```
 
-Метод должен содержать логику обработки запроса и вызывать родительский метод 
+Метод должен содержать логику обработки запроса и вызывать родительский метод
 `BaseChain.form_response(data, body, code, message)`
 ```
 class LoginChain(BaseChain):
     request_type = "login"
 
     async def get_response_body(self, data):
         # Обработка запроса
```

### Comparing `rabbitmq-broker-1.0.0/README.md` & `rabbitmq-broker-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # RabbitMQ Broker
 [![Python versions](https://img.shields.io/badge/python-%3E=3.9-blue)](https://www.python.org/)
 [![Docker version](https://img.shields.io/badge/Docker-23.0.1-blue)](https://www.docker.com//)
 [![](https://img.shields.io/badge/-FastAPI-green)](https://fastapi.tiangolo.com/)
 [![Black code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Isort imports](https://img.shields.io/badge/imports-isort-31674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-![coverage](http://192.168.32.52/gazprom-asez/webportal-logic/badges/develop/coverage.svg) 
+![coverage](http://192.168.32.52/gazprom-asez/webportal-logic/badges/develop/coverage.svg)
 
 Не зависящий от фреймворков пакет для общения между микросервисами. Пакет предоставляет интерфейс для работы с брокером сообщений `RabbitMQ` и базовый класс цепочки обработчиков.
 
 Пакет реализует паттерн цепочка обязанностей в синхронном и асинхронном виде.
 
 ## Конфигурация
 
@@ -35,24 +35,24 @@
     def get_response_body(self, data: dict) -> dict:
         ...
 ```
 
 Также, можно унаследоваться от асинхронного варианта реализации:
 ```
 from rmq_broker.async_chains.base import BaseChain
-    
-    
+
+
 class LoginChain(BaseChain):
     request_type = "login"
-    
+
     async def get_response_body(self, data: dict) -> dict:
         ...
 ```
 
-Метод должен содержать логику обработки запроса и вызывать родительский метод 
+Метод должен содержать логику обработки запроса и вызывать родительский метод
 `BaseChain.form_response(data, body, code, message)`
 ```
 class LoginChain(BaseChain):
     request_type = "login"
 
     async def get_response_body(self, data):
         # Обработка запроса
```

### Comparing `rabbitmq-broker-1.0.0/pyproject.toml` & `rabbitmq-broker-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rabbitmq-broker"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Nikita Sysoev", email="njt55cs@gmail.com" },
 ]
 description = "RPC брокер сообщений"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/PKG-INFO` & `rabbitmq-broker-1.0.1/rabbitmq_broker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitmq-broker
-Version: 1.0.0
+Version: 1.0.1
 Summary: RPC брокер сообщений
 Author-email: Nikita Sysoev <njt55cs@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 # RabbitMQ Broker
 [![Python versions](https://img.shields.io/badge/python-%3E=3.9-blue)](https://www.python.org/)
 [![Docker version](https://img.shields.io/badge/Docker-23.0.1-blue)](https://www.docker.com//)
 [![](https://img.shields.io/badge/-FastAPI-green)](https://fastapi.tiangolo.com/)
 [![Black code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Isort imports](https://img.shields.io/badge/imports-isort-31674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-![coverage](http://192.168.32.52/gazprom-asez/webportal-logic/badges/develop/coverage.svg) 
+![coverage](http://192.168.32.52/gazprom-asez/webportal-logic/badges/develop/coverage.svg)
 
 Не зависящий от фреймворков пакет для общения между микросервисами. Пакет предоставляет интерфейс для работы с брокером сообщений `RabbitMQ` и базовый класс цепочки обработчиков.
 
 Пакет реализует паттерн цепочка обязанностей в синхронном и асинхронном виде.
 
 ## Конфигурация
 
@@ -47,24 +47,24 @@
     def get_response_body(self, data: dict) -> dict:
         ...
 ```
 
 Также, можно унаследоваться от асинхронного варианта реализации:
 ```
 from rmq_broker.async_chains.base import BaseChain
-    
-    
+
+
 class LoginChain(BaseChain):
     request_type = "login"
-    
+
     async def get_response_body(self, data: dict) -> dict:
         ...
 ```
 
-Метод должен содержать логику обработки запроса и вызывать родительский метод 
+Метод должен содержать логику обработки запроса и вызывать родительский метод
 `BaseChain.form_response(data, body, code, message)`
 ```
 class LoginChain(BaseChain):
     request_type = "login"
 
     async def get_response_body(self, data):
         # Обработка запроса
```

### Comparing `rabbitmq-broker-1.0.0/rabbitmq_broker.egg-info/SOURCES.txt` & `rabbitmq-broker-1.0.1/rabbitmq_broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-1.0.0/rmq_broker/async_chains/base.py` & `rabbitmq-broker-1.0.1/rmq_broker/async_chains/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,15 +147,20 @@
             "%s: handle(data): Successful validation" % self.__class__.__name__
         )
         response = {}
         if data["request_type"] == self.request_type:
             response["request_id"] = data["request_id"]
             response["request_type"] = data["request_type"]
             logger.info("%s: get_response_body(data)" % self.__class__.__name__)
-            response.update(await self.get_response_body(data))
+            try:
+                response.update(await self.get_response_body(data))
+            except Exception as e:
+                return self.form_response(
+                    MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
+                )
             logger.info(
                 "%s: get_response_header(data) data=%s"
                 % (self.__class__.__name__, data)
             )
             response.update(self.get_response_header(data))
             logger.info(f"{self.__class__.__name__}: handle(data) response={response}")
             try:
```

### Comparing `rabbitmq-broker-1.0.0/rmq_broker/chains/base.py` & `rabbitmq-broker-1.0.1/rmq_broker/chains/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,15 +147,20 @@
             "%s: handle(data): Successful validation" % self.__class__.__name__
         )
         response = {}
         if data["request_type"] == self.request_type:
             response["request_id"] = data["request_id"]
             response["request_type"] = data["request_type"]
             logger.info("%s: get_response_body(data)" % self.__class__.__name__)
-            response.update(self.get_response_body(data))
+            try:
+                response.update(self.get_response_body(data))
+            except Exception as e:
+                return self.form_response(
+                    MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
+                )
             logger.info(
                 "%s: get_response_header(data) data=%s"
                 % (self.__class__.__name__, data)
             )
             response.update(self.get_response_header(data))
             logger.info(f"{self.__class__.__name__}: handle(data) response={response}")
             try:
```

### Comparing `rabbitmq-broker-1.0.0/rmq_broker/queues/base.py` & `rabbitmq-broker-1.0.1/rmq_broker/queues/base.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-1.0.0/rmq_broker/queues/rabbitmq.py` & `rabbitmq-broker-1.0.1/rmq_broker/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-1.0.0/rmq_broker/schemas.py` & `rabbitmq-broker-1.0.1/rmq_broker/schemas.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-broker-1.0.0/setup.cfg` & `rabbitmq-broker-1.0.1/setup.cfg`

 * *Files identical despite different names*


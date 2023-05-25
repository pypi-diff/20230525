# Comparing `tmp/bovine_pubsub-0.2.0.tar.gz` & `tmp/bovine_pubsub-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_pubsub-0.2.0.tar", max compression
+gzip compressed data, was "bovine_pubsub-0.2.1.tar", max compression
```

## Comparing `bovine_pubsub-0.2.0.tar` & `bovine_pubsub-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0       68 2023-05-22 14:17:04.666842 bovine_pubsub-0.2.0/README.md
--rw-r--r--   0        0        0     1132 2023-05-22 14:17:04.666842 bovine_pubsub-0.2.0/bovine_pubsub/__init__.py
--rw-r--r--   0        0        0      354 2023-05-22 14:17:04.666842 bovine_pubsub-0.2.0/bovine_pubsub/test_app.py
--rw-r--r--   0        0        0      632 2023-05-22 14:17:04.670843 bovine_pubsub-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 bovine_pubsub-0.2.0/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 bovine_pubsub-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-05-22 14:17:04.666842 bovine_pubsub-0.2.1/README.md
+-rw-r--r--   0        0        0      279 2023-05-25 18:44:02.790690 bovine_pubsub-0.2.1/bovine_pubsub/__init__.py
+-rw-r--r--   0        0        0      493 2023-05-25 18:44:02.790690 bovine_pubsub-0.2.1/bovine_pubsub/queue.py
+-rw-r--r--   0        0        0     1091 2023-05-25 18:44:02.790690 bovine_pubsub-0.2.1/bovine_pubsub/redis.py
+-rw-r--r--   0        0        0      258 2023-05-25 18:44:02.790690 bovine_pubsub-0.2.1/bovine_pubsub/test_app.py
+-rw-r--r--   0        0        0      632 2023-05-25 18:44:02.790690 bovine_pubsub-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 bovine_pubsub-0.2.1/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 bovine_pubsub-0.2.1/PKG-INFO
```

### Comparing `bovine_pubsub-0.2.0/bovine_pubsub/__init__.py` & `bovine_pubsub-0.2.1/bovine_pubsub/redis.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import asyncio
+import logging
+from quart_redis import get_redis
 
-from quart_redis import RedisHandler, get_redis
+logger = logging.getLogger(__name__)
 
 
-async def configure_bovine_pub_sub(app):
-    app.config["REDIS_URI"] = "redis://localhost"
-
-    RedisHandler(app)
-    app.config["bovine_pub_sub"] = BovinePubSub()
-
-
-class BovinePubSub:
+class RedisBovinePubSub:
     def __init__(self):
         self.health_pings = {}
 
     async def send(self, endpoint_path, data):
         redis = get_redis()
         await redis.publish(endpoint_path, data)
 
     async def event_stream(self, endpoint_path):
-        self.health_pings[endpoint_path] = asyncio.create_task(
-            self.health_ping(endpoint_path)
-        )
-        redis = get_redis()
-        async with redis.pubsub() as pubsub:
-            await pubsub.subscribe(endpoint_path)
-            async for message in pubsub.listen():
-                if message["type"] == "message":
-                    msg = message["data"]
-                    yield msg
-                    yield "\n".encode("utf-8")
+        task = asyncio.create_task(self.health_ping(endpoint_path))
+
+        try:
+            redis = get_redis()
+            async with redis.pubsub() as pubsub:
+                await pubsub.subscribe(endpoint_path)
+                async for message in pubsub.listen():
+                    if message["type"] == "message":
+                        msg = message["data"]
+                        yield msg
+                        yield "\n".encode("utf-8")
+        finally:
+            logger.info("Cancelling task")
+            task.cancel()
 
     async def health_ping(self, endpoint_path):
         while True:
             await asyncio.sleep(30)
             await self.send(endpoint_path, (":" + " " * 2048 + "\n").encode("utf-8"))
```

### Comparing `bovine_pubsub-0.2.0/pyproject.toml` & `bovine_pubsub-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine-pubsub"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Quart Redis thing to handle pubsub tasks in particular the event source"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://codeberg.org/bovine/bovine"
 packages = [{include = "bovine_pubsub"}]
```

### Comparing `bovine_pubsub-0.2.0/setup.py` & `bovine_pubsub-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['quart-redis>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'bovine-pubsub',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'A Quart Redis thing to handle pubsub tasks in particular the event source',
     'long_description': '# bovine_pubsub\n\nRequires redis. Usage see `examples/basic_app.py`.\n',
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/bovine/bovine',
```

### Comparing `bovine_pubsub-0.2.0/PKG-INFO` & `bovine_pubsub-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine-pubsub
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Quart Redis thing to handle pubsub tasks in particular the event source
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/aiodiskqueue-0.1.0a4.tar.gz` & `tmp/aiodiskqueue-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0a4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.0a5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0a4.tar` & `aiodiskqueue-0.1.0a5.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a4/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a4/.github/workflows/main.yml
--rw-r--r--   0        0        0      107 2023-05-24 14:44:42.314154 aiodiskqueue-0.1.0a4/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a4/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     2098 2023-05-25 12:55:53.126334 aiodiskqueue-0.1.0a4/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a4/docs/Makefile
--rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0a4/docs/_static/custom.css
--rw-r--r--   0        0        0      228 2023-05-24 15:12:23.388951 aiodiskqueue-0.1.0a4/docs/api.rst
--rw-r--r--   0        0        0     1873 2023-05-25 13:02:52.209564 aiodiskqueue-0.1.0a4/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a4/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a4/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a4/examples/__init__.py
--rw-r--r--   0        0        0      210 2023-05-25 12:55:04.093686 aiodiskqueue-0.1.0a4/examples/basic_usage.py
--rw-r--r--   0        0        0     1768 2023-05-25 12:55:53.290336 aiodiskqueue-0.1.0a4/examples/consumer_producer_processes.py
--rw-r--r--   0        0        0     1045 2023-05-25 12:55:53.278336 aiodiskqueue-0.1.0a4/examples/multiple_consumers.py
--rw-r--r--   0        0        0      991 2023-05-25 12:55:53.234335 aiodiskqueue-0.1.0a4/examples/single_consumer.py
--rw-r--r--   0        0        0      943 2023-05-24 22:01:37.989063 aiodiskqueue-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0      188 2023-05-25 12:54:35.397381 aiodiskqueue-0.1.0a4/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0     3270 2023-05-25 13:05:14.303569 aiodiskqueue-0.1.0a4/src/aiodiskqueue/core.py
--rw-r--r--   0        0        0      212 2023-05-24 13:48:27.949169 aiodiskqueue-0.1.0a4/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a4/tests/__init__.py
--rw-r--r--   0        0        0     2122 2023-05-25 12:55:53.378337 aiodiskqueue-0.1.0a4/tests/test_core.py
--rw-r--r--   0        0        0      394 2023-05-24 14:12:01.108384 aiodiskqueue-0.1.0a4/tox.ini
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a5/.coveragerc
+-rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a5/.github/workflows/main.yml
+-rw-r--r--   0        0        0      107 2023-05-24 14:44:42.314154 aiodiskqueue-0.1.0a5/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a5/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     2012 2023-05-25 19:52:58.687290 aiodiskqueue-0.1.0a5/README.rst
+-rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a5/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0a5/docs/_static/custom.css
+-rw-r--r--   0        0        0      228 2023-05-24 15:12:23.388951 aiodiskqueue-0.1.0a5/docs/api.rst
+-rw-r--r--   0        0        0     1873 2023-05-25 13:02:52.209564 aiodiskqueue-0.1.0a5/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a5/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a5/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a5/examples/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-25 19:53:16.675360 aiodiskqueue-0.1.0a5/examples/basic_usage.py
+-rw-r--r--   0        0        0      933 2023-05-25 19:47:09.774293 aiodiskqueue-0.1.0a5/examples/multiple_consumers.py
+-rw-r--r--   0        0        0      879 2023-05-25 19:45:20.370257 aiodiskqueue-0.1.0a5/examples/single_consumer.py
+-rw-r--r--   0        0        0      943 2023-05-24 22:01:37.989063 aiodiskqueue-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-05-25 14:35:48.129507 aiodiskqueue-0.1.0a5/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0     4206 2023-05-25 20:16:18.165114 aiodiskqueue-0.1.0a5/src/aiodiskqueue/core.py
+-rw-r--r--   0        0        0      212 2023-05-24 13:48:27.949169 aiodiskqueue-0.1.0a5/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a5/tests/__init__.py
+-rw-r--r--   0        0        0     2695 2023-05-25 20:12:15.141090 aiodiskqueue-0.1.0a5/tests/test_core.py
+-rw-r--r--   0        0        0      394 2023-05-24 14:12:01.108384 aiodiskqueue-0.1.0a5/tox.ini
+-rw-r--r--   0        0        0     2818 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a5/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0a4/.github/workflows/main.yml` & `aiodiskqueue-0.1.0a5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a4/LICENSE` & `aiodiskqueue-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a4/README.rst` & `aiodiskqueue-0.1.0a5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Description
 -----------
 
 This library provides a persistent queue for Python AsyncIO.
 
 It's main advantage is that it's content will survive a normal process restart and potentially even a process crash.
 
-Each queue is stored in it's own SQLite database on disk to provide maximum isolation between queues. Using SQLite should also make the queue inherently process safe [needs confirmation].
+Each queue is stored in it's own SQLite database on disk to provide maximum isolation between queues.
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
```

### Comparing `aiodiskqueue-0.1.0a4/docs/Makefile` & `aiodiskqueue-0.1.0a5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a4/docs/conf.py` & `aiodiskqueue-0.1.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a4/docs/make.bat` & `aiodiskqueue-0.1.0a5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a4/examples/multiple_consumers.py` & `aiodiskqueue-0.1.0a5/examples/multiple_consumers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 """Example: Multiple producers and multiple consumers act in parallel."""
 
 import asyncio
 import random
 import string
 from pathlib import Path
 
-from aiodiskqueue import Queue, QueueEmpty
+from aiodiskqueue import Queue
 
 
 async def producer(queue: Queue, num: int):
     for letter in string.ascii_uppercase:
         msg = f"producer {num}: {letter}"
         await queue.put(msg)
         await asyncio.sleep(random.random() / 10)
 
 
 async def consumer(queue: Queue):
     while True:
-        try:
-            message = await queue.get()
-        except QueueEmpty:
-            await asyncio.sleep(0.05)
-        else:
-            print(message)
+        message = await queue.get()
+        print(message)
 
 
 async def main():
     path = Path.cwd() / "example_queue.sqlite"
     queue = await Queue.create(path)
     coroutines = [
         consumer(queue),
```

### Comparing `aiodiskqueue-0.1.0a4/examples/single_consumer.py` & `aiodiskqueue-0.1.0a5/examples/single_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 """Example: Multiple producers and a single consumer act in parallel."""
 
 import asyncio
 import random
 import string
 from pathlib import Path
 
-from aiodiskqueue import Queue, QueueEmpty
+from aiodiskqueue import Queue
 
 
 async def producer(queue: Queue, num: int):
     for letter in string.ascii_uppercase:
         msg = f"producer {num}: {letter}"
         await queue.put(msg)
         await asyncio.sleep(random.random() / 10)
 
 
 async def consumer(queue: Queue):
     while True:
-        try:
-            message = await queue.get()
-        except QueueEmpty:
-            await asyncio.sleep(0.05)
-        else:
-            print(message)
+        message = await queue.get()
+        print(message)
 
 
 async def main():
     path = Path.cwd() / "example_queue.sqlite"
     queue = await Queue.create(path)
     coroutines = [
         consumer(queue),
```

### Comparing `aiodiskqueue-0.1.0a4/pyproject.toml` & `aiodiskqueue-0.1.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a4/src/aiodiskqueue/core.py` & `aiodiskqueue-0.1.0a5/src/aiodiskqueue/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Core implementation of a persistent AsyncIO queue."""
 
+import asyncio
 import pickle
 from pathlib import Path
 from typing import Any, Union
 
 import aiosqlite
 
 from aiodiskqueue.exceptions import QueueEmpty
@@ -11,24 +12,27 @@
 
 class Queue:
     """A persistent AsyncIO queue.
 
     The queue has no upper limited and is constrained by available disk space only.
 
     Create a new object with the factory method :func:`create`.
+
+    This class is not thread safe.
     """
 
     def __init__(self, db_path: Union[str, Path]) -> None:
         """Note that when calling this method it is assumed
         that the queue DB already exists at the given path.
 
         Args:
             db_path: Path of an existing queue DB
         """
         self.db_path = Path(db_path)
+        self.has_new_item = asyncio.Condition()
 
     async def qsize(self) -> int:
         """Return the approximate size of the queue.
         Note, qsize() > 0 doesn’t guarantee that a subsequent get()
         will not raise :class:`.QueueEmpty`.
         """
         async with aiosqlite.connect(self.db_path, isolation_level=None) as db:
@@ -45,28 +49,49 @@
         If empty() returns False it doesn’t guarantee
         that a subsequent call to get() will not raise :class:`.QueueEmpty`.
         """
         return await self.qsize() == 0
 
     async def get(self) -> Any:
         """Remove and return an item from the queue.
-        If queue is empty, raise :class:`.QueueEmpty`.
+        If queue is empty, wait until an item is available.
         """
+
         async with aiosqlite.connect(self.db_path, isolation_level=None) as db:
-            db.row_factory = aiosqlite.Row
-            rows: list = await db.execute_fetchall(
-                """
+            while True:
+                try:
+                    return await self._fetch_item(db)
+                except QueueEmpty:
+                    pass
+                async with self.has_new_item:
+                    await self.has_new_item.wait()
+
+    async def get_nowait(self) -> Any:
+        """Remove and return an item if one is immediately available,
+        else raise :class:`.QueueEmpty`.
+        """
+        async with aiosqlite.connect(self.db_path, isolation_level=None) as db:
+            return await self._fetch_item(db)
+
+    async def _fetch_item(self, db: aiosqlite.Connection) -> Any:
+        """Make the DB call to remote and return an item
+        if one is immediately available else raise `QueueEmpty`.
+        """
+        db.row_factory = aiosqlite.Row
+        rows: list = await db.execute_fetchall(
+            """
                 DELETE FROM queue
                 RETURNING *
                 ORDER BY rowid
                 LIMIT 1;
                 """
-            )  # type: ignore
+        )  # type: ignore
         if rows:
-            return pickle.loads(rows[0]["item"])
+            item = pickle.loads(rows[0]["item"])
+            return item
         raise QueueEmpty()
 
     async def put(self, item: Any) -> None:
         """Put an item into the queue.
 
         Args:
             item: Any Python object that can be pickled
@@ -75,14 +100,16 @@
         async with aiosqlite.connect(self.db_path, isolation_level=None) as db:
             await db.execute(
                 """
                 INSERT INTO queue (item) VALUES (?);
                 """,
                 (data,),
             )
+        async with self.has_new_item:
+            self.has_new_item.notify()
 
     @classmethod
     async def create(cls, db_path: Union[str, Path]) -> "Queue":
         """Create a new queue object.
 
         A new queue DB will be created for this queue if it does not exist.
```

### Comparing `aiodiskqueue-0.1.0a4/tests/test_core.py` & `aiodiskqueue-0.1.0a5/tests/test_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import datetime as dt
 import shutil
 import tempfile
 from pathlib import Path
 from unittest import IsolatedAsyncioTestCase
 
 from aiodiskqueue import Queue, QueueEmpty
@@ -33,43 +34,59 @@
         self.assertEqual(result, 1)
 
     async def test_should_get_items(self):
         # given
         q = await Queue.create(self.db_path)
         await q.put("dummy")
         # when
-        result = await q.get()
+        result = await q.get_nowait()
         # then
         self.assertEqual(result, "dummy")
 
     async def test_should_handle_complex_items(self):
         # given
         q = await Queue.create(self.db_path)
         item = {
             "alpha": ["one", "two", "three"],
             "now": dt.datetime.now(tz=dt.timezone.utc),
         }
         await q.put(item)
         # when
-        result = await q.get()
+        result = await q.get_nowait()
         # then
         self.assertEqual(result, item)
 
     async def test_should_raise_exception_when_get_on_empty_queue(self):
         # given
         q = await Queue.create(self.db_path)
         # when/then
         with self.assertRaises(QueueEmpty):
-            await q.get()
+            await q.get_nowait()
 
     async def test_should_report_as_empty(self):
         # given
         q = await Queue.create(self.db_path)
         # when/then
         self.assertTrue(await q.empty())
 
     async def test_should_not_report_as_empty(self):
         # given
         q = await Queue.create(self.db_path)
         await q.put("dummy")
         # when/then
         self.assertFalse(await q.empty())
+
+    async def test_get_should_wait_until_item_is_available(self):
+        async def consumer():
+            item = await q.get()
+            await queue_2.put(item)
+
+        # given
+        queue_2 = asyncio.Queue()
+        q = await Queue.create(self.db_path)
+        asyncio.create_task(consumer())
+        # when
+        await asyncio.sleep(1)  # consumer sees an empty queue when task starts
+        await q.put("special-item")
+        # then
+        item = await queue_2.get_nowait()
+        self.assertEqual(item, "special-item")
```

### Comparing `aiodiskqueue-0.1.0a4/PKG-INFO` & `aiodiskqueue-0.1.0a5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Persistent queues for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -27,15 +27,15 @@
 Description
 -----------
 
 This library provides a persistent queue for Python AsyncIO.
 
 It's main advantage is that it's content will survive a normal process restart and potentially even a process crash.
 
-Each queue is stored in it's own SQLite database on disk to provide maximum isolation between queues. Using SQLite should also make the queue inherently process safe [needs confirmation].
+Each queue is stored in it's own SQLite database on disk to provide maximum isolation between queues.
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
```


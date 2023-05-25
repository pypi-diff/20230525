# Comparing `tmp/aiodiskqueue-0.1.0a2.tar.gz` & `tmp/aiodiskqueue-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.0a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0a2.tar` & `aiodiskqueue-0.1.0a3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a2/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a2/.github/workflows/main.yml
--rw-r--r--   0        0        0      107 2023-05-24 14:44:42.314154 aiodiskqueue-0.1.0a2/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a2/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     2098 2023-05-24 17:01:45.615031 aiodiskqueue-0.1.0a2/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a2/docs/Makefile
--rw-r--r--   0        0        0      228 2023-05-24 15:12:23.388951 aiodiskqueue-0.1.0a2/docs/api.rst
--rw-r--r--   0        0        0     1545 2023-05-24 15:28:28.604971 aiodiskqueue-0.1.0a2/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a2/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a2/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a2/examples/__init__.py
--rw-r--r--   0        0        0      210 2023-05-24 13:48:28.153169 aiodiskqueue-0.1.0a2/examples/basic_usage.py
--rw-r--r--   0        0        0     1768 2023-05-24 13:48:28.049169 aiodiskqueue-0.1.0a2/examples/consumer_producer_processes.py
--rw-r--r--   0        0        0     1045 2023-05-24 13:48:28.073169 aiodiskqueue-0.1.0a2/examples/multiple_consumers.py
--rw-r--r--   0        0        0      991 2023-05-24 13:48:28.073169 aiodiskqueue-0.1.0a2/examples/single_consumer.py
--rw-r--r--   0        0        0      911 2023-05-24 17:01:20.419148 aiodiskqueue-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      188 2023-05-24 16:56:21.656687 aiodiskqueue-0.1.0a2/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0     2838 2023-05-24 15:47:24.487374 aiodiskqueue-0.1.0a2/src/aiodiskqueue/core.py
--rw-r--r--   0        0        0      212 2023-05-24 13:48:27.949169 aiodiskqueue-0.1.0a2/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0      685 2023-05-24 12:22:48.648480 aiodiskqueue-0.1.0a2/src/aiodiskqueue/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a2/tests/__init__.py
--rw-r--r--   0        0        0     2277 2023-05-24 13:48:28.153169 aiodiskqueue-0.1.0a2/tests/test_core.py
--rw-r--r--   0        0        0      394 2023-05-24 14:12:01.108384 aiodiskqueue-0.1.0a2/tox.ini
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a3/.coveragerc
+-rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a3/.github/workflows/main.yml
+-rw-r--r--   0        0        0      107 2023-05-24 14:44:42.314154 aiodiskqueue-0.1.0a3/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a3/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     2085 2023-05-24 22:02:26.160973 aiodiskqueue-0.1.0a3/README.rst
+-rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a3/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0a3/docs/_static/custom.css
+-rw-r--r--   0        0        0      228 2023-05-24 15:12:23.388951 aiodiskqueue-0.1.0a3/docs/api.rst
+-rw-r--r--   0        0        0     1872 2023-05-24 21:58:07.301391 aiodiskqueue-0.1.0a3/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a3/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a3/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a3/examples/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-24 22:02:06.881009 aiodiskqueue-0.1.0a3/examples/basic_usage.py
+-rw-r--r--   0        0        0     1742 2023-05-24 22:02:26.288972 aiodiskqueue-0.1.0a3/examples/consumer_producer_processes.py
+-rw-r--r--   0        0        0     1032 2023-05-24 22:02:26.240972 aiodiskqueue-0.1.0a3/examples/multiple_consumers.py
+-rw-r--r--   0        0        0      978 2023-05-24 22:02:26.268972 aiodiskqueue-0.1.0a3/examples/single_consumer.py
+-rw-r--r--   0        0        0      943 2023-05-24 22:01:37.989063 aiodiskqueue-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-05-24 21:50:41.649493 aiodiskqueue-0.1.0a3/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0     2871 2023-05-24 22:11:19.807736 aiodiskqueue-0.1.0a3/src/aiodiskqueue/core.py
+-rw-r--r--   0        0        0      212 2023-05-24 13:48:27.949169 aiodiskqueue-0.1.0a3/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a3/tests/__init__.py
+-rw-r--r--   0        0        0     2031 2023-05-24 21:49:02.693441 aiodiskqueue-0.1.0a3/tests/test_core.py
+-rw-r--r--   0        0        0      394 2023-05-24 14:12:01.108384 aiodiskqueue-0.1.0a3/tox.ini
+-rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a3/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0a2/.github/workflows/main.yml` & `aiodiskqueue-0.1.0a3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a2/LICENSE` & `aiodiskqueue-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a2/README.rst` & `aiodiskqueue-0.1.0a3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 .. code:: python
 
    import asyncio
    from aiodiskqueue import Queue
 
    async def main():
-       q = await Queue.create("example_queue.sqlite")
+       q = Queue("example_queue.sqlite")
        await q.put("some item")
        item = await q.get()
        print(item)
 
    asyncio.run(main())
 
 Please see the examples folder for more usage examples.
```

### Comparing `aiodiskqueue-0.1.0a2/docs/Makefile` & `aiodiskqueue-0.1.0a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a2/docs/conf.py` & `aiodiskqueue-0.1.0a3/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,23 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.autodoc", "sphinx.ext.napoleon"]
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
+# -- Options for autodoc -----------------------------------------------------
+# autoclass_content = "both"
+autodoc_default_options = {
+    "members": True,
+    "member-order": "alphabetical",
+    "special-members": "__init__",
+    "undoc-members": True,
+    "exclude-members": "__weakref__",
+}
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "alabaster"
 html_theme_options = {
     "description": "Persistent queues for Python AsyncIO",
@@ -43,7 +52,8 @@
         "navigation.html",
         "relations.html",
         "searchbox.html",
     ],
 }
 
 html_static_path = ["_static"]
+html_css_files = ["custom.css"]
```

### Comparing `aiodiskqueue-0.1.0a2/docs/make.bat` & `aiodiskqueue-0.1.0a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a2/examples/consumer_producer_processes.py` & `aiodiskqueue-0.1.0a3/examples/consumer_producer_processes.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,22 +33,22 @@
             await asyncio.sleep(0.05)
         else:
             print(message)
 
 
 async def run_consumer():
     path = Path.cwd() / "example_queue.sqlite"
-    queue = await Queue.create(path)
+    queue = Queue(path)
     async with asyncio.TaskGroup() as tg:
         tg.create_task(consumer(queue))
 
 
 async def run_producer(num: int):
     path = Path.cwd() / "example_queue.sqlite"
-    queue = await Queue.create(path)
+    queue = Queue(path)
     async with asyncio.TaskGroup() as tg:
         tg.create_task(producer(queue, num))
 
 
 def run_consumer_process():
     asyncio.run(run_consumer())
```

### Comparing `aiodiskqueue-0.1.0a2/examples/multiple_consumers.py` & `aiodiskqueue-0.1.0a3/examples/multiple_consumers.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             await asyncio.sleep(0.05)
         else:
             print(message)
 
 
 async def main():
     path = Path.cwd() / "example_queue.sqlite"
-    queue = await Queue.create(path)
+    queue = Queue(path)
     coroutines = [
         consumer(queue),
         consumer(queue),
         producer(queue, 1),
         producer(queue, 2),
         producer(queue, 3),
         producer(queue, 4),
```

### Comparing `aiodiskqueue-0.1.0a2/examples/single_consumer.py` & `aiodiskqueue-0.1.0a3/examples/single_consumer.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             await asyncio.sleep(0.05)
         else:
             print(message)
 
 
 async def main():
     path = Path.cwd() / "example_queue.sqlite"
-    queue = await Queue.create(path)
+    queue = Queue(path)
     coroutines = [
         consumer(queue),
         producer(queue, 1),
         producer(queue, 2),
         producer(queue, 3),
     ]
     await asyncio.gather(*coroutines)
```

### Comparing `aiodiskqueue-0.1.0a2/pyproject.toml` & `aiodiskqueue-0.1.0a3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,7 +25,10 @@
 [project.urls]
 Documentation = "https://aiodiskqueue.readthedocs.io/en/latest/"
 Source = "https://github.com/ErikKalkoken/aiodiskqueue"
 Tracker = "https://github.com/ErikKalkoken/aiodiskqueue/issues"
 
 [tool.flit.module]
 name = "aiodiskqueue"
+
+[tool.isort]
+profile = "black"
```

### Comparing `aiodiskqueue-0.1.0a2/src/aiodiskqueue/core.py` & `aiodiskqueue-0.1.0a3/src/aiodiskqueue/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,51 @@
-"""Core implementation of a persistent asyncio queue."""
+"""Core implementation of a persistent AsyncIO queue."""
 
 import pickle
+import sqlite3
 from pathlib import Path
 from typing import Any, Union
 
 import aiosqlite
 
 from aiodiskqueue.exceptions import QueueEmpty
-from aiodiskqueue.utils import NoPublicConstructor
 
 
-class Queue(metaclass=NoPublicConstructor):
-    """A persistent asyncio queue.
+class Queue:
+    """A persistent AsyncIO queue.
 
     The queue has no upper limited and is constrained by available disk space only.
-
-    Create a new queue with the :func:`Queue.create` factory method.
     """
 
-    def __init__(self, _db_path: Path) -> None:
-        self.db_path = _db_path
+    def __init__(self, db_path: Union[str, Path]) -> None:
+        """Create a new queue object.
+
+        A new queue DB will be created for this queue if it does not exist.
+
+        If the queue DB does exist it will be reused
+        and it's content will be preserved.
+
+        Args:
+            db_path: Path of the SQLite DB to be created / used. e.g. `queue.sqlite`
+
+        Returns:
+            newly created queue object
+        """
+        self.db_path = Path(db_path)
+        with sqlite3.connect(self.db_path, isolation_level=None) as db:
+            db.execute(
+                """
+                CREATE TABLE IF NOT EXISTS queue (item BLOB);
+                """
+            )
 
     async def qsize(self) -> int:
         """Return the approximate size of the queue.
         Note, qsize() > 0 doesn’t guarantee that a subsequent get()
-        will not raise QueueEmpty.
+        will not raise :class:`.QueueEmpty`.
         """
         async with aiosqlite.connect(self.db_path, isolation_level=None) as db:
             rows: list = await db.execute_fetchall(
                 """
                 SELECT count(*) FROM queue;
                 """
             )  # type: ignore
@@ -57,31 +74,20 @@
                 """
             )  # type: ignore
         if rows:
             return pickle.loads(rows[0]["item"])
         raise QueueEmpty()
 
     async def put(self, item: Any) -> None:
-        """Put an item into the queue. Any item that can be pickled is allowed."""
+        """Put an item into the queue.
+
+        Args:
+            item: Any Python object that can be pickled
+        """
         data = pickle.dumps(item)
         async with aiosqlite.connect(self.db_path, isolation_level=None) as db:
             await db.execute(
                 """
                 INSERT INTO queue (item) VALUES (?);
                 """,
                 (data,),
             )
-
-    @classmethod
-    async def create(cls, db_path: Union[str, Path]) -> "Queue":
-        """Create a new queue.
-
-        When a queue already exists at the given path it will be reused.
-        """
-        db_path = Path(db_path)
-        async with aiosqlite.connect(db_path, isolation_level=None) as db:
-            await db.execute(
-                """
-                CREATE TABLE IF NOT EXISTS queue (item BLOB);
-                """
-            )
-        return cls._create(db_path)
```

### Comparing `aiodiskqueue-0.1.0a2/tests/test_core.py` & `aiodiskqueue-0.1.0a3/tests/test_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,70 +11,65 @@
     def setUp(self) -> None:
         self.temp_dir = Path(tempfile.mkdtemp())
         self.db_path = self.temp_dir / "test_queue.sqlite"
 
     def tearDown(self) -> None:
         shutil.rmtree(self.temp_dir, ignore_errors=True)
 
-    def test_should_not_permit_direct_instantiation(self):
-        # when/then
-        with self.assertRaises(TypeError):
-            Queue(self.db_path)
-
     async def test_should_create_queue_and_measure_size(self):
         # given
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         # when
         result = await q.qsize()
         # then
         self.assertEqual(result, 0)
 
     async def test_should_put_items_and_measure_size(self):
         # given
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         # when
         await q.put("dummy")
         # then
         result = await q.qsize()
         self.assertEqual(result, 1)
 
     async def test_should_get_items(self):
         # given
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         await q.put("dummy")
         # when
         result = await q.get()
         # then
         self.assertEqual(result, "dummy")
 
     async def test_should_handle_complex_items(self):
         # given
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         item = {
             "alpha": ["one", "two", "three"],
             "now": dt.datetime.now(tz=dt.timezone.utc),
         }
         await q.put(item)
         # when
         result = await q.get()
         # then
         self.assertEqual(result, item)
 
     async def test_should_raise_exception_when_get_on_empty_queue(self):
         # given
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         # when/then
         with self.assertRaises(QueueEmpty):
             await q.get()
 
     async def test_should_report_as_empty(self):
         # given
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         # when/then
         self.assertTrue(await q.empty())
 
     async def test_should_not_report_as_empty(self):
         # given
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         await q.put("dummy")
         # when/then
         self.assertFalse(await q.empty())
```

### Comparing `aiodiskqueue-0.1.0a2/PKG-INFO` & `aiodiskqueue-0.1.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Persistent queues for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -40,15 +40,15 @@
 
 .. code:: python
 
    import asyncio
    from aiodiskqueue import Queue
 
    async def main():
-       q = await Queue.create("example_queue.sqlite")
+       q = Queue("example_queue.sqlite")
        await q.put("some item")
        item = await q.get()
        print(item)
 
    asyncio.run(main())
 
 Please see the examples folder for more usage examples.
```


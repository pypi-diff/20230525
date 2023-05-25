# Comparing `tmp/aiodiskqueue-0.1.0a1.tar.gz` & `tmp/aiodiskqueue-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.0a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0a1.tar` & `aiodiskqueue-0.1.0a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a1/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a1/.github/workflows/main.yml
--rw-r--r--   0        0        0      107 2023-05-24 14:44:42.314154 aiodiskqueue-0.1.0a1/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a1/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     1743 2023-05-24 16:34:06.356844 aiodiskqueue-0.1.0a1/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a1/docs/Makefile
--rw-r--r--   0        0        0      228 2023-05-24 15:12:23.388951 aiodiskqueue-0.1.0a1/docs/api.rst
--rw-r--r--   0        0        0     1545 2023-05-24 15:28:28.604971 aiodiskqueue-0.1.0a1/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a1/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a1/examples/__init__.py
--rw-r--r--   0        0        0      210 2023-05-24 13:48:28.153169 aiodiskqueue-0.1.0a1/examples/basic_usage.py
--rw-r--r--   0        0        0     1768 2023-05-24 13:48:28.049169 aiodiskqueue-0.1.0a1/examples/consumer_producer_processes.py
--rw-r--r--   0        0        0     1045 2023-05-24 13:48:28.073169 aiodiskqueue-0.1.0a1/examples/multiple_consumers.py
--rw-r--r--   0        0        0      991 2023-05-24 13:48:28.073169 aiodiskqueue-0.1.0a1/examples/single_consumer.py
--rw-r--r--   0        0        0      663 2023-05-24 15:08:11.550346 aiodiskqueue-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      188 2023-05-24 15:27:56.829086 aiodiskqueue-0.1.0a1/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0     2838 2023-05-24 15:47:24.487374 aiodiskqueue-0.1.0a1/src/aiodiskqueue/core.py
--rw-r--r--   0        0        0      212 2023-05-24 13:48:27.949169 aiodiskqueue-0.1.0a1/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0      685 2023-05-24 12:22:48.648480 aiodiskqueue-0.1.0a1/src/aiodiskqueue/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a1/tests/__init__.py
--rw-r--r--   0        0        0     2277 2023-05-24 13:48:28.153169 aiodiskqueue-0.1.0a1/tests/test_core.py
--rw-r--r--   0        0        0      394 2023-05-24 14:12:01.108384 aiodiskqueue-0.1.0a1/tox.ini
--rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a2/.coveragerc
+-rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a2/.github/workflows/main.yml
+-rw-r--r--   0        0        0      107 2023-05-24 14:44:42.314154 aiodiskqueue-0.1.0a2/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     2098 2023-05-24 17:01:45.615031 aiodiskqueue-0.1.0a2/README.rst
+-rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a2/docs/Makefile
+-rw-r--r--   0        0        0      228 2023-05-24 15:12:23.388951 aiodiskqueue-0.1.0a2/docs/api.rst
+-rw-r--r--   0        0        0     1545 2023-05-24 15:28:28.604971 aiodiskqueue-0.1.0a2/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a2/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a2/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a2/examples/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-24 13:48:28.153169 aiodiskqueue-0.1.0a2/examples/basic_usage.py
+-rw-r--r--   0        0        0     1768 2023-05-24 13:48:28.049169 aiodiskqueue-0.1.0a2/examples/consumer_producer_processes.py
+-rw-r--r--   0        0        0     1045 2023-05-24 13:48:28.073169 aiodiskqueue-0.1.0a2/examples/multiple_consumers.py
+-rw-r--r--   0        0        0      991 2023-05-24 13:48:28.073169 aiodiskqueue-0.1.0a2/examples/single_consumer.py
+-rw-r--r--   0        0        0      911 2023-05-24 17:01:20.419148 aiodiskqueue-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-05-24 16:56:21.656687 aiodiskqueue-0.1.0a2/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0     2838 2023-05-24 15:47:24.487374 aiodiskqueue-0.1.0a2/src/aiodiskqueue/core.py
+-rw-r--r--   0        0        0      212 2023-05-24 13:48:27.949169 aiodiskqueue-0.1.0a2/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0      685 2023-05-24 12:22:48.648480 aiodiskqueue-0.1.0a2/src/aiodiskqueue/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a2/tests/__init__.py
+-rw-r--r--   0        0        0     2277 2023-05-24 13:48:28.153169 aiodiskqueue-0.1.0a2/tests/test_core.py
+-rw-r--r--   0        0        0      394 2023-05-24 14:12:01.108384 aiodiskqueue-0.1.0a2/tox.ini
+-rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a2/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0a1/.github/workflows/main.yml` & `aiodiskqueue-0.1.0a2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a1/LICENSE` & `aiodiskqueue-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a1/docs/Makefile` & `aiodiskqueue-0.1.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a1/docs/conf.py` & `aiodiskqueue-0.1.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a1/docs/make.bat` & `aiodiskqueue-0.1.0a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a1/examples/consumer_producer_processes.py` & `aiodiskqueue-0.1.0a2/examples/consumer_producer_processes.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a1/examples/multiple_consumers.py` & `aiodiskqueue-0.1.0a2/examples/multiple_consumers.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a1/examples/single_consumer.py` & `aiodiskqueue-0.1.0a2/examples/single_consumer.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a1/src/aiodiskqueue/core.py` & `aiodiskqueue-0.1.0a2/src/aiodiskqueue/core.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a1/src/aiodiskqueue/utils.py` & `aiodiskqueue-0.1.0a2/src/aiodiskqueue/utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a1/tests/test_core.py` & `aiodiskqueue-0.1.0a2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a1/PKG-INFO` & `aiodiskqueue-0.1.0a2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,73 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Persistent queues for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiosqlite
+Requires-Dist: aiosqlite>=0.19.0
+Project-URL: Documentation, https://aiodiskqueue.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/ErikKalkoken/aiodiskqueue
+Project-URL: Tracker, https://github.com/ErikKalkoken/aiodiskqueue/issues
 
 aiodiskqueue
 ============
 
 Persistent queues for Python AsyncIO.
 
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
 
 Description
 -----------
 
-This library for Python AsyncIO provides queues, which persist their content on disk. Their main advantage is that they their content will survive a normal process restart and potentially even a process crash.
+This library provides a persistent queue for Python AsyncIO.
+
+It's main advantage is that it's content will survive a normal process restart and potentially even a process crash.
+
+Each queue is stored in it's own SQLite database on disk to provide maximum isolation between queues. Using SQLite should also make the queue inherently process safe [needs confirmation].
 
 Usage
 -----
 
-Here is a basic example on how to use the queue
+Here is a basic example on how to use the queue:
 
 .. code:: python
 
    import asyncio
    from aiodiskqueue import Queue
 
    async def main():
        q = await Queue.create("example_queue.sqlite")
        await q.put("some item")
        item = await q.get()
        print(item)
 
    asyncio.run(main())
 
+Please see the examples folder for more usage examples.
+
+Installation
+------------
+
+You can install directly from PyPI with the following command:
+
+.. code:: shell
+
+   pip install aiodiskqueue
+
+
+
 .. |release| image:: https://img.shields.io/pypi/v/aiodiskqueue?label=release
    :target: https://pypi.org/project/aiodiskqueue/
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodiskqueue
    :target: https://pypi.org/project/aiodiskqueue/
 .. |tests| image:: https://github.com/ErikKalkoken/aiodiskqueue/actions/workflows/main.yml/badge.svg
    :target: https://github.com/ErikKalkoken/aiodiskqueue/actions
 .. |codecov| image:: https://codecov.io/gh/ErikKalkoken/aiodiskqueue/branch/main/graph/badge.svg?token=V43h7hl1Te
```


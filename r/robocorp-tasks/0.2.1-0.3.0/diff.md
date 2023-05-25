# Comparing `tmp/robocorp_tasks-0.2.1.tar.gz` & `tmp/robocorp_tasks-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-0.2.1.tar", max compression
+gzip compressed data, was "robocorp_tasks-0.3.0.tar", max compression
```

## Comparing `robocorp_tasks-0.2.1.tar` & `robocorp_tasks-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     4922 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/README.md
--rw-r--r--   0        0        0     1134 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3502 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     4495 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1457 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     5120 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0     7689 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0     2245 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_config.py
--rw-r--r--   0        0        0      182 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0     1123 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     1367 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_lifecycle.py
--rw-r--r--   0        0        0     5267 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0      461 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     3738 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0     5487 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0      870 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0        0 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/py.typed
--rw-r--r--   0        0        0     5666 1970-01-01 00:00:00.000000 robocorp_tasks-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4922 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/README.md
+-rw-r--r--   0        0        0     1134 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3502 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     4495 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1457 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5120 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0     7935 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      182 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     1123 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     1367 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     5267 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0      461 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     3738 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0     5487 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0      870 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0        0 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/py.typed
+-rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 robocorp_tasks-0.3.0/PKG-INFO
```

### Comparing `robocorp_tasks-0.2.1/README.md` & `robocorp_tasks-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.1/pyproject.toml` & `robocorp_tasks-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "0.2.1"
+version = "0.3.0"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/tasks", from = "src"}]
 classifiers = [
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-log = "0.1.1"
+robocorp-log = "0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [tool.mypy]
 mypy_path = "src:tests"
```

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/__init__.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 automatically logged is not imported prior the the `cli.main` call.
 """
 from pathlib import Path
 from typing import Optional
 from ._protocols import ITask
 
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def task(func):
     """
     Decorator for tasks (entry points) which can be executed by `robocorp.tasks`.
```

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/_argdispatch.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/_callback.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/_commands.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,18 +133,22 @@
         return 1
 
     from robocorp import log
 
     task_names: Sequence[str]
     if not task_name:
         task_names = []
+        task_or_tasks = "tasks"
     elif isinstance(task_name, str):
         task_names = [task_name]
+        task_or_tasks = "task"
     else:
         task_names = task_name
+        task_name = ", ".join(str(x) for x in task_names)
+        task_or_tasks = "task" if len(task_names) == 1 else "tasks"
 
     config: log.BaseConfig
     pyproject_path_and_contents = read_pyproject_toml(context, p)
     pyproject_toml_contents: dict
     if not pyproject_path_and_contents:
         config = log.ConfigFilesFiltering()
         pyproject_toml_contents = {}
@@ -186,15 +190,17 @@
 
         try:
             log.start_task("Collect tasks", "setup", "", 0)
             try:
                 if not task_name:
                     context.show(f"\nCollecting tasks from: {path}")
                 else:
-                    context.show(f"\nCollecting task {task_name} from: {path}")
+                    context.show(
+                        f"\nCollecting {task_or_tasks} {task_name} from: {path}"
+                    )
 
                 tasks: List[ITask] = list(collect_tasks(p, task_names))
 
                 if not tasks:
                     raise RobocorpTasksCollectError(
                         f"Did not find any tasks in: {path}"
                     )
```

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/_config.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/_lifecycle.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/_task.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.1/src/robocorp/tasks/cli.py` & `robocorp_tasks-0.3.0/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.1/PKG-INFO` & `robocorp_tasks-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 0.2.1
+Version: 0.3.0
 Summary: The automation framework for Python
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Dist: robocorp-log (==0.1.1)
+Requires-Dist: robocorp-log (==0.2.0)
 Description-Content-Type: text/markdown
 
 # robocorp-tasks
 
 `robocorp-tasks` is a Python framework designed to simplify the development 
 of Python automations.
```


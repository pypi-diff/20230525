# Comparing `tmp/spectacles-2.3.8.tar.gz` & `tmp/spectacles-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectacles-2.3.8.tar", last modified: Fri Jan  6 16:07:32 2023, max compression
+gzip compressed data, was "spectacles-2.3.9.tar", last modified: Wed Apr 19 13:45:20 2023, max compression
```

## Comparing `spectacles-2.3.8.tar` & `spectacles-2.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-01-06 16:07:32.532965 spectacles-2.3.8/
--rw-r--r--   0 dylan      (501) staff       (20)     1082 2019-10-02 19:47:43.000000 spectacles-2.3.8/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)     3603 2023-01-06 16:07:32.533119 spectacles-2.3.8/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     3192 2022-11-21 17:52:41.000000 spectacles-2.3.8/README.md
--rw-r--r--   0 dylan      (501) staff       (20)      488 2023-01-06 16:07:32.533574 spectacles-2.3.8/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)     1538 2022-12-05 12:33:42.000000 spectacles-2.3.8/setup.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-01-06 16:07:32.530080 spectacles-2.3.8/spectacles/
--rw-r--r--   0 dylan      (501) staff       (20)       22 2023-01-06 16:07:14.000000 spectacles-2.3.8/spectacles/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)    32426 2022-11-21 17:52:41.000000 spectacles-2.3.8/spectacles/cli.py
--rw-r--r--   0 dylan      (501) staff       (20)    37589 2022-12-05 12:33:42.000000 spectacles-2.3.8/spectacles/client.py
--rw-r--r--   0 dylan      (501) staff       (20)     5658 2022-08-26 11:43:56.000000 spectacles-2.3.8/spectacles/exceptions.py
--rw-r--r--   0 dylan      (501) staff       (20)     3566 2022-11-21 17:52:41.000000 spectacles-2.3.8/spectacles/logger.py
--rw-r--r--   0 dylan      (501) staff       (20)    17173 2022-12-21 15:57:20.000000 spectacles-2.3.8/spectacles/lookml.py
--rw-r--r--   0 dylan      (501) staff       (20)     5145 2022-11-21 17:52:41.000000 spectacles-2.3.8/spectacles/printer.py
--rw-r--r--   0 dylan      (501) staff       (20)        0 2022-08-26 11:43:56.000000 spectacles-2.3.8/spectacles/py.typed
--rw-r--r--   0 dylan      (501) staff       (20)    22666 2023-01-06 16:07:14.000000 spectacles-2.3.8/spectacles/runner.py
--rw-r--r--   0 dylan      (501) staff       (20)     1458 2022-04-12 12:30:09.000000 spectacles-2.3.8/spectacles/select.py
--rw-r--r--   0 dylan      (501) staff       (20)     1277 2021-03-23 17:37:58.000000 spectacles-2.3.8/spectacles/tracking.py
--rw-r--r--   0 dylan      (501) staff       (20)     2559 2022-11-21 17:52:41.000000 spectacles-2.3.8/spectacles/types.py
--rw-r--r--   0 dylan      (501) staff       (20)     3156 2022-11-21 17:52:41.000000 spectacles-2.3.8/spectacles/utils.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-01-06 16:07:32.532617 spectacles-2.3.8/spectacles/validators/
--rw-r--r--   0 dylan      (501) staff       (20)      317 2022-01-14 11:56:20.000000 spectacles-2.3.8/spectacles/validators/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     7257 2022-11-21 17:52:41.000000 spectacles-2.3.8/spectacles/validators/content.py
--rw-r--r--   0 dylan      (501) staff       (20)     4842 2023-01-03 17:08:06.000000 spectacles-2.3.8/spectacles/validators/data_test.py
--rw-r--r--   0 dylan      (501) staff       (20)     2289 2022-08-26 11:43:56.000000 spectacles-2.3.8/spectacles/validators/lookml.py
--rw-r--r--   0 dylan      (501) staff       (20)    18385 2022-12-05 12:33:42.000000 spectacles-2.3.8/spectacles/validators/sql.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-01-06 16:07:32.531494 spectacles-2.3.8/spectacles.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     3603 2023-01-06 16:07:32.000000 spectacles-2.3.8/spectacles.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      681 2023-01-06 16:07:32.000000 spectacles-2.3.8/spectacles.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-01-06 16:07:32.000000 spectacles-2.3.8/spectacles.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       52 2023-01-06 16:07:32.000000 spectacles-2.3.8/spectacles.egg-info/entry_points.txt
--rw-r--r--   0 dylan      (501) staff       (20)       99 2023-01-06 16:07:32.000000 spectacles-2.3.8/spectacles.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       11 2023-01-06 16:07:32.000000 spectacles-2.3.8/spectacles.egg-info/top_level.txt
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-19 13:45:20.086694 spectacles-2.3.9/
+-rw-r--r--   0 josh       (501) staff       (20)     1082 2021-11-18 20:00:49.000000 spectacles-2.3.9/LICENSE
+-rw-r--r--   0 josh       (501) staff       (20)     3566 2023-04-19 13:45:20.086824 spectacles-2.3.9/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     3192 2022-11-08 19:17:18.000000 spectacles-2.3.9/README.md
+-rw-r--r--   0 josh       (501) staff       (20)      488 2023-04-19 13:45:20.087241 spectacles-2.3.9/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)     1538 2022-11-22 19:57:14.000000 spectacles-2.3.9/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-19 13:45:20.078953 spectacles-2.3.9/spectacles/
+-rw-r--r--   0 josh       (501) staff       (20)       22 2023-04-19 13:38:00.000000 spectacles-2.3.9/spectacles/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    32426 2023-04-13 14:22:32.000000 spectacles-2.3.9/spectacles/cli.py
+-rw-r--r--   0 josh       (501) staff       (20)    37605 2023-04-18 18:35:36.000000 spectacles-2.3.9/spectacles/client.py
+-rw-r--r--   0 josh       (501) staff       (20)     5658 2022-11-08 19:17:18.000000 spectacles-2.3.9/spectacles/exceptions.py
+-rw-r--r--   0 josh       (501) staff       (20)     3566 2022-11-21 18:46:43.000000 spectacles-2.3.9/spectacles/logger.py
+-rw-r--r--   0 josh       (501) staff       (20)    17173 2022-11-08 19:17:18.000000 spectacles-2.3.9/spectacles/lookml.py
+-rw-r--r--   0 josh       (501) staff       (20)     5145 2022-11-08 19:17:18.000000 spectacles-2.3.9/spectacles/printer.py
+-rw-r--r--   0 josh       (501) staff       (20)        0 2022-11-08 19:17:18.000000 spectacles-2.3.9/spectacles/py.typed
+-rw-r--r--   0 josh       (501) staff       (20)    22612 2023-04-19 13:37:45.000000 spectacles-2.3.9/spectacles/runner.py
+-rw-r--r--   0 josh       (501) staff       (20)     1458 2022-05-06 16:38:15.000000 spectacles-2.3.9/spectacles/select.py
+-rw-r--r--   0 josh       (501) staff       (20)     1277 2021-11-18 20:00:49.000000 spectacles-2.3.9/spectacles/tracking.py
+-rw-r--r--   0 josh       (501) staff       (20)     2559 2022-11-08 19:17:18.000000 spectacles-2.3.9/spectacles/types.py
+-rw-r--r--   0 josh       (501) staff       (20)     3156 2022-11-08 19:17:18.000000 spectacles-2.3.9/spectacles/utils.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-19 13:45:20.085179 spectacles-2.3.9/spectacles/validators/
+-rw-r--r--   0 josh       (501) staff       (20)      317 2022-05-06 16:38:15.000000 spectacles-2.3.9/spectacles/validators/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     7257 2022-11-17 17:52:02.000000 spectacles-2.3.9/spectacles/validators/content.py
+-rw-r--r--   0 josh       (501) staff       (20)     4842 2023-01-05 15:39:19.000000 spectacles-2.3.9/spectacles/validators/data_test.py
+-rw-r--r--   0 josh       (501) staff       (20)     2289 2023-04-18 18:35:33.000000 spectacles-2.3.9/spectacles/validators/lookml.py
+-rw-r--r--   0 josh       (501) staff       (20)    18617 2023-04-19 13:37:45.000000 spectacles-2.3.9/spectacles/validators/sql.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-04-19 13:45:20.081316 spectacles-2.3.9/spectacles.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)     3566 2023-04-19 13:45:20.000000 spectacles-2.3.9/spectacles.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      681 2023-04-19 13:45:20.000000 spectacles-2.3.9/spectacles.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-04-19 13:45:20.000000 spectacles-2.3.9/spectacles.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)       51 2023-04-19 13:45:20.000000 spectacles-2.3.9/spectacles.egg-info/entry_points.txt
+-rw-r--r--   0 josh       (501) staff       (20)       99 2023-04-19 13:45:20.000000 spectacles-2.3.9/spectacles.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       11 2023-04-19 13:45:20.000000 spectacles-2.3.9/spectacles.egg-info/top_level.txt
```

### Comparing `spectacles-2.3.8/LICENSE` & `spectacles-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/PKG-INFO` & `spectacles-2.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: spectacles
-Version: 2.3.8
+Version: 2.3.9
 Summary: A command-line, continuous integration tool for Looker and LookML.
 Home-page: https://github.com/spectacles-ci/spectacles
-Download-URL: https://github.com/spectacles-ci/spectacles/tarball/2.3.8
+Download-URL: https://github.com/spectacles-ci/spectacles/tarball/2.3.9
 Author: Spectacles
 Author-email: hello@spectacles.dev
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://github.com/spectacles-ci/spectacles/raw/master/docs/img/logo.png" width="600">
 
 [![CircleCI](https://circleci.com/gh/spectacles-ci/spectacles.svg?style=svg)](https://circleci.com/gh/spectacles-ci/spectacles)
 [![downloads](https://img.shields.io/pypi/dm/spectacles)](https://img.shields.io/pypi/dm/spectacles)
@@ -56,9 +54,7 @@
 **We believe in the power of testing and continuous integration for analytics.** We believe that automated tests should catch these errors before they're ever pushed to production.
 
 We wanted a single tool to perform these checks for us, so we built Spectacles to enhance the business intelligence layer of analytics CI pipelines.
 
 ## Community
 
 Have a question or just want to chat Spectacles or Looker? [Join us in Slack.](https://join.slack.com/t/spectacles-ci/shared_invite/zt-akmm4mo6-XnPcUUaG3Z5~giRc_5JaUQ)
-
-
```

### Comparing `spectacles-2.3.8/README.md` & `spectacles-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/setup.py` & `spectacles-2.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/cli.py` & `spectacles-2.3.9/spectacles/cli.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/client.py` & `spectacles-2.3.9/spectacles/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,16 +382,16 @@
         except httpx.HTTPStatusError as error:
             raise LookerApiError(
                 name="unable-to-get-active-branch",
                 title="Couldn't determine active Git branch.",
                 status=response.status_code,
                 detail=(
                     f"Unable to get active branch for project '{project}'. "
-                    "Please check that the project exists and that your user "
-                    "has the correct permissions and try again."
+                    "Please check that the project exists, is configured, "
+                    "and that your user has the correct permissions and try again."
                 ),
                 response=response,
             ) from error
 
         branch_name = response.json()["name"]
         logger.debug(f"The active branch is '{branch_name}'")
```

### Comparing `spectacles-2.3.8/spectacles/exceptions.py` & `spectacles-2.3.9/spectacles/exceptions.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/logger.py` & `spectacles-2.3.9/spectacles/logger.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/lookml.py` & `spectacles-2.3.9/spectacles/lookml.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/printer.py` & `spectacles-2.3.9/spectacles/printer.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/runner.py` & `spectacles-2.3.9/spectacles/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,17 +395,15 @@
             f"Testing {explore_count} "
             f"{'explore' if explore_count == 1 else 'explores'} "
             + ("[fail fast] " if fail_fast else "")
             + f"[concurrency = {concurrency}]"
         )
 
         async with self.branch_manager(ref=ref):
-            await validator.search(
-                explores, fail_fast, chunk_size, profile=profile if fail_fast else False
-            )
+            await validator.search(explores, fail_fast, chunk_size, profile=profile)
 
         # Create dimension tests for the desired ref when explores errored
         if not fail_fast and incremental:
             errored_dimensions = project.iter_dimensions(errored=True)
             # For errored dimensions, create dimension tests for the target ref
             async with self.branch_manager(ref=target, ephemeral=True):
                 target_ref = self.branch_manager.ref
```

### Comparing `spectacles-2.3.8/spectacles/select.py` & `spectacles-2.3.9/spectacles/select.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/tracking.py` & `spectacles-2.3.9/spectacles/tracking.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/types.py` & `spectacles-2.3.9/spectacles/types.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/utils.py` & `spectacles-2.3.9/spectacles/utils.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/validators/content.py` & `spectacles-2.3.9/spectacles/validators/content.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/validators/data_test.py` & `spectacles-2.3.9/spectacles/validators/data_test.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/validators/lookml.py` & `spectacles-2.3.9/spectacles/validators/lookml.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.3.8/spectacles/validators/sql.py` & `spectacles-2.3.9/spectacles/validators/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from spectacles.utils import consume_queue, halt_queue
 from spectacles.types import QueryResult, CompletedQueryResult, ErrorQueryResult
 
 QUERY_TASK_LIMIT = 250
 DEFAULT_CHUNK_SIZE = 500
 DEFAULT_QUERY_CONCURRENCY = 10
 DEFAULT_RUNTIME_THRESHOLD = 5
-ProfilerTableRow = Tuple[str, float, str, str]
+ProfilerTableRow = Tuple[str, str, float, str, str]
 
 
 @dataclass
 class Query:
     explore: Explore
     dimensions: tuple[Dimension, ...]
     query_id: str | None = None
@@ -58,15 +58,21 @@
                 "Query.query_id cannot be None, run Query.create to get a query ID"
             )
         if self.explore_url is None:
             raise TypeError(
                 "Query.explore_url cannot be None, "
                 "run Query.create to get an explore URL"
             )
-        return (self.explore.name, self.runtime, self.query_id, self.explore_url)
+        return (
+            self.explore.name,
+            self.dimensions[0].name if len(self.dimensions) == 1 else "*",
+            self.runtime,
+            self.query_id,
+            self.explore_url,
+        )
 
 
 def print_profile_results(queries: List[Query], runtime_threshold: int) -> None:
     """Defined here instead of in .printer to avoid circular type imports."""
     HEADER_CHAR = "."
     print_header("Query profiler results", char=HEADER_CHAR, leading_newline=False)
     if queries:
@@ -75,14 +81,15 @@
             key=lambda x: x.runtime if x.runtime is not None else -1,
             reverse=True,
         )
         output = tabulate(
             [query.to_profiler_format() for query in queries_by_runtime],
             headers=[
                 "Explore",
+                "Dimension(s)",
                 "Runtime (s)",
                 "Query ID",
                 "Explore From Here",
             ],
             tablefmt="github",
             numalign="left",
             floatfmt=".1f",
@@ -311,14 +318,15 @@
 
                     # Append long-running queries for the profiler
                     if query_result.status in ("complete", "error"):
                         query_result = cast(
                             Union[CompletedQueryResult, ErrorQueryResult], query_result
                         )
                         query = self._task_to_query[task_id]
+                        query.runtime = query_result.runtime
                         if query_result.runtime > self.runtime_threshold:
                             self._long_running_queries.append(query)
                         if query_result.status == "complete":
                             query_slot.release()
                             query.errored = False
                             query.explore.queried = True
                             queries_to_run.task_done()
```

### Comparing `spectacles-2.3.8/spectacles.egg-info/PKG-INFO` & `spectacles-2.3.9/spectacles.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: spectacles
-Version: 2.3.8
+Version: 2.3.9
 Summary: A command-line, continuous integration tool for Looker and LookML.
 Home-page: https://github.com/spectacles-ci/spectacles
-Download-URL: https://github.com/spectacles-ci/spectacles/tarball/2.3.8
+Download-URL: https://github.com/spectacles-ci/spectacles/tarball/2.3.9
 Author: Spectacles
 Author-email: hello@spectacles.dev
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://github.com/spectacles-ci/spectacles/raw/master/docs/img/logo.png" width="600">
 
 [![CircleCI](https://circleci.com/gh/spectacles-ci/spectacles.svg?style=svg)](https://circleci.com/gh/spectacles-ci/spectacles)
 [![downloads](https://img.shields.io/pypi/dm/spectacles)](https://img.shields.io/pypi/dm/spectacles)
@@ -56,9 +54,7 @@
 **We believe in the power of testing and continuous integration for analytics.** We believe that automated tests should catch these errors before they're ever pushed to production.
 
 We wanted a single tool to perform these checks for us, so we built Spectacles to enhance the business intelligence layer of analytics CI pipelines.
 
 ## Community
 
 Have a question or just want to chat Spectacles or Looker? [Join us in Slack.](https://join.slack.com/t/spectacles-ci/shared_invite/zt-akmm4mo6-XnPcUUaG3Z5~giRc_5JaUQ)
-
-
```

### Comparing `spectacles-2.3.8/spectacles.egg-info/SOURCES.txt` & `spectacles-2.3.9/spectacles.egg-info/SOURCES.txt`

 * *Files identical despite different names*


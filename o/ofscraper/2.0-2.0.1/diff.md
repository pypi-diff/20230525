# Comparing `tmp/ofscraper-2.0.tar.gz` & `tmp/ofscraper-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.0.tar", max compression
+gzip compressed data, was "ofscraper-2.0.1.tar", max compression
```

## Comparing `ofscraper-2.0.tar` & `ofscraper-2.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1067 2023-05-25 19:57:24.283919 ofscraper-2.0/LICENSE
--rw-r--r--   0        0        0     5192 2023-05-25 19:57:24.283919 ofscraper-2.0/README.md
--rw-r--r--   0        0        0      607 2023-05-25 19:57:25.163928 ofscraper-2.0/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-05-25 19:57:25.163928 ofscraper-2.0/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-05-25 19:57:25.163928 ofscraper-2.0/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     1986 2023-05-25 19:57:25.163928 ofscraper-2.0/ofscraper/api/highlights.py
--rw-r--r--   0        0        0      838 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/init.py
--rw-r--r--   0        0        0     2243 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/me.py
--rw-r--r--   0        0        0     5671 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/messages.py
--rw-r--r--   0        0        0     1884 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/paid.py
--rw-r--r--   0        0        0     9037 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/posts.py
--rw-r--r--   0        0        0     2841 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1867 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     8070 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     4999 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3199 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     3548 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/interaction/like.py
--rw-r--r--   0        0        0     5477 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    20976 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/prompts/prompts.py
--rwxr-xr-x   0        0        0    23572 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/scraper.py
--rw-r--r--   0        0        0        1 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     4320 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8996 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/auth.py
--rw-r--r--   0        0        0    10859 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    17889 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2938 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     2381 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     4408 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     5220 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3008 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     1526 2023-05-25 19:58:01.928343 ofscraper-2.0/pyproject.toml
--rw-r--r--   0        0        0     6593 1970-01-01 00:00:00.000000 ofscraper-2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-25 21:03:02.597295 ofscraper-2.0.1/LICENSE
+-rw-r--r--   0        0        0     5192 2023-05-25 21:03:02.601295 ofscraper-2.0.1/README.md
+-rw-r--r--   0        0        0      607 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     1986 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2243 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/me.py
+-rw-r--r--   0        0        0     5671 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     1884 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     9037 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     2841 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1867 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     8069 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     4999 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4053 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0     5477 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    20976 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/prompts/prompts.py
+-rwxr-xr-x   0        0        0    23572 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/scraper.py
+-rw-r--r--   0        0        0        1 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     4320 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     8996 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0    10859 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    17889 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2938 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     2381 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     4408 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     5220 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3008 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     1528 2023-05-25 21:03:36.441192 ofscraper-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6595 1970-01-01 00:00:00.000000 ofscraper-2.0.1/PKG-INFO
```

### Comparing `ofscraper-2.0/LICENSE` & `ofscraper-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/README.md` & `ofscraper-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/__init__.py` & `ofscraper-2.0.1/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/__version__.py` & `ofscraper-2.0.1/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/api/highlights.py` & `ofscraper-2.0.1/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/api/init.py` & `ofscraper-2.0.1/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/api/me.py` & `ofscraper-2.0.1/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/api/messages.py` & `ofscraper-2.0.1/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/api/paid.py` & `ofscraper-2.0.1/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/api/posts.py` & `ofscraper-2.0.1/ofscraper/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/api/profile.py` & `ofscraper-2.0.1/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/api/subscriptions.py` & `ofscraper-2.0.1/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/api/timeline.py` & `ofscraper-2.0.1/ofscraper/api/timeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             log.debug(f"[bold]timeline request status code:[/bold]{r.status_code}")
             log.debug(f"[bold]timeline response:[/bold] {r.content.decode()}")
             r.raise_for_status()
 
 async def get_timeline_post(headers,model_id):
     global sem
     sem = asyncio.Semaphore(8)
-    overall_progress=Progress(SpinnerColumn(style=Style(color="blue"),),TextColumn("Getting timeline media...\n{task.description}"))
+    overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting timeline media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
     with Live(progress_group, refresh_per_second=10,console=console.shared_console): 
 
         oldtimeline=cache.get(f"timeline_{model_id}",default=[])
```

### Comparing `ofscraper-2.0/ofscraper/constants.py` & `ofscraper-2.0.1/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/db/operations.py` & `ofscraper-2.0.1/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/db/queries.py` & `ofscraper-2.0.1/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/interaction/like.py` & `ofscraper-2.0.1/ofscraper/interaction/like.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,31 @@
 
 import random
 import time
 import logging
 from typing import Union
 import asyncio
 import httpx
-from rich.console import Console
-console=Console()
+
 from halo import Halo
+log=logging.getLogger(__package__)
+
+from rich.progress import Progress
+from rich.progress import (
+    Progress,
+    MofNCompleteColumn,
+    BarColumn,
+    TextColumn,
+    SpinnerColumn
+)
+from rich.style import Style
 from ..api import timeline
 from ..constants import favoriteEP, postURL
 from ..utils import auth
-
-log=logging.getLogger(__package__)
-
+import ofscraper.utils.console as console
 
 
 
 def get_posts(headers, model_id):
     pinned_posts = timeline.scrape_pinned_posts(headers, model_id)
     timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
     archived_posts = timeline.scrape_archived_posts(headers, model_id)
@@ -61,15 +69,16 @@
 
 def unlike(headers, model_id, username, ids: list):
     _like(headers, model_id, username, ids, False)
 
 
 def _like(headers, model_id, username, ids: list, like_action: bool):
     title = "Liking" if like_action else "Unliking"
-    with Halo(text=f'{title} posts...'):
+    with Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}"),BarColumn(),MofNCompleteColumn(),console=console.shared_console) as overall_progress:
+        task1=overall_progress.add_task(f"{title} posts...\n",total=len(ids))
         for i in ids:
             with httpx.Client(http2=True, headers=headers) as c:
                 url = favoriteEP.format(i, model_id)
 
                 auth.add_cookies(c)
                 c.headers.update(auth.create_sign(url, headers))
 
@@ -77,21 +86,21 @@
                 while retries <= 1:
                     time.sleep(random.uniform(0.8, 0.9))
                     retries += 1
                     try:
                         r = c.post(url)
                         if not r.is_error or r.status_code == 400:
                             log.debug(f"ID: {i} Performed {'like' if like_action==True else 'unlike'} action")
+                            overall_progress.update(task1,advance=1,refresh=True)
                             break
                         else:
                             _handle_err(r, postURL.format(i, username))
                     except httpx.TransportError as e:
                         _handle_err(e, postURL.format(i, username))
-      
-
+        overall_progress.remove_task(task1)
 
 def _handle_err(param: Union[httpx.Response, httpx.TransportError], url: str) -> str:
     message = 'unable to execute action'
     status = ''
     try:
         if isinstance(param, httpx.Response):
             json = param.json()
```

### Comparing `ofscraper-2.0/ofscraper/prompts/prompt_functions.py` & `ofscraper-2.0.1/ofscraper/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/prompts/prompts.py` & `ofscraper-2.0.1/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/scraper.py` & `ofscraper-2.0.1/ofscraper/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/args.py` & `ofscraper-2.0.1/ofscraper/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/auth.py` & `ofscraper-2.0.1/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/config.py` & `ofscraper-2.0.1/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/dates.py` & `ofscraper-2.0.1/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/download.py` & `ofscraper-2.0.1/ofscraper/utils/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/encoding.py` & `ofscraper-2.0.1/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/exit.py` & `ofscraper-2.0.1/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/filters.py` & `ofscraper-2.0.1/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/logger.py` & `ofscraper-2.0.1/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/paths.py` & `ofscraper-2.0.1/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/profiles.py` & `ofscraper-2.0.1/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/ofscraper/utils/separate.py` & `ofscraper-2.0.1/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0/pyproject.toml` & `ofscraper-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.0"
+version = "2.0.1"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 packages = [{include = "ofscraper"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
```

### Comparing `ofscraper-2.0/PKG-INFO` & `ofscraper-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.0
+Version: 2.0.1
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


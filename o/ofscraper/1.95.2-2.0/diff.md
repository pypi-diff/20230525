# Comparing `tmp/ofscraper-1.95.2.tar.gz` & `tmp/ofscraper-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.95.2.tar", max compression
+gzip compressed data, was "ofscraper-2.0.tar", max compression
```

## Comparing `ofscraper-1.95.2.tar` & `ofscraper-2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1067 2023-05-24 13:48:31.755754 ofscraper-1.95.2/LICENSE
--rw-r--r--   0        0        0     5192 2023-05-24 13:48:31.755754 ofscraper-1.95.2/README.md
--rw-r--r--   0        0        0      607 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     1986 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/highlights.py
--rw-r--r--   0        0        0      838 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/init.py
--rw-r--r--   0        0        0     2243 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/me.py
--rw-r--r--   0        0        0     4359 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/messages.py
--rw-r--r--   0        0        0     1884 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/paid.py
--rw-r--r--   0        0        0     9170 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/posts.py
--rw-r--r--   0        0        0     2841 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1867 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     6457 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     4999 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3199 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     3611 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/interaction/like.py
--rw-r--r--   0        0        0     5477 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    20976 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/prompts/prompts.py
--rwxr-xr-x   0        0        0    21369 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/scraper.py
--rw-r--r--   0        0        0        1 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3938 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8996 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/auth.py
--rw-r--r--   0        0        0    10859 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/config.py
--rw-r--r--   0        0        0      993 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    17597 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2938 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     1926 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     4540 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     5377 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3008 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-05-24 13:48:32.731812 ofscraper-1.95.2/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     1546 2023-05-24 13:49:24.333831 ofscraper-1.95.2/pyproject.toml
--rw-r--r--   0        0        0     6634 1970-01-01 00:00:00.000000 ofscraper-1.95.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-25 19:57:24.283919 ofscraper-2.0/LICENSE
+-rw-r--r--   0        0        0     5192 2023-05-25 19:57:24.283919 ofscraper-2.0/README.md
+-rw-r--r--   0        0        0      607 2023-05-25 19:57:25.163928 ofscraper-2.0/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-05-25 19:57:25.163928 ofscraper-2.0/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-05-25 19:57:25.163928 ofscraper-2.0/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     1986 2023-05-25 19:57:25.163928 ofscraper-2.0/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2243 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/me.py
+-rw-r--r--   0        0        0     5671 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     1884 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     9037 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     2841 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1867 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     8070 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     4999 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     3548 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0     5477 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    20976 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/prompts/prompts.py
+-rwxr-xr-x   0        0        0    23572 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/scraper.py
+-rw-r--r--   0        0        0        1 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     4320 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     8996 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0    10859 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    17889 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2938 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     2381 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     4408 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     5220 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3008 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-05-25 19:57:25.167929 ofscraper-2.0/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     1526 2023-05-25 19:58:01.928343 ofscraper-2.0/pyproject.toml
+-rw-r--r--   0        0        0     6593 1970-01-01 00:00:00.000000 ofscraper-2.0/PKG-INFO
```

### Comparing `ofscraper-1.95.2/LICENSE` & `ofscraper-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/README.md` & `ofscraper-2.0/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/__init__.py` & `ofscraper-2.0/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/__version__.py` & `ofscraper-2.0/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/api/highlights.py` & `ofscraper-2.0/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/api/init.py` & `ofscraper-2.0/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/api/me.py` & `ofscraper-2.0/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/api/paid.py` & `ofscraper-2.0/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/api/posts.py` & `ofscraper-2.0/ofscraper/api/posts.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,45 +229,47 @@
             return None
 
 
 
     @property
     def text_(self):
         text = self.text
+        if len(text)==0:
+            return text
         # this is for removing emojis
         # text=re.sub("[^\x00-\x7F]","",text)
         # this is for removing html tags
         text = re.sub("<[^>]*>", "", text)
         # this for remove random special invalid special characters
         text = re.sub('[\n<>:"/\|?*]+', '', text)
         text = re.sub(" +", " ", text)
         length = int(config.get_textlength(config.read_config()))
-        if args_.getargs().letter_count:
-            if length==0 and self._addcount():
+        if length==0 and self._addcount():
                 return f"{text}_{self.count}"
-            elif length==0 and not self._addcount():
+        elif length==0 and not self._addcount():
                 return text
-            elif length!=0 and not self._addcount():
+ 
+        elif args_.getargs().letter_count:
+            if not self._addcount():
                 return "".join(list(text))[:length]
-            elif length!=0 and self._addcount():
+            elif self._addcount():
                 append=f"_{self.count}"
-                return f"{''.join(list(text)[:length-len(append)])}{append}"
-                
-        if not args_.getargs().letter_count:
-            if length==0 and self._addcount():
-                return f"{text}_{self.count}"
-            elif length==0 and not self._addcount():
-                return text
-            elif length!=0 and not self._addcount():
-                return "".join(list(filter(lambda x:len(x)!=0,re.split("( )", text)))[:length])
-            elif length!=0 and self._addcount():
+                baselength=length-len(append)
+                return f"{''.join(list(text)[:baselength])}{append}"         
+        elif not args_.getargs().letter_count :
+            # split and reduce
+            wordarray=list(filter(lambda x:len(x)!=0,re.split("( )", text)))
+            if not self._addcount():
+                return "".join(wordarray[:length])
+            elif self._addcount():
                 append=f"_{self.count}"
-                splitArray=list(filter(lambda x:len(x)!=0,re.split("( )", text)))[:length]
-                splitArray[-1]=re.sub(" ","",f"{splitArray[-1]}{append}")
-                return "".join(splitArray)
+                baselength=length-1
+                splitArray=wordarray[:baselength]
+                text=f"{''.join(splitArray)}{append}"
+                return text
```

### Comparing `ofscraper-1.95.2/ofscraper/api/profile.py` & `ofscraper-2.0/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/api/subscriptions.py` & `ofscraper-2.0/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/api/timeline.py` & `ofscraper-2.0/ofscraper/api/timeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 r"""
                                                              
-        _____                                               
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import time
 import asyncio
 import logging
+import contextvars
+import math
 import httpx
 from tenacity import retry,stop_after_attempt,wait_random
-from tqdm.asyncio import tqdm
+from rich.progress import Progress
+from rich.progress import (
+    Progress,
+    TextColumn,
+    SpinnerColumn
+)
+from rich.panel import Panel
+from rich.console import Group
+from rich.live import Live
+from rich.style import Style
+import arrow
 import ofscraper.constants as constants
 from ..utils import auth
 from ..utils.paths import getcachepath
+import ofscraper.utils.console as console
+
 from diskcache import Cache
 cache = Cache(getcachepath())
 log=logging.getLogger(__package__)
-
-
-
+attempt = contextvars.ContextVar("attempt")
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def scrape_pinned_posts(headers, model_id,timestamp=0) -> list:
     with httpx.Client(http2=True, headers=headers) as c:
         ep = constants.timelinePinnedNextEP if timestamp else constants.timelinePinnedEP
         url = ep.format(model_id, timestamp)
         # url = timelinePinnedEP.format(model_id)
 
@@ -39,95 +50,116 @@
         log.debug(f"[bold]pinned request status code:[/bold]{r.status_code}")
         log.debug(f"[bold]pinned response:[/bold] {r.content.decode()}")
 
 def get_pinned_post(headers,model_id,username):
     return scrape_pinned_posts(headers,model_id)
    
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
-async def scrape_timeline_posts(headers, model_id, timestamp=None,recursive=False) -> list:
-    global sem
-    sem = asyncio.Semaphore(8)
+async def scrape_timeline_posts(headers, model_id,progress, timestamp=None,recursive=False) -> list:
+    global sem 
+    attempt.set(attempt.get(0) + 1)
     if timestamp:
+        log.debug(arrow.get(math.trunc(float(timestamp))))
         timestamp=str(timestamp)
         ep = constants.timelineNextEP
         url = ep.format(model_id, timestamp)
     else:
         ep=constants.timelineEP
         url=ep.format(model_id)
+    log.debug(url)
     async with sem:
+        task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=False if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else True)
+
         async with httpx.AsyncClient(http2=True, headers=headers) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(url, headers))
             r = await c.get(url , timeout=None)
             if not r.is_error:
+                progress.remove_task(task)
                 posts = r.json()['list']
     
                 if not posts:
                     return []
                 elif len(posts)==0:
                     return posts
                 elif not recursive:
                     return posts
                 # recursive search for posts
+                attempt.set(0)
                 global tasks
-                tasks.append(asyncio.create_task( scrape_timeline_posts(headers, model_id,posts[-1]['postedAtPrecise'],recursive=True)))
+                tasks.append(asyncio.create_task( scrape_timeline_posts(headers, model_id,progress,posts[-1]['postedAtPrecise'],recursive=True)))
                 return posts
             log.debug(f"[bold]timeline request status code:[/bold]{r.status_code}")
             log.debug(f"[bold]timeline response:[/bold] {r.content.decode()}")
             r.raise_for_status()
-#max result is 50, try to get 40 in each async task for leeway
-# Also need to grab new posts
+
 async def get_timeline_post(headers,model_id):
-    oldtimeline=cache.get(f"timeline_{model_id}",default=[]) 
-    log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
-    postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldtimeline)))
-    global tasks
-    tasks=[]
-    
-    split=40
-    interval=30
-    if len(postedAtArray)>split:
+    global sem
+    sem = asyncio.Semaphore(8)
+    overall_progress=Progress(SpinnerColumn(style=Style(color="blue"),),TextColumn("Getting timeline media...\n{task.description}"))
+    job_progress=Progress("{task.description}")
+    progress_group = Group(
+    overall_progress,
+    Panel(Group(job_progress)))
+    with Live(progress_group, refresh_per_second=10,console=console.shared_console): 
+
+        oldtimeline=cache.get(f"timeline_{model_id}",default=[]) 
+        oldtimeset=set(map(lambda x:x.get("id"),oldtimeline))
+        log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
+        oldtimeline=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldtimeline))
+        postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldtimeline)))
+        global tasks
+        tasks=[]
+        #max result is 50, try to get 40 in each async task for leeway
+        # Also need to grab new posts
         #add differing splits and interval for inclusivity and potential breakpoints
         split=40
         interval=30
-        splitArrays=[postedAtArray[i:i+split] for i in range(0, len(postedAtArray), interval)]
-        
-        tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id)))
-        tasks.extend(list(map(lambda x:asyncio.create_task(scrape_timeline_posts(headers,model_id,timestamp=x[0]-100)),splitArrays[1:-1])))
-        tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,timestamp=splitArrays[-1][0],recursive=True)))
-    else:
-        tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,recursive=True)))
+        if len(postedAtArray)>split:
+            split=40
+            interval=30
+            splitArrays=[postedAtArray[i:i+split] for i in range(0, len(postedAtArray), interval)]
+            
+            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress)))
+            tasks.extend(list(map(lambda x:asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=x[0]-100)),splitArrays[1:-1])))
+            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=splitArrays[-1][0],recursive=True)))
+        else:
+            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,recursive=True)))
 
-    responseArray=[]
-   
-   
-    page_count=0 
-    desc = 'Pages Progress: {page_count}'   
-
-    with tqdm(desc=desc.format(page_count=page_count), colour='cyan',position=2,disable=True if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else False) as main_bar:
+        responseArray=[]
+    
+    
+        page_count=0 
+        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=False if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else True)
         while len(tasks)!=0:
             for coro in asyncio.as_completed(tasks):
                 result=await coro or []
                 page_count=page_count+1
-                main_bar.set_description(desc.format(page_count=page_count), refresh=False)
-                main_bar.update()
+                overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
                 responseArray.extend(result)
             time.sleep(2)
             tasks=list(filter(lambda x:x.done()==False,tasks))
+        overall_progress.remove_task(page_task)
     unduped=[]
     dupeSet=set()
     log.debug(f"[bold]Timeline Count with Dupes[/bold] {len(responseArray)} found")
     for post in sorted(responseArray,key=lambda x:x["postedAtPrecise"]):
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
+        oldtimeset.discard(post["id"])
         unduped.append(post)
     log.debug(f"[bold]Timeline Count without Dupes[/bold] {len(unduped)} found")
-    cache.set(f"timeline_{model_id}",unduped,expire=constants.RESPONSE_EXPIRY)
-    cache.close() 
+    if len(oldtimeset)==0:
+        cache.set(f"timeline_{model_id}",unduped,expire=constants.RESPONSE_EXPIRY)
+        cache.close()
+    else:
+        cache.set(f"timeline_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
+        cache.close()
+        log.debug("Some post where not retrived resetting cache")
 
     return unduped                                
 
 def get_archive_post(headers,model_id):
     return scrape_archived_posts(headers,model_id)
```

### Comparing `ofscraper-1.95.2/ofscraper/constants.py` & `ofscraper-2.0/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/db/operations.py` & `ofscraper-2.0/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/db/queries.py` & `ofscraper-2.0/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/interaction/like.py` & `ofscraper-2.0/ofscraper/interaction/like.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,33 +23,32 @@
 
 log=logging.getLogger(__package__)
 
 
 
 
 def get_posts(headers, model_id):
-    with Halo(text='Getting all timeline posts...'):
-        pinned_posts = timeline.scrape_pinned_posts(headers, model_id)
-        timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
-        archived_posts = timeline.scrape_archived_posts(headers, model_id)
+    pinned_posts = timeline.scrape_pinned_posts(headers, model_id)
+    timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
+    archived_posts = timeline.scrape_archived_posts(headers, model_id)
     log.debug(f"[bold]Number of Post Found[/bold] {len(pinned_posts) + len(timeline_posts) + len(archived_posts)}")
     return pinned_posts + timeline_posts + archived_posts
 
 
 def filter_for_unfavorited(posts: list) -> list:
     output=list(filter(lambda x:x.get("isFavorite")==False,posts))
-    log.debug(f"[bold]Number of unliked post[/bold {len(output)}")
+    log.debug(f"[bold]Number of unliked post[/bold] {len(output)}")
     return output
 
 
 
 
 def filter_for_favorited(posts: list) -> list:
     output=list(filter(lambda x:x.get("isFavorite")==True,posts))
-    log.debug(f"[bold]Number of liked post[/bold {len(output)}")
+    log.debug(f"[bold]Number of liked post[/bold] {len(output)}")
     return output
 
 
 
 def get_post_ids(posts: list) -> list:
     valid_post=list(filter(lambda x:x.get("isOpened")==True,posts))
     return list(map(lambda x:x.get("id"),valid_post))
```

### Comparing `ofscraper-1.95.2/ofscraper/prompts/prompt_functions.py` & `ofscraper-2.0/ofscraper/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/prompts/prompts.py` & `ofscraper-2.0/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/scraper.py` & `ofscraper-2.0/ofscraper/scraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 
 console=Console()
 log=logger.init_logger(logging.getLogger(__package__))
 args=args_.getargs()
 log.debug(args)
 f = open(os.devnull, 'w')
 
-@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f ,text='Getting messages...')
 def process_messages(headers, model_id,username):
     messages_ =asyncio.run(messages.get_messages(headers,  model_id)) 
     messages_=list(map(lambda x:posts_.Post(x,model_id,username),messages_))
     log.debug(f"[bold]Messages Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),messages_))}")
     log.debug("Removing locked messages media")
     for message in messages_:
      operations.write_messages_table(message)
@@ -104,15 +103,15 @@
      
 
 
 
 
 
 
-@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting timeline media...')
+# @Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting timeline media...')
 def process_timeline_posts(headers, model_id,username):
     timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
     timeline_posts  =list(map(lambda x:posts_.Post(x,model_id,username,"timeline"), timeline_posts ))
     log.debug(f"[bold]Timeline Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),timeline_posts))}")
     log.debug("Removing locked timeline media")
     for post in timeline_posts:
         operations.write_post_table(post,model_id,username)
@@ -325,56 +324,92 @@
 
 def process_post():
     with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
         userdata=getselected_usernames()
-        for ele in userdata:
-            if args.posts:
-                log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
-            try:
-                model_id = profile.get_id(headers, ele["name"])
-                create_tables(model_id,ele['name'])
-                operations.write_profile_table(model_id,ele['name'])
-                combined_urls=process_areas(headers, ele, model_id)
-                asyncio.run(download.process_dicts(
-                ele["name"],
-                model_id,
-                combined_urls,
-                forced=args.dupe,
-                ))
-            except Exception as e:
-                log.traceback(f"failed with exception: {e}")
-                log.traceback(traceback.format_exc())
+        length=len(userdata)
+        if args.users_first:
+            eleDict={}
+            for count,ele in enumerate(userdata):
+                key=ele['name']
+                eleDict[key]={}
+                eleDict[key]["name"]=ele['name']
+                log.debug(f"getting content for {count+1}/{length} model")
+                if args.posts:
+                    log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
+                try:
+                    model_id = profile.get_id(headers, ele["name"])
+                    eleDict[key]["id"]=model_id
+                    create_tables(model_id,ele['name'])
+                    operations.write_profile_table(model_id,ele['name'])
+                    eleDict[key]["combined"]=process_areas(headers, ele, model_id)
+                
+                except Exception as e:
+                    log.traceback(f"failed with exception: {e}")
+                    log.traceback(traceback.format_exc())      
+            for key in eleDict.keys():
+                try:
+                    asyncio.run(download.process_dicts(
+                        eleDict[key]["name"],
+                        eleDict[key]["id"],
+                        eleDict[key]["combined"],
+                        forced=args.dupe,
+                        ))
+                except Exception as e:
+                    log.traceback(f"failed with exception: {e}")
+                    log.traceback(traceback.format_exc())   
+        else:
+            for count,ele in enumerate(userdata):
+                log.debug(f"Getting content+downloading {count+1}/{length} model")
+
+                if args.posts:
+                    log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
+                try:
+                    model_id = profile.get_id(headers, ele["name"])
+                    create_tables(model_id,ele['name'])
+                    operations.write_profile_table(model_id,ele['name'])
+                    combined_urls=process_areas(headers, ele, model_id)
+                    asyncio.run(download.process_dicts(
+                    ele["name"],
+                    model_id,
+                    combined_urls,
+                    forced=args.dupe,
+                    ))
+                except Exception as e:
+                    log.traceback(f"failed with exception: {e}")
+                    log.traceback(traceback.format_exc())
         
         
 
 def process_like():
     with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         userdata=getselected_usernames()
         for ele in list(filter(lambda x: x["active"],userdata)):
                 model_id = profile.get_id(headers, ele["name"])
                 posts = like.get_posts(headers, model_id)
-                unfavorited_posts = like.filter_for_unfavorited(posts)
+                unfavorited_posts = like.filter_for_unfavorited(posts)  
+                unfavorited_posts=filters.timeline_array_filter(unfavorited_posts)             
                 post_ids = like.get_post_ids(unfavorited_posts)
                 like.like(headers, model_id, ele["name"], post_ids)
 
 def process_unlike():
     with scrape_context_manager(): 
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
         userdata=getselected_usernames()
         for ele in list(filter(lambda x: x["active"],userdata)):
                 model_id = profile.get_id(headers, ele["name"])
                 posts = like.get_posts(headers, model_id)
                 favorited_posts = like.filter_for_favorited(posts)
+                favorited_posts=filters.timeline_array_filter(favorited_posts) 
                 post_ids = like.get_post_ids(favorited_posts)
                 like.unlike(headers, model_id, ele["name"], post_ids)
 #Adds a function to the job queue
 def set_schedule(*functs):
     [schedule.every(args.daemon).minutes.do(jobqueue.put,funct) for funct in functs]
     while True:
         schedule.run_pending()
@@ -431,54 +466,70 @@
         console.print("You need to select path for ffmpeg\n\n")
         log.debug(f"[bold]current ffmpeg path[/bold] {config.get_ffmpeg(config.read_config())}")
         config.update_ffmpeg()
     log.debug(f"[bold]final mp4decrypt path[/bold] {config.get_mp4decrypt(config.read_config())}")
     log.debug(f"[bold]final ffmpeg path[/bold] {config.get_ffmpeg(config.read_config())}")
 
 
-
-       
-
 def getselected_usernames():
-    #username list will be retrived once per run
+    #username list will be retrived once per daemon run
+    # manual prompt will need to recertify options every call
     global selectedusers
-    if selectedusers:
-        if len(args.posts)>0:
+    scraper_bool=len(args.posts)>0 or args.action
+    #always return with correct args
+    if selectedusers and scraper_bool:
             return selectedusers
-        elif prompts.reset_username_prompt()=="No":
-           return selectedusers
-        else:
+    if scraper_bool:
+        selectedusers=selectuserhelper()
+    #create in these situations
+    elif not selectedusers and not scraper_bool:
+        setfilter()
+        selectedusers=selectuserhelper()
+    elif selectedusers and not scraper_bool:
+        if prompts.reset_username_prompt()=="Yes":
             setfilter()
+            selectedusers=selectuserhelper()
+    return selectedusers
+
+def selectuserhelper():
+    headers = auth.make_headers(auth.read_auth())
+    subscribe_count = process_me(headers)
+    parsed_subscriptions = get_models(headers, subscribe_count)
+    filter_subscriptions=filteruserHelper(parsed_subscriptions )
+    if args.username and "ALL" in args.username:
+        selectedusers=filter_subscriptions
+        
+    elif args.username:
+        userSelect=set(args.username)
+        selectedusers=list(filter(lambda x:x["name"] in userSelect,filter_subscriptions))
+    #manually select usernames
     else:
-        if len(args.posts)==0:
-            setfilter()
-        headers = auth.make_headers(auth.read_auth())
-        subscribe_count = process_me(headers)
-        parsed_subscriptions = get_models(headers, subscribe_count)
-        filter_subscriptions=filteruserHelper(parsed_subscriptions )
-        if args.username and "ALL" in args.username:
-            selectedusers=filter_subscriptions
+        selectedusers= get_model(filter_subscriptions)
+    return selectedusers
+
         
 
-        elif args.username:
-            userSelect=set(args.username)
-            selectedusers=list(filter(lambda x:x["name"] in userSelect,filter_subscriptions))
-        #manually select usernames
-        else:
-            selectedusers= get_model(filter_subscriptions)
-        #remove dupes
-        return selectedusers
+        
+
+                  
+    # else:
+    #     if len(args.posts)==0 or args.action:
+           
+
+  
+    # #remove dupes
+    return selectedusers
 def filteruserHelper(usernames):
     #paid/free
     filterusername=usernames
     if args.account_type=="paid":
         filterusername=list(filter(lambda x:x["data"]["subscribePrice"]>0,filterusername))
     if args.account_type=="free":
         filterusername=list(filter(lambda x:x["data"]["subscribePrice"]==0,filterusername))
-    if args.renewal=="acive":
+    if args.renewal=="active":
         filterusername=list(filter(lambda x:x["data"]["subscribedOn"]==True,filterusername))     
     if args.renewal=="disabled":
         filterusername=list(filter(lambda x:x["data"]["subscribedOn"]==False,filterusername))      
     if args.sub_status=="active":
         filterusername=list(filter(lambda x:x["data"]["subscribedIsExpiredNow"]==False,filterusername))     
     if args.sub_status=="expired":
         filterusername=list(filter(lambda x:x["data"]["subscribedIsExpiredNow"]==True,filterusername))      
@@ -524,24 +575,23 @@
     
 # Python program for creating a
 # context manager using @contextmanager
 # decorator
  
     with exit.DelayedKeyboardInterrupt(paths.cleanup,False):
         try:
- 
-            scrapper()
-
-            
-
+            scrapper()        
         except Exception as E:
             log.traceback(E)
             log.traceback(traceback.format_exc())
         quit()
 def scrapper():
+    import time
+
+
     if platform.system == 'Windows':
         os.system('color')
     # try:
     #     webbrowser.open(donateEP)
     # except:
     #     pass
     global selectedusers
```

### Comparing `ofscraper-1.95.2/ofscraper/utils/args.py` & `ofscraper-2.0/ofscraper/utils/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,33 +44,38 @@
 
     post.add_argument("-e","--dupe",action="store_true",default=False,help="Bypass the dupe check and redownload all files")
     post.add_argument(
         '-o', '--posts', help = 'Download content from a model',default=[],required=False,type = posttype_helper,action='extend'
     )
     post.add_argument("-c","--letter-count",action="store_true",default=False,help="intrepret config 'textlength' as max length by letter")
     post.add_argument("-a","--action",default=None,help="perform like or unlike action on each post",choices=["like","unlike"])
-    post.add_argument(
-        '-be', '--before', help = 'Download post at or before the given date general synax is Month/Day/Year',type=arrow.get)
- 
-    post.add_argument(
-        '-af', '--after', help = 'Download post at or after the given date Month/Day/Year',type=arrow.get)
-    
-    
+   
      #Filters for accounts
     filters=parser.add_argument_group("filters",description="Filters out usernames based on selected parameters")
     
     filters.add_argument(
         '-t', '--account-type', help = 'Filter Free or paid accounts',default=None,required=False,type = str.lower,choices=["paid","free"]
     )
     filters.add_argument(
         '-r', '--renewal', help = 'Filter by whether renewal is on or off for account',default=None,required=False,type = str.lower,choices=["active","disabled"]
     )
     filters.add_argument(
         '-ss', '--sub-status', help = 'Filter by whether or not your subscription has expired or not',default=None,required=False,type = str.lower,choices=["active","expired"]
     )
+    filters.add_argument(
+        '-be', '--before', help = 'Process post at or before the given date general synax is Month/Day/Year\nWorks for like,unlike, and scraping posts',type=arrow.get)
+ 
+    filters.add_argument(
+        '-af', '--after', help = 'Process post at or after the given date Month/Day/Year\nnWorks for like,unlike, and scraping posts',type=arrow.get)
+    
+    
+    advanced=parser.add_argument_group("Advanced",description="Advanced Args")  
+    advanced.add_argument(
+        '-uf', '--users-first', help = 'Scrape all users first rather then one at a time. This only effects scraping posts',default=False,required=False,action="store_true"
+    )
 
     args=parser.parse_args(input)
     #deduplicate posts
     args.posts=list(set(args.posts or []))
     return args
```

### Comparing `ofscraper-1.95.2/ofscraper/utils/auth.py` & `ofscraper-2.0/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/utils/config.py` & `ofscraper-2.0/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/utils/dates.py` & `ofscraper-2.0/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/utils/download.py` & `ofscraper-2.0/ofscraper/utils/download.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,174 +16,183 @@
 import traceback
 import re
 import logging
 import httpx
 import contextvars
 import json
 import subprocess
-from rich.console import Console
-from tqdm.asyncio import tqdm
+from rich.progress import Progress
+from rich.progress import (
+    Progress,
+    TimeElapsedColumn,
+    TotalFileSizeColumn,
+    TransferSpeedColumn,
+    TextColumn,
+    TaskProgressColumn,
+    BarColumn
+)
+from rich.live import Live
+from rich.panel import Panel
+from rich.console import Group
 import arrow
 from bs4 import BeautifulSoup
 try:
     from win32_setctime import setctime  # pylint: disable=import-error
 except ModuleNotFoundError:
     pass
 from tenacity import retry,stop_after_attempt,wait_random,retry_if_result
+
+
 import ffmpeg
 import ofscraper.utils.config as config_
 import ofscraper.utils.separate as seperate
 import ofscraper.db.operations as operations
 import ofscraper.utils.paths as paths
 import ofscraper.utils.auth as auth
 import ofscraper.constants as constants
 import ofscraper.utils.dates as dates
 import ofscraper.utils.logger as logger
-from tqdm import tqdm
+import ofscraper.utils.console as console
 from diskcache import Cache
 
 cache = Cache(paths.getcachepath())
 attempt = contextvars.ContextVar("attempt")
 log=logging.getLogger(__package__)
-console=Console()
+
 
 async def process_dicts(username, model_id, medialist,forced=False):
-    if medialist:
-        if not forced:
-            media_ids = set(operations.get_media_ids(model_id,username))
-            medialist = seperate.separate_by_id(medialist, media_ids)
-            log.info(f"Skipping previously downloaded\nMedia left for download {len(medialist)}")
-        else:
-            log.info("forcing all downloads")
-        file_size_limit = config_.get_filesize()
-        global sem
-        sem = asyncio.Semaphore(8)
-      
-        aws=[]
-        photo_count = 0
-        video_count = 0
-        audio_count=0
-        skipped = 0
-        total_bytes_downloaded = 0
-        data = 0
-        desc = 'Progress: ({p_count} photos, {v_count} videos, {a_count} audios,  {skipped} skipped || {sumcount}/{mediacount}||{data})'    
+    overall_progress=Progress(  TextColumn("{task.description}"),
+    BarColumn(),TaskProgressColumn(),TimeElapsedColumn())
+    job_progress=Progress(*Progress.get_default_columns(),TransferSpeedColumn(),TotalFileSizeColumn())
+    progress_group = Group(
+    overall_progress
+    , Panel(Group(job_progress)))
+    with Live(progress_group, refresh_per_second=10,console=console.shared_console):    
+            if not forced:
+                media_ids = set(operations.get_media_ids(model_id,username))
+                medialist = seperate.separate_by_id(medialist, media_ids)
+                log.info(f"Skipping previously downloaded\nMedia left for download {len(medialist)}")
+            else:
+                log.info("forcing all downloads")
+            file_size_limit = config_.get_filesize()
+            global sem
+            sem = asyncio.Semaphore(8)
+        
+            aws=[]
+            photo_count = 0
+            video_count = 0
+            audio_count=0
+            skipped = 0
+            total_bytes_downloaded = 0
+            data = 0
+            desc = 'Progress: ({p_count} photos, {v_count} videos, {a_count} audios,  {skipped} skipped || {sumcount}/{mediacount}||{data})'    
+        
+            
 
-        with tqdm(desc=desc.format(p_count=photo_count, v_count=video_count,a_count=audio_count, skipped=skipped,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped,data=data), total=len(aws), colour='cyan', leave=True,disable=True if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else False) as main_bar:   
+            
             for ele in medialist:
                 with paths.set_directory(paths.getmediadir(ele,username,model_id)):
-
-                    aws.append(asyncio.create_task(download(ele,pathlib.Path(".").absolute() ,model_id, username,file_size_limit
-                                                            )))
+                    aws.append(asyncio.create_task(download(ele,pathlib.Path(".").absolute() ,model_id, username,file_size_limit,job_progress)))
+            task1 = overall_progress.add_task(desc.format(p_count=photo_count, v_count=video_count,a_count=audio_count, skipped=skipped,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped,data=data), total=len(aws),visible=False if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else True)
             for coro in asyncio.as_completed(aws):
                     try:
                         media_type, num_bytes_downloaded = await coro
                     except Exception as e:
                         log.traceback(e)
                         log.traceback(traceback.format_exc())
                         media_type = "skipped"
                         num_bytes_downloaded = 0
 
                     total_bytes_downloaded += num_bytes_downloaded
                     data = convert_num_bytes(total_bytes_downloaded)
                     if media_type == 'images':
-                        photo_count += 1
-                        main_bar.set_description(
-                            desc.format(
-                                p_count=photo_count, v_count=video_count, a_count=audio_count,skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True)
+                        photo_count += 1 
 
                     elif media_type == 'videos':
                         video_count += 1
-                        main_bar.set_description(
-                            desc.format(
-                                p_count=photo_count, v_count=video_count, a_count=audio_count ,skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True)
-
                     elif media_type == 'audios':
                         audio_count += 1
-                        main_bar.set_description(
-                            desc.format(
-                                p_count=photo_count, v_count=video_count,a_count=audio_count , skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True)
-
                     elif media_type == 'skipped':
                         skipped += 1
-                        main_bar.set_description(
-                            desc.format(
-                                p_count=photo_count, v_count=video_count,a_count=audio_count , skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True)
-
-                    main_bar.update()
-        log.warning(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios,  {skipped} skipped)' )
+                    overall_progress.update(task1,description=desc.format(
+                                p_count=photo_count, v_count=video_count, a_count=audio_count,skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True, advance=1)
+    overall_progress.remove_task(task1)
+    log.warning(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios,  {skipped} skipped)' )
 def retry_required(value):
     return value == ('skipped', 1)
 
 @retry(retry=retry_if_result(retry_required),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=20, max=40),reraise=True) 
-async def download(ele,path,model_id,username,file_size_limit):
+async def download(ele,path,model_id,username,file_size_limit,progress):
     attempt.set(attempt.get(0) + 1)
     
     try:
         if ele.url:
-           log.debug(f"ID:{ele.id} Downloading with normal downloader")
-           return await main_download_helper(ele,path,file_size_limit,username,model_id)
+           log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with normal downloader")
+           return await main_download_helper(ele,path,file_size_limit,username,model_id,progress)
         elif ele.mpd:  
-            log.debug(f"ID:{ele.id} Downloading with protected media downloader")      
-            return await alt_download_helper(ele,path,file_size_limit,username,model_id)
+            log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with protected media downloader")      
+            return await alt_download_helper(ele,path,file_size_limit,username,model_id,progress)
         else:
             return "skipped",1
     except Exception as e:
-        log.debug(f"ID:{ele.id} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {e}")   
-        log.debug(f"ID:{ele.id} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {traceback.format_exc()}")   
+        log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {e}")   
+        log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {traceback.format_exc()}")   
         return 'skipped', 1
-async def main_download_helper(ele,path,file_size_limit,username,model_id):
+async def main_download_helper(ele,path,file_size_limit,username,model_id,progress):
     url=ele.url
-    log.debug(f"ID:{ele.id} Attempting to download media {ele.filename} with {url}")
+    log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename} with {url}")
     path_to_file=None
     async with sem:
-            async with httpx.AsyncClient(http2=True, headers = auth.make_headers(auth.read_auth()), follow_redirects=True, timeout=None) as c: 
+            async with httpx.AsyncClient(http2=True, follow_redirects=True, timeout=None) as c: 
                 auth.add_cookies(c)        
                 async with c.stream('GET',url) as r:
                     if not r.is_error:
                         rheaders=r.headers
                         total = int(rheaders['Content-Length'])
                         if file_size_limit>0 and total > int(file_size_limit): 
                                 return 'skipped', 1       
                         content_type = rheaders.get("content-type").split('/')[-1]
                         filename=createfilename(ele,username,model_id,content_type)
                         path_to_file = paths.trunicate(pathlib.Path(path,f"{filename}"))                 
                         pathstr=str(path_to_file)
                         temp=paths.trunicate(f"{path_to_file}.part")
                         pathlib.Path(temp).unlink(missing_ok=True)
-                        with tqdm(desc=f"{attempt.get()}/{constants.NUM_TRIES} {(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr}" ,total=total, unit_scale=True, unit_divisor=1024, unit='B', leave=False,disable=True if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else False) as bar:
-                            with open(temp, 'wb') as f:                           
+                        task1 = progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} {(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr}", total=total,visible=False)
+                        with open(temp, 'wb') as f:                           
+                            num_bytes_downloaded = r.num_bytes_downloaded
+                            progress.update(task1,visible=False if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else True)
+                            async for chunk in r.aiter_bytes(chunk_size=1024):
+                                f.write(chunk)
+                                progress.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                                 num_bytes_downloaded = r.num_bytes_downloaded
-                                async for chunk in r.aiter_bytes(chunk_size=1024):
-                                    f.write(chunk)
-                                    bar.update(r.num_bytes_downloaded - num_bytes_downloaded)
-                                    num_bytes_downloaded = r.num_bytes_downloaded 
-            
+                            progress.remove_task(task1) 
+        
                     else:
                         r.raise_for_status()
     if not pathlib.Path(temp).exists():
-        log.debug(f"ID:{ele.id} [attempt {attempt.get()}/{constants.NUM_TRIES}] {temp} was not created") 
+        log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {temp} was not created") 
         return "skipped",1
     elif abs(total-pathlib.Path(temp).absolute().stat().st_size)>500:
-        log.debug(f"ID:{ele.id} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename} size mixmatch target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
+        log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename} size mixmatch target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
         return "skipped",1 
     else:
-        log.debug(f"ID:{ele.id} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename} size match target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
-        log.debug(f"ID:{ele.id} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(temp).absolute()} -> {path_to_file}")   
+        log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename} size match target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
+        log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(temp).absolute()} -> {path_to_file}")   
         shutil.move(temp,path_to_file)
         if ele.postdate:
             newDate=dates.convert_local_time(ele.postdate)
-            log.debug(f"ID:{ele.id} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
+            log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
             set_time(path_to_file,newDate )
-            log.debug(f"ID:{ele.id} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
+            log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
 
         if ele.id:
             operations.write_media_table(ele,path_to_file,model_id,username)
         return ele.mediatype,total
 
-async def alt_download_helper(ele,path,file_size_limit,username,model_id):
+async def alt_download_helper(ele,path,file_size_limit,username,model_id,progress):
     video = None
     audio = None
     base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
     mpd=ele.parse_mpd
     path_to_file = paths.trunicate(pathlib.Path(path,f'{createfilename(ele,username,model_id,"mp4")}')) 
 
     for period in mpd.periods:
@@ -206,15 +215,15 @@
                     logger.updateSenstiveDict(kId,"pssh_code")
                     break
             for repr in adapt_set.representations:
                 audio={"name":repr.base_urls[0].base_url_value,"pssh":kId,"type":"audio"}
                 break
         for item in [audio,video]:
             url=f"{base_url}{item['name']}"
-            log.debug(f"ID:{ele.id} Attempting to download media {item['name']} with {url}")
+            log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {item['name']} with {url}")
             async with sem:
                 params={"Policy":ele.policy,"Key-Pair-Id":ele.keypair,"Signature":ele.signature}   
                 async with httpx.AsyncClient(http2=True, headers = auth.make_headers(auth.read_auth()), follow_redirects=True, timeout=None,params=params) as c: 
                     auth.add_cookies(c) 
                     async with c.stream('GET',url) as r:
                         if not r.is_error:
                             rheaders=r.headers
@@ -222,54 +231,56 @@
                             item["total"]=total
                             if file_size_limit>0 and total > int(file_size_limit): 
                                     return 'skipped', 1       
                             temp= paths.trunicate(pathlib.Path(path,f"{item['name']}.part"))
                             temp.unlink(missing_ok=True)
                             item["path"]=temp
                             pathstr=str(temp)
-                            with tqdm(desc=f"{attempt.get()}/{constants.NUM_TRIES} {(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr}" ,total=total, unit_scale=True, unit_divisor=1024, unit='B', leave=False,disable=True if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else False) as bar:
-                                with open(temp, 'wb') as f:                           
+                            task1 = progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} {(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr}", total=total,visible=False)
+                            with open(temp, 'wb') as f:                           
+                                num_bytes_downloaded = r.num_bytes_downloaded
+                                progress.update(task1,visible=False if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else True)
+                                async for chunk in r.aiter_bytes(chunk_size=1024):
+                                    f.write(chunk)
+                                    progress.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                                     num_bytes_downloaded = r.num_bytes_downloaded
-                                    async for chunk in r.aiter_bytes(chunk_size=1024):
-                                        f.write(chunk)
-                                        bar.update(r.num_bytes_downloaded - num_bytes_downloaded)
-                                        num_bytes_downloaded = r.num_bytes_downloaded      
+                                progress.remove_task(task1) 
                         else:
                             r.raise_for_status()
-    log.debug(f"ID:{ele.id} video name:{video['name']}")
-    log.debug(f"ID:{ele.id} audio name:{audio['name']}")
+    log.debug(f"Media:{ele.id} Post:{ele.postid} video name:{video['name']}")
+    log.debug(f"Media:{ele.id} Post:{ele.postid} audio name:{audio['name']}")
     for item in [audio,video]:
         if not pathlib.Path(item["path"]).exists():
-                log.debug(f"ID:{ele.id} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['path']} was not created") 
+                log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['path']} was not created") 
                 return "skipped",1
         elif abs(item["total"]-pathlib.Path(item['path']).absolute().stat().st_size)>500:
-            log.debug(f"ID:{ele.id} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['name']} size mixmatch target: {total} vs actual: {pathlib.Path(item['path']).absolute().stat().st_size}")   
+            log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['name']} size mixmatch target: {total} vs actual: {pathlib.Path(item['path']).absolute().stat().st_size}")   
             return "skipped",1 
                 
     for item in [audio,video]:
         key=await key_helper(item["pssh"],ele.license,ele.id)
         if key==None:
-            log.debug(f"ID:{ele.id} Could not get key")
+            log.debug(f"Media:{ele.id} Post:{ele.postid} Could not get key")
             return "skipped",1 
-        log.debug(f"ID:{ele.id} got key")
+        log.debug(f"Media:{ele.id} Post:{ele.postid} got key")
         newpath=pathlib.Path(re.sub("\.part$","",str(item["path"]),re.IGNORECASE))
-        log.debug(f"ID:{ele.id} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(item['path']).absolute()} -> {newpath}")   
+        log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(item['path']).absolute()} -> {newpath}")   
         subprocess.run([config_.get_mp4decrypt(config_.read_config()),"--key",key,str(item["path"]),str(newpath)])
         pathlib.Path(item["path"]).unlink(missing_ok=True)
         item["path"]=newpath
     path_to_file.unlink(missing_ok=True)
    
     ffmpeg.output( ffmpeg.input(str(video["path"])), ffmpeg.input(str(audio["path"])), str(path_to_file),codec='copy',loglevel="quiet").overwrite_output().run(capture_stdout=True,cmd=config_.get_ffmpeg(config_.read_config()))
     video["path"].unlink(missing_ok=True)
     audio["path"].unlink(missing_ok=True)
     if ele.postdate:
         newDate=dates.convert_local_time(ele.postdate)
-        log.debug(f"ID:{ele.id} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
+        log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
         set_time(path_to_file,newDate )
-        log.debug(f"ID:{ele.id} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
+        log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
     if ele.id:
         operations.write_media_table(ele,path_to_file,model_id,username)
     return ele.mediatype,total
 
 async def key_helper(pssh,licence_url,id):
     out=cache.get(licence_url)
     log.debug(f"ID:{id} pssh: {pssh!=None}")
```

### Comparing `ofscraper-1.95.2/ofscraper/utils/encoding.py` & `ofscraper-2.0/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/utils/exit.py` & `ofscraper-2.0/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/utils/filters.py` & `ofscraper-2.0/ofscraper/utils/filters.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,38 +4,49 @@
 import ofscraper.utils.config as config
 import ofscraper.utils.args as args_
 
 args=args_.getargs()
 log=logging.getLogger(__package__)
 def filterMedia(media):
     media=dupefilter(media)
-    media=datesorter(media)
+    media=post_datesorter(media)
     media=posts_type_filter(media)
     media=posts_date_filter(media)
     return media
 
-def date_filter(media):
-    media=media
-    print("test")
-
 
 def dupefilter(media):
     output=[]
     ids=set()
     log.info("Removing duplicate media")
     log.debug(f"[bold]Combined Media Count with dupes[/bold]  {len(media)}")
     for item in media:
         if not item.id or item.id not in ids:
             output.append(item)
             ids.add(item.id)
     log.debug(f"[bold]Combined Media Count without dupes[/bold] {len(output)}")
     return output
-def datesorter(output):
+def post_datesorter(output):
     return list(sorted(output,key=lambda x:x.date,reverse=True))
 
+
+
+    
+def timeline_array_filter(posts):
+    out=[]
+    undated=filter(lambda x:x.get("postedAt")==None,posts)
+    dated=filter(lambda x:x.get("postedAt")!=None,posts)
+    dated=sorted(dated,key=lambda x:arrow.get(x.get("postedAt")))
+    if args.before:
+        dated=list(filter(lambda x:arrow.get(x.get("postedAt"))<=args.before,dated))
+    if args.after:
+         dated=list(filter(lambda x:arrow.get(x.get("postedAt"))>=args.after,dated))
+    out.extend(undated)
+    out.extend(dated)
+    return out
 def posts_type_filter(media): 
     filtersettings=config.get_filter(config.read_config())
     if isinstance(filtersettings,str):
         filtersettings=filtersettings.split(",")
     if isinstance(filtersettings,list):
         filtersettings=list(map(lambda x:x.lower().replace(" ",""),filtersettings))
         filtersettings=list(filter(lambda x:x!="",filtersettings))
```

### Comparing `ofscraper-1.95.2/ofscraper/utils/logger.py` & `ofscraper-2.0/ofscraper/utils/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import logging
 import re
 import httpx
 import logging
 from rich.logging import RichHandler
-from rich.console import Console
-from rich.theme import Theme
 import ofscraper.utils.paths as paths
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args
+import ofscraper.utils.console as console
 
 senstiveDict={}
 
 class DebugOnly(logging.Filter):
     def filter(self, record):
         if record.levelname=="DEBUG" or record.levelname=="TRACEBACK":
             return True
@@ -84,27 +83,30 @@
 def getLevel(input):
     """
     ERROR 50
     WARNING 30
     INFO 20
     DEBUG 10
     """
-    return {"OFF":100,"PROMPT":"ERROR","LOW":"WARNING","NORMAL":"INFO","DEBUG":"DEBUG"}.get(input,100)
+    return {"OFF":100,
+            "PROMPT":"ERROR",
+            "LOW":"WARNING",
+            "NORMAL":"INFO",
+            "DEBUG":"DEBUG"}.get(input,100)
 
 def init_logger(log):
     log.setLevel(1)
     addtrackback()
     # # #log file
       # #discord
     cord=DiscordHandler()
     cord.setLevel(getLevel(args.getargs().discord))
     cord.setFormatter(SensitiveFormatter('%(message)s'))
-    console = Console(theme=Theme({"logging.level.error":"green","logging.level.warning": "green","logging.level.debug":"yellow","logging.level.info":"white","logging.level.traceback":"red"}))
     #console
-    sh=RichHandler(rich_tracebacks=True, console=console,markup=True,tracebacks_show_locals=True,show_time=False,show_level=False)
+    sh=RichHandler(rich_tracebacks=True,markup=True,tracebacks_show_locals=True,show_time=False,show_level=False,console=console.shared_console)
     sh.setLevel(getLevel(args.getargs().output))
     sh.setFormatter(SensitiveFormatter('%(message)s'))
     sh.addFilter(NoDebug())
     log.addHandler(cord)
     log.addHandler(sh)
     if args.getargs().log!="OFF":
         stream=open(paths.getlogpath(), encoding='utf-8',mode="a",)
@@ -112,15 +114,15 @@
         fh.setLevel(getLevel(args.getargs().log))
         fh.setFormatter(LogFileFormatter('%(asctime)s - %(message)s',"%Y-%m-%d %H:%M:%S"))
         fh.addFilter(NoDebug())
         log.addHandler(fh)
 
     
     if args.getargs().output=="DEBUG":
-        sh2=RichHandler(rich_tracebacks=True, console=console,markup=True,tracebacks_show_locals=True,show_time=False)
+        sh2=RichHandler(rich_tracebacks=True, console=console.shared_console,markup=True,tracebacks_show_locals=True,show_time=False)
         sh2.setLevel(args.getargs().output)
         sh2.setFormatter(SensitiveFormatter('%(message)s'))
         sh2.addFilter(DebugOnly())
         log.addHandler(sh2)
     if args.getargs().log=="DEBUG":
         fh2=logging.StreamHandler(stream)
         fh2.setLevel(getLevel(args.getargs().log))
```

### Comparing `ofscraper-1.95.2/ofscraper/utils/paths.py` & `ofscraper-2.0/ofscraper/utils/paths.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,46 +88,41 @@
         return _windows_trunicateHelper(path)
     elif platform.system() == 'Linux':
         return _linux_trunicateHelper(path)
     else:
         return pathlib.Path(path)
 def _windows_trunicateHelper(path):
     path=pathlib.Path(path)
-    if re.search("\.[a-z]*$",path.name,re.IGNORECASE):
-        ext=re.search("\.[a-z]*$",path.name,re.IGNORECASE).group(0)
+    dir=path.parent
+    file=path.name
+    match=re.search("_[0-9]+\.[a-z]*$",path.name,re.IGNORECASE) or re.search("\.[a-z]*$",path.name,re.IGNORECASE)
+    if match:
+        ext=match.group(0)
     else:
         ext=""
-    filebase=str(path.with_suffix("").name)
-    dir=path.parent
-    #-1 for path split /
-    maxLength=256-len(ext)-len(str(dir))-1
-    outString=""
-    for ele in list(filebase):
-        temp=outString+ele
-        if len(temp)>maxLength:
-            break
-        outString=temp
-    return pathlib.Path(f"{pathlib.Path(dir,outString)}{ext}")
+    #-1 is for / between parentdirs and file
+    fileLength=256-len(ext)-len(str(dir))-1
+    newFile=f"{re.sub(ext,'',file)[fileLength]}{ext}"
+    return pathlib.Path(dir,newFile)
 
 def _linux_trunicateHelper(path):
     path=pathlib.Path(path)
-    if re.search("\.[a-z]*$",path.name,re.IGNORECASE):
-        ext=re.search("\.[a-z]*$",path.name,re.IGNORECASE).group(0)
+    dir=path.parent
+    file=path.name
+    match=re.search("_[0-9]+\.[a-z]*$",path.name,re.IGNORECASE) or re.search("\.[a-z]*$",path.name,re.IGNORECASE)
+    if match:
+        ext=match.group(0)
     else:
         ext=""
-    filebase=str(re.sub(ext,"",path.name))
-    dir=path.parent
-    maxLength=255-len(ext.encode('utf8'))
-    outString=""
-    for ele in list(filebase):
-        temp=outString+ele
-        if len(temp.encode("utf8"))>maxLength:
-            break
-        outString=temp
-    return pathlib.Path(f"{pathlib.Path(dir,outString)}{ext}")
+    fileLength=255-len(ext.encode('utf8'))
+    newFileByte=re.sub(ext,"",file).encode("utf8")[:fileLength]
+    newFile=f"{newFileByte.decode('utf8')}{ext}"
+    return pathlib.Path(dir,newFile)
+
+
 
 def mp4decryptchecker(x):
     if not pathlib.Path(x).is_file():
         return False
     try:
         t=subprocess.run([x],stdout=subprocess.PIPE,stderr=subprocess.PIPE)
         if re.search("mp4decrypt",t.stdout.decode())!=None or  re.search("mp4decrypt",t.stderr.decode())!=None:
```

### Comparing `ofscraper-1.95.2/ofscraper/utils/profiles.py` & `ofscraper-2.0/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/ofscraper/utils/separate.py` & `ofscraper-2.0/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.95.2/pyproject.toml` & `ofscraper-2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "ofscraper"
-version = "1.95.2"
+version = "2.0"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 packages = [{include = "ofscraper"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
 inquirerpy = "^0.3.4"
-tqdm = "^4.65.0"
 setuptools = "^67.6.0"
 schedule = "^1.1.0"
 browser-cookie3 = "^0.17.1"
 requests = "^2.28.2"
 bs4 = "^0.0.1"
 rich = "^13.3.2"
 tenacity = "^8.2.2"
```

### Comparing `ofscraper-1.95.2/PKG-INFO` & `ofscraper-2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.95.2
+Version: 2.0
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -24,15 +24,14 @@
 Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
 Requires-Dist: poetry-dynamic-versioning (>=0.22.0,<0.23.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
 Project-URL: Homepage, https://github.com/datawhores/OF-Scraper
 Description-Content-Type: text/markdown
 
 A fork of onlyfans-scraper. It has been optimized to make it more feature complete with digitalcriminal's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
```


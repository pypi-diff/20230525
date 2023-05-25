# Comparing `tmp/freeGPT-1.0.8.tar.gz` & `tmp/freeGPT-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-fr_ututs\freeGPT-1.0.8.tar", last modified: Thu May 25 17:06:54 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-_jzlibhi\freeGPT-1.0.9.tar", last modified: Thu May 25 17:30:27 2023, max compression
```

## Comparing `freeGPT-1.0.8.tar` & `freeGPT-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.041076 freeGPT-1.0.8/
--rw-rw-rw-   0        0        0    35149 2023-05-25 17:06:10.000000 freeGPT-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-25 17:06:10.000000 freeGPT-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3273 2023-05-25 17:06:54.041076 freeGPT-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2269 2023-05-25 17:06:10.000000 freeGPT-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT/
--rw-rw-rw-   0        0        0     1336 2023-05-25 17:06:10.000000 freeGPT-1.0.8/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     2042 2023-05-25 17:06:10.000000 freeGPT-1.0.8/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT/gpt3web/
--rw-rw-rw-   0        0        0     5176 2023-05-25 17:06:10.000000 freeGPT-1.0.8/freeGPT/gpt3web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     2662 2023-05-25 17:06:10.000000 freeGPT-1.0.8/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT/gpt4web/
--rw-rw-rw-   0        0        0     8418 2023-05-25 17:06:10.000000 freeGPT-1.0.8/freeGPT/gpt4web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3273 2023-05-25 17:06:53.000000 freeGPT-1.0.8/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-05-25 17:06:54.000000 freeGPT-1.0.8/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 17:06:53.000000 freeGPT-1.0.8/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-25 17:06:53.000000 freeGPT-1.0.8/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 17:06:53.000000 freeGPT-1.0.8/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 17:06:54.041076 freeGPT-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1396 2023-05-25 17:06:10.000000 freeGPT-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.659539 freeGPT-1.0.9/
+-rw-rw-rw-   0        0        0    35149 2023-05-25 17:06:10.000000 freeGPT-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-25 17:06:10.000000 freeGPT-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3273 2023-05-25 17:30:27.659539 freeGPT-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2269 2023-05-25 17:06:10.000000 freeGPT-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.628285 freeGPT-1.0.9/freeGPT/
+-rw-rw-rw-   0        0        0     1336 2023-05-25 17:28:53.000000 freeGPT-1.0.9/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.643912 freeGPT-1.0.9/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     2223 2023-05-25 17:28:36.000000 freeGPT-1.0.9/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.643912 freeGPT-1.0.9/freeGPT/gpt3web/
+-rw-rw-rw-   0        0        0     5176 2023-05-25 17:06:10.000000 freeGPT-1.0.9/freeGPT/gpt3web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.643912 freeGPT-1.0.9/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     2662 2023-05-25 17:06:10.000000 freeGPT-1.0.9/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.643912 freeGPT-1.0.9/freeGPT/gpt4web/
+-rw-rw-rw-   0        0        0     8418 2023-05-25 17:06:10.000000 freeGPT-1.0.9/freeGPT/gpt4web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.643912 freeGPT-1.0.9/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3273 2023-05-25 17:30:27.000000 freeGPT-1.0.9/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-05-25 17:30:27.000000 freeGPT-1.0.9/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 17:30:27.000000 freeGPT-1.0.9/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-25 17:30:27.000000 freeGPT-1.0.9/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 17:30:27.000000 freeGPT-1.0.9/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 17:30:27.659539 freeGPT-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2023-05-25 17:30:00.000000 freeGPT-1.0.9/setup.py
```

### Comparing `freeGPT-1.0.8/LICENSE` & `freeGPT-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.8/PKG-INFO` & `freeGPT-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.8
+Version: 1.0.9
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
```

### Comparing `freeGPT-1.0.8/README.md` & `freeGPT-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.8/freeGPT/__init__.py` & `freeGPT-1.0.9/freeGPT/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from freeGPT import gpt3, gpt3web, gpt4, gpt4web
 
 __author__ = "Ruu3f"
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 class Provider(Enum):
     GPT3 = 'gpt3'
     GPT3WEB = 'gpt3web'
     GPT4 = 'gpt4'
     GPT4WEB = 'gpt4web'
```

### Comparing `freeGPT-1.0.8/freeGPT/gpt3/__init__.py` & `freeGPT-1.0.9/freeGPT/gpt3/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from queue import Queue, Empty
+import json
 from threading import Thread
-from typing import Generator, Optional
-from curl_cffi import requests
+from curl_cffi import CurlEasy
+from queue import Queue, Empty
 from fake_useragent import UserAgent
+from typing import Generator, Optional
 
 
 class Completion:
     """
     A class for generating chat completions using the chatbot API.
     """
 
@@ -24,26 +25,33 @@
         headers = {
             "authority": "chatbot.theb.ai",
             "content-type": "application/json",
             "origin": "https://chatbot.theb.ai",
             "user-agent": UserAgent().random,
         }
 
-        proxies = (
-            {"http": "http://" + proxy, "https": "http://" + proxy} if proxy else None
-        )
-
-        response = requests.post(
-            "https://chatbot.theb.ai/api/chat-completion",
-            headers=headers,
-            proxies=proxies,
-            json={"role": "assistant", "prompt": prompt, "options": {}},
-        )
+        c = CurlEasy()
+        c.setopt(c.URL, "https://chatbot.theb.ai/api/chat-completion")
+        c.setopt(c.HTTPHEADER, [f"{k}: {v}" for k, v in headers.items()])
+        if proxy:
+            c.setopt(c.PROXY, proxy)
+
+        data = {
+            "role": "assistant",
+            "prompt": prompt,
+            "options": {},
+        }
+        c.setopt(c.POSTFIELDS, json.dumps(data))
+
+        c.setopt(c.WRITEFUNCTION, Completion.handle_response)
+        c.perform()
 
-        completion = json.loads(response.text)["delta"]
+    @staticmethod
+    def handle_response(body):
+        completion = json.loads(body.decode())["delta"]
         Completion.message_queue.put(completion)
 
     @staticmethod
     def create(prompt: str, proxy: Optional[str] = None) -> Generator[str, None, None]:
         """
         Creates a generator that yields chat completions for the given prompt.
 
@@ -56,8 +64,8 @@
         """
         Thread(target=Completion.request, args=[prompt, proxy]).start()
 
         try:
             completion = Completion.message_queue.get(timeout=10)
             yield completion
         except Empty:
-            raise Exception("Unable to get the response, please try again later.")
+            raise Exception("Unable to get the response, please try again later.")
```

### Comparing `freeGPT-1.0.8/freeGPT/gpt3web/__init__.py` & `freeGPT-1.0.9/freeGPT/gpt3web/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.8/freeGPT/gpt4/__init__.py` & `freeGPT-1.0.9/freeGPT/gpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.8/freeGPT/gpt4web/__init__.py` & `freeGPT-1.0.9/freeGPT/gpt4web/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.8/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.0.9/freeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.8
+Version: 1.0.9
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
```

### Comparing `freeGPT-1.0.8/setup.py` & `freeGPT-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.0.8",
+    version="1.0.9",
     description="freeGPT is a Python package that gives free access to GPT3 and GPT4 models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
```


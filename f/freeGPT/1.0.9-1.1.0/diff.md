# Comparing `tmp/freeGPT-1.0.9.tar.gz` & `tmp/freeGPT-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-_jzlibhi\freeGPT-1.0.9.tar", last modified: Thu May 25 17:30:27 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-fhwkn9co\freeGPT-1.1.0.tar", last modified: Thu May 25 17:45:34 2023, max compression
```

## Comparing `freeGPT-1.0.9.tar` & `freeGPT-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.659539 freeGPT-1.0.9/
--rw-rw-rw-   0        0        0    35149 2023-05-25 17:06:10.000000 freeGPT-1.0.9/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-25 17:06:10.000000 freeGPT-1.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3273 2023-05-25 17:30:27.659539 freeGPT-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2269 2023-05-25 17:06:10.000000 freeGPT-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.628285 freeGPT-1.0.9/freeGPT/
--rw-rw-rw-   0        0        0     1336 2023-05-25 17:28:53.000000 freeGPT-1.0.9/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.643912 freeGPT-1.0.9/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     2223 2023-05-25 17:28:36.000000 freeGPT-1.0.9/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.643912 freeGPT-1.0.9/freeGPT/gpt3web/
--rw-rw-rw-   0        0        0     5176 2023-05-25 17:06:10.000000 freeGPT-1.0.9/freeGPT/gpt3web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.643912 freeGPT-1.0.9/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     2662 2023-05-25 17:06:10.000000 freeGPT-1.0.9/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.643912 freeGPT-1.0.9/freeGPT/gpt4web/
--rw-rw-rw-   0        0        0     8418 2023-05-25 17:06:10.000000 freeGPT-1.0.9/freeGPT/gpt4web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:30:27.643912 freeGPT-1.0.9/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3273 2023-05-25 17:30:27.000000 freeGPT-1.0.9/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-05-25 17:30:27.000000 freeGPT-1.0.9/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 17:30:27.000000 freeGPT-1.0.9/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-25 17:30:27.000000 freeGPT-1.0.9/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 17:30:27.000000 freeGPT-1.0.9/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 17:30:27.659539 freeGPT-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1396 2023-05-25 17:30:00.000000 freeGPT-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.641065 freeGPT-1.1.0/
+-rw-rw-rw-   0        0        0    35149 2023-05-25 17:06:10.000000 freeGPT-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-25 17:06:10.000000 freeGPT-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3273 2023-05-25 17:45:34.641065 freeGPT-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2269 2023-05-25 17:06:10.000000 freeGPT-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT/
+-rw-rw-rw-   0        0        0     1336 2023-05-25 17:39:20.000000 freeGPT-1.1.0/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     2208 2023-05-25 17:41:54.000000 freeGPT-1.1.0/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT/gpt3web/
+-rw-rw-rw-   0        0        0     5176 2023-05-25 17:06:10.000000 freeGPT-1.1.0/freeGPT/gpt3web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     2662 2023-05-25 17:06:10.000000 freeGPT-1.1.0/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT/gpt4web/
+-rw-rw-rw-   0        0        0     8418 2023-05-25 17:06:10.000000 freeGPT-1.1.0/freeGPT/gpt4web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3273 2023-05-25 17:45:34.000000 freeGPT-1.1.0/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-05-25 17:45:34.000000 freeGPT-1.1.0/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 17:45:34.000000 freeGPT-1.1.0/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-25 17:45:34.000000 freeGPT-1.1.0/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 17:45:34.000000 freeGPT-1.1.0/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 17:45:34.641065 freeGPT-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1416 2023-05-25 17:38:18.000000 freeGPT-1.1.0/setup.py
```

### Comparing `freeGPT-1.0.9/LICENSE` & `freeGPT-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.9/PKG-INFO` & `freeGPT-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.9
+Version: 1.1.0
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
```

### Comparing `freeGPT-1.0.9/README.md` & `freeGPT-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.9/freeGPT/__init__.py` & `freeGPT-1.1.0/freeGPT/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from freeGPT import gpt3, gpt3web, gpt4, gpt4web
 
 __author__ = "Ruu3f"
-__version__ = "1.0.9"
+__version__ = "1.1.0"
 
 class Provider(Enum):
     GPT3 = 'gpt3'
     GPT3WEB = 'gpt3web'
     GPT4 = 'gpt4'
     GPT4WEB = 'gpt4web'
```

### Comparing `freeGPT-1.0.9/freeGPT/gpt3/__init__.py` & `freeGPT-1.1.0/freeGPT/gpt3/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import json
+import json, requests
 from threading import Thread
-from curl_cffi import CurlEasy
 from queue import Queue, Empty
 from fake_useragent import UserAgent
 from typing import Generator, Optional
 
 
 class Completion:
     """
@@ -25,29 +24,28 @@
         headers = {
             "authority": "chatbot.theb.ai",
             "content-type": "application/json",
             "origin": "https://chatbot.theb.ai",
             "user-agent": UserAgent().random,
         }
 
-        c = CurlEasy()
-        c.setopt(c.URL, "https://chatbot.theb.ai/api/chat-completion")
-        c.setopt(c.HTTPHEADER, [f"{k}: {v}" for k, v in headers.items()])
-        if proxy:
-            c.setopt(c.PROXY, proxy)
-
+        url = "https://chatbot.theb.ai/api/chat-completion"
         data = {
             "role": "assistant",
             "prompt": prompt,
             "options": {},
         }
-        c.setopt(c.POSTFIELDS, json.dumps(data))
+        
+        response = requests.post(url, headers=headers, json=data, proxies={'https': proxy} if proxy else None)
 
-        c.setopt(c.WRITEFUNCTION, Completion.handle_response)
-        c.perform()
+        if response.ok:
+            completion = response.json()["delta"]
+            Completion.message_queue.put(completion)
+        else:
+            response.raise_for_status()
 
     @staticmethod
     def handle_response(body):
         completion = json.loads(body.decode())["delta"]
         Completion.message_queue.put(completion)
 
     @staticmethod
```

### Comparing `freeGPT-1.0.9/freeGPT/gpt3web/__init__.py` & `freeGPT-1.1.0/freeGPT/gpt3web/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.9/freeGPT/gpt4/__init__.py` & `freeGPT-1.1.0/freeGPT/gpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.9/freeGPT/gpt4web/__init__.py` & `freeGPT-1.1.0/freeGPT/gpt4web/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.9/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.1.0/freeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.9
+Version: 1.1.0
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
```

### Comparing `freeGPT-1.0.9/setup.py` & `freeGPT-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.0.9",
+    version="1.1.0",
     description="freeGPT is a Python package that gives free access to GPT3 and GPT4 models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
@@ -36,14 +36,15 @@
         "Programming Language :: Python :: 3.10",
     ],
     packages=find_packages(),
     install_requires=[
         "pydantic",
         "pymailtm",
         "curl_cffi",
+        "requests",
         "fake-useragent",
     ],
     project_urls={
         "Source": "https://github.com/Ruu3f/freeGPT",
         "Issues": "https://github.com/Ruu3f/freeGPT/issues",
     },
 )
```


# Comparing `tmp/freeGPT-1.0.0.2.tar.gz` & `tmp/freeGPT-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-s8zeo95c\freeGPT-1.0.2.tar", last modified: Tue May 23 08:28:35 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-oyiaf5f4\freeGPT-1.0.3.tar", last modified: Thu May 25 14:39:04 2023, max compression
```

## Comparing `freeGPT-1.0.0.2.tar` & `freeGPT-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 08:28:35.747689 freeGPT-1.0.2/
--rw-rw-rw-   0        0        0    35149 2023-05-23 08:00:03.000000 freeGPT-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-23 08:00:03.000000 freeGPT-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3349 2023-05-23 08:28:35.747689 freeGPT-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2258 2023-05-23 08:00:03.000000 freeGPT-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 08:28:35.736288 freeGPT-1.0.2/freeGPT/
--rw-rw-rw-   0        0        0     2449 2023-05-23 08:28:09.000000 freeGPT-1.0.2/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:28:35.746353 freeGPT-1.0.2/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     2018 2023-05-23 08:00:03.000000 freeGPT-1.0.2/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:28:35.745331 freeGPT-1.0.2/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3349 2023-05-23 08:28:35.000000 freeGPT-1.0.2/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-23 08:28:35.000000 freeGPT-1.0.2/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 08:28:35.000000 freeGPT-1.0.2/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-23 08:28:35.000000 freeGPT-1.0.2/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 08:28:35.000000 freeGPT-1.0.2/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 08:28:35.747689 freeGPT-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-05-23 08:28:20.000000 freeGPT-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:39:04.667060 freeGPT-1.0.3/
+-rw-rw-rw-   0        0        0    35149 2023-05-25 14:37:43.000000 freeGPT-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-25 14:37:43.000000 freeGPT-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3265 2023-05-25 14:39:04.667060 freeGPT-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2261 2023-05-25 14:37:43.000000 freeGPT-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 14:39:04.667060 freeGPT-1.0.3/freeGPT/
+-rw-rw-rw-   0        0        0      146 2023-05-25 14:37:43.000000 freeGPT-1.0.3/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:39:04.667060 freeGPT-1.0.3/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     2042 2023-05-25 14:37:43.000000 freeGPT-1.0.3/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:39:04.667060 freeGPT-1.0.3/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     2662 2023-05-25 14:37:43.000000 freeGPT-1.0.3/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:39:04.667060 freeGPT-1.0.3/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3265 2023-05-25 14:39:04.000000 freeGPT-1.0.3/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-25 14:39:04.000000 freeGPT-1.0.3/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 14:39:04.000000 freeGPT-1.0.3/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-25 14:39:04.000000 freeGPT-1.0.3/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 14:39:04.000000 freeGPT-1.0.3/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 14:39:04.667060 freeGPT-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2023-05-25 14:37:43.000000 freeGPT-1.0.3/setup.py
```

### Comparing `freeGPT-1.0.2/LICENSE` & `freeGPT-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.2/PKG-INFO` & `freeGPT-1.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,79 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.2
-Summary: A Python package that provides free access to GPT3, GPT4, and more models.
+Version: 1.0.3
+Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
-Project-URL: Discussions, https://github.com/Ruu3f/freeGPT/discussions
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-#### *Latest: 5 MORE STARS FOR INTERNET SEARCH GPT MODELS*
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
+[![License](https://img.shields.io/badge/License-MIT-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
 *Get started by doing: `pip install freeGPT`*
 
-## Examples:
-
-#### GPT-3:
-
-```python
-from freeGPT import gpt3
-
-def send_prompt():
-    try:
-        prompt = input("> ")
-        response = gpt3.Completion.create(prompt=prompt)
-        print("Response:", response.text)
-    except Exception as e:
-        print("Error:", str(e))
-
-while True:
-    send_prompt()
-```
-#### GPT-4:
-
-```python
-from freeGPT import gpt4
-
-token = gpt4.Account.create(logging=True)
-print("Token:", token) 
-
-def send_prompt():
-    try:
-        prompt = input("> ")
-        for response in gpt4.Completion.create(prompt=prompt, token=token):
-            print("Response:", response.text)
-    except Exception as e:
-        print("Error:", str(e))
-
-while True:
-    send_prompt()
-```
-
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
 | gpt3              | [theb.ai](https://theb.ai)               |
 | gpt3.web          | [you.com](https://you.com)               |
-| gpt4              | [useless.com](https://ai.useless.com)    |
+| gpt4              | [usesless.com](https://ai.usesless.com)  |
 | gpt4.web          | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
-- [ ] Add a internet search model for GPT-3 & GPT-4
-- [ ] Make a discord bot
+- [x] Add a internet search model for GPT-3 & GPT-4
 - [ ] Add text to image generation
+- [ ] Make a discord bot
+
+## Support me:
+- Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
+- Star this repository :D
+
+## Examples:
+
+#### GPT-3:
+
+```python
+from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3.web as gpt3` and no other changes needed.
+
+prompt = input("👦 > ")
+resp = gpt3.Completion.create(prompt=prompt)
+print(f"🤖 > {resp.text}")
+```
+#### GPT-4:
+
+```python
+from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4.web as gpt4` and no other changes needed.
+
+token = gpt4.Account.create(logging=True) # Don't forget to remove this if you want to use web.
+prompt = input("👦 > ")
+resp = gpt4.Completion.create(prompt=prompt, token=token) # Don't forget to remove the token parameter here if you want to use web.
+print(f"🤖 > {resp.text}")
+```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
 
-## Discord Server:
-#### Join my server to support me :D
-#### -> [discord.gg/NcQ26PrNDp](https://discord.gg/NcQ26PrNDp)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `freeGPT-1.0.2/README.md` & `freeGPT-1.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,57 @@
-#### *Latest: 5 MORE STARS FOR INTERNET SEARCH GPT MODELS*
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
+[![License](https://img.shields.io/badge/License-MIT-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
 *Get started by doing: `pip install freeGPT`*
 
-## Examples:
-
-#### GPT-3:
-
-```python
-from freeGPT import gpt3
-
-def send_prompt():
-    try:
-        prompt = input("> ")
-        response = gpt3.Completion.create(prompt=prompt)
-        print("Response:", response.text)
-    except Exception as e:
-        print("Error:", str(e))
-
-while True:
-    send_prompt()
-```
-#### GPT-4:
-
-```python
-from freeGPT import gpt4
-
-token = gpt4.Account.create(logging=True)
-print("Token:", token) 
-
-def send_prompt():
-    try:
-        prompt = input("> ")
-        for response in gpt4.Completion.create(prompt=prompt, token=token):
-            print("Response:", response.text)
-    except Exception as e:
-        print("Error:", str(e))
-
-while True:
-    send_prompt()
-```
-
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
 | gpt3              | [theb.ai](https://theb.ai)               |
 | gpt3.web          | [you.com](https://you.com)               |
-| gpt4              | [useless.com](https://ai.useless.com)    |
+| gpt4              | [usesless.com](https://ai.usesless.com)  |
 | gpt4.web          | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
-- [ ] Add a internet search model for GPT-3 & GPT-4
-- [ ] Make a discord bot
+- [x] Add a internet search model for GPT-3 & GPT-4
 - [ ] Add text to image generation
+- [ ] Make a discord bot
+
+## Support me:
+- Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
+- Star this repository :D
+
+## Examples:
+
+#### GPT-3:
+
+```python
+from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3.web as gpt3` and no other changes needed.
+
+prompt = input("👦 > ")
+resp = gpt3.Completion.create(prompt=prompt)
+print(f"🤖 > {resp.text}")
+```
+#### GPT-4:
+
+```python
+from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4.web as gpt4` and no other changes needed.
+
+token = gpt4.Account.create(logging=True) # Don't forget to remove this if you want to use web.
+prompt = input("👦 > ")
+resp = gpt4.Completion.create(prompt=prompt, token=token) # Don't forget to remove the token parameter here if you want to use web.
+print(f"🤖 > {resp.text}")
+```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
 
-## Discord Server:
-#### Join my server to support me :D
-#### -> [discord.gg/NcQ26PrNDp](https://discord.gg/NcQ26PrNDp)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `freeGPT-1.0.2/freeGPT/gpt3/__init__.py` & `freeGPT-1.0.3/freeGPT/gpt3/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,30 +18,32 @@
         Sends a request to the chatbot API with the given prompt.
 
         Args:
             prompt (str): The input prompt for the chatbot.
             proxy (str, optional): The proxy server to use for the request. Defaults to None.
         """
         headers = {
-            'authority': 'chatbot.theb.ai',
-            'content-type': 'application/json',
-            'origin': 'https://chatbot.theb.ai',
-            'user-agent': UserAgent().random,
+            "authority": "chatbot.theb.ai",
+            "content-type": "application/json",
+            "origin": "https://chatbot.theb.ai",
+            "user-agent": UserAgent().random,
         }
 
-        proxies = {'http': 'http://' + proxy, 'https': 'http://' + proxy} if proxy else None
+        proxies = (
+            {"http": "http://" + proxy, "https": "http://" + proxy} if proxy else None
+        )
 
         response = requests.post(
-            'https://chatbot.theb.ai/api/chat-completion',
+            "https://chatbot.theb.ai/api/chat-completion",
             headers=headers,
             proxies=proxies,
-            json={'role': 'assistant', 'prompt': prompt, 'options': {}},
+            json={"role": "assistant", "prompt": prompt, "options": {}},
         )
 
-        completion = json.loads(response.text)['delta']
+        completion = json.loads(response.text)["delta"]
         Completion.message_queue.put(completion)
 
     @staticmethod
     def create(prompt: str, proxy: Optional[str] = None) -> Generator[str, None, None]:
         """
         Creates a generator that yields chat completions for the given prompt.
 
@@ -54,8 +56,8 @@
         """
         Thread(target=Completion.request, args=[prompt, proxy]).start()
 
         try:
             completion = Completion.message_queue.get(timeout=10)
             yield completion
         except Empty:
-            raise Exception('Unable to get the response, please try again later.')
+            raise Exception("Unable to get the response, please try again later.")
```

### Comparing `freeGPT-1.0.2/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.0.3/freeGPT.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,79 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.2
-Summary: A Python package that provides free access to GPT3, GPT4, and more models.
+Version: 1.0.3
+Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
-Project-URL: Discussions, https://github.com/Ruu3f/freeGPT/discussions
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-#### *Latest: 5 MORE STARS FOR INTERNET SEARCH GPT MODELS*
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
+[![License](https://img.shields.io/badge/License-MIT-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
 *Get started by doing: `pip install freeGPT`*
 
-## Examples:
-
-#### GPT-3:
-
-```python
-from freeGPT import gpt3
-
-def send_prompt():
-    try:
-        prompt = input("> ")
-        response = gpt3.Completion.create(prompt=prompt)
-        print("Response:", response.text)
-    except Exception as e:
-        print("Error:", str(e))
-
-while True:
-    send_prompt()
-```
-#### GPT-4:
-
-```python
-from freeGPT import gpt4
-
-token = gpt4.Account.create(logging=True)
-print("Token:", token) 
-
-def send_prompt():
-    try:
-        prompt = input("> ")
-        for response in gpt4.Completion.create(prompt=prompt, token=token):
-            print("Response:", response.text)
-    except Exception as e:
-        print("Error:", str(e))
-
-while True:
-    send_prompt()
-```
-
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
 | gpt3              | [theb.ai](https://theb.ai)               |
 | gpt3.web          | [you.com](https://you.com)               |
-| gpt4              | [useless.com](https://ai.useless.com)    |
+| gpt4              | [usesless.com](https://ai.usesless.com)  |
 | gpt4.web          | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
-- [ ] Add a internet search model for GPT-3 & GPT-4
-- [ ] Make a discord bot
+- [x] Add a internet search model for GPT-3 & GPT-4
 - [ ] Add text to image generation
+- [ ] Make a discord bot
+
+## Support me:
+- Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
+- Star this repository :D
+
+## Examples:
+
+#### GPT-3:
+
+```python
+from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3.web as gpt3` and no other changes needed.
+
+prompt = input("👦 > ")
+resp = gpt3.Completion.create(prompt=prompt)
+print(f"🤖 > {resp.text}")
+```
+#### GPT-4:
+
+```python
+from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4.web as gpt4` and no other changes needed.
+
+token = gpt4.Account.create(logging=True) # Don't forget to remove this if you want to use web.
+prompt = input("👦 > ")
+resp = gpt4.Completion.create(prompt=prompt, token=token) # Don't forget to remove the token parameter here if you want to use web.
+print(f"🤖 > {resp.text}")
+```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
 
-## Discord Server:
-#### Join my server to support me :D
-#### -> [discord.gg/NcQ26PrNDp](https://discord.gg/NcQ26PrNDp)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `freeGPT-1.0.2/setup.py` & `freeGPT-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.0.2",
-    description="A Python package that provides free access to GPT3, GPT4, and more models.",
+    version="1.0.3",
+    description="freeGPT is a Python package that gives free access to GPT3 and GPT4 models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
         "artificial-intelligence",
@@ -35,17 +35,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     packages=find_packages(),
     install_requires=[
         "pydantic",
         "pymailtm",
-        "requests",
         "curl_cffi",
         "fake-useragent",
     ],
     project_urls={
         "Source": "https://github.com/Ruu3f/freeGPT",
         "Issues": "https://github.com/Ruu3f/freeGPT/issues",
-        "Discussions": "https://github.com/Ruu3f/freeGPT/discussions",
     },
 )
```

